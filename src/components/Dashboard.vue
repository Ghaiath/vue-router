<template>
  <div>
    <h1>Dashboard</h1>
    <p>Welcome to the protected dashboard!</p>
    <button @click="Logout">Logout</button>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

const Logout = () => {
  localStorage.removeItem('auth');
  router.push("/login")
}

</script>
 