<template>
  <div>
    <h1>Login</h1>
    <button @click="Login">Login</button>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

const Login = () => {
  localStorage.setItem('auth', 'true');
  router.push("/dashboard")
}

</script>