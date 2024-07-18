<template>
  <!-- <splashscreen /> -->
  <!-- <loginView /> -->
   <!-- <forgotPassword /> -->
    <signupView />
</template>
<script>
import splashscreen from '../components/splashscreen.vue'
import loginView from '~/components/enroll/loginView.vue'
import forgotPassword from '~/components/enroll/forgotPassword.vue';
import signupView from '~/components/enroll/signupView.vue';

export default{
  name: 'Home',
  components: {
    splashscreen,
    loginView,
    forgotPassword,
    signupView,
  },
}
</script>
<style>

</style>