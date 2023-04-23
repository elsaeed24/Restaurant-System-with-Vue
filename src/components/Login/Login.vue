<template>

    <form @click.prevent >
      
        <div class="row g-3 align-items-center">
            <h1>Login</h1>
            <div class="col-auto d-block mx-auto">
                <input type="email" class="form-control" placeholder="Enter Your Email" v-model="email">
            </div>
        </div>
        <br>
    
        <div class="row g-3 align-items-center">
            
            <div class="col-auto d-block mx-auto">
                <input type="password" class="form-control" placeholder="Enter Your Password" v-model="pass">
            </div>
        </div>
        <br>
    
        <div class="row g-3 align-items-center">
            
            <div class="col-auto d-block mx-auto">
            <button type="submit" class="btn btn-primary">Login</button> &nbsp; &nbsp; &nbsp;
            <button type="button" @click="signUpPage()" class="btn btn-primary">Sign Up</button> 
            </div>
        </div>
        
    </form>
    
    </template>
    
    <script>
    export default {
        name: "LoginForm",
        data(){
            return{    
                email:'',
                pass:''
            };
        },
        methods: {
            signUpPage(){
                this.$router.push({path:"/sign-up"});
            }
        },
    
    
    };
    </script>
    
    <style lang="scss" scoped></style>
    