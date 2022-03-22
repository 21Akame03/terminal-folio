<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import Terminal from './components/Terminal.vue'
</script>

<template>
  <Terminal id="terminal" />

  <div class="group">
    <div class="h-40 w-40 bottom-6 right-6 bg-white rounded-lg absolute -z-10 opacity-0 duration-500 group-hover:z-10 transform group-hover:opacity-100 font-mono grid">
      <p class="place-self-center">
        Password: <b class="underline">Password</b>
      </p>
    </div>

    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 fixed right-1 bottom-1 group group-hover:text-white cursor-pointer z-10 duration-200" viewBox="0 0 20 20" fill="currentColor">
      <path fill-rule="evenodd" d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-7-4a1 1 0 11-2 0 1 1 0 012 0zM9 9a1 1 0 000 2v3a1 1 0 001 1h1a1 1 0 100-2v-3a1 1 0 00-1-1H9z" clip-rule="evenodd" />

    </svg>
  </div>

</template>

<style>
@tailwind base;
@tailwind components;
@tailwind utilities;

body{
  margin: 0;
}

#terminal {
  border: 1px solid #ccc;
  flex: 1;
  margin: 1.5rem;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  background-color: #121920;
  position: absolute;
  height: 100%;
  width: 100%;
  display: flex;
}
</style>
