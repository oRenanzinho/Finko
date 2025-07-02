<template>
  <LoginForm />
</template>

<script>
import LoginForm from './components/LoginForm.vue';

export default {
  name: 'App',
  components: {
    LoginForm
  }
}
</script>

<style>
body {
  background: linear-gradient(135deg, #00172e, #00eec6);
    margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
};
</style>