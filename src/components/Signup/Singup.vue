<template>

<form @click.prevent >
    <div class="row g-3 align-items-center">
        <h1>Sign Up</h1>
        <div class="col-auto d-block mx-auto">
            <input type="text" class="form-control" placeholder="Enter Your Name" v-model="name">
        </div>
    </div>
    <br>

    <div class="row g-3 align-items-center">

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
        <button type="submit" class="btn btn-primary">Sign Up Now</button> &nbsp;&nbsp;&nbsp;
        <button type="button" @click="login()" class="btn btn-primary">Login</button> 
        </div>
    </div>
    
</form>

</template>

<script>
export default {
    name: "SignUpForm",
    data(){
        return{
            name:'',
            email:'',
            pass:''
        }
    },
    methods: {
        login(){
            this.$router.push({path:"/login"})
        }
    
    },


};
</script>

<style lang="scss" scoped></style>
