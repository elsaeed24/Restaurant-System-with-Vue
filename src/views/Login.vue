<template>
    <div class="container">
  
      <LoginForm />
  
    </div>
  </template>
  
  <script>
  
  import LoginForm from "@/components/Login/Login.vue";
  
  export default {
      name: "Login",
      components: {
         LoginForm,    // name of component
      }
  
  }
  </script>
  
  <style>
  
  </style>