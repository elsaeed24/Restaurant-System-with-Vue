<template>
  <div class="container">

    <SignUpForm />

  </div>
</template>

<script>

import SignUpForm from "@/components/Signup/Singup.vue";

export default {
    name: "Signup",
    components: {
        SignUpForm,    // name of component
    }

}
</script>

<style>

</style>