<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from "./components/HelloWorld.vue";
import TextOne from "./components/TextOne.vue";
import TextState from "./components/TextState.vue";
import Counter from "./components/Counter.vue";
import Greeting from "./components/Greeting.vue";
import Register from "./components/Register.vue";
import AuthUser from "./components/AuthUser.vue";
import UserList from './components/UserList.vue'
</script>

<template>
  <div>
    <!-- <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo mx-auto"  alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue mx-auto" alt="Vue logo" />
    </a> -->
  </div>
  <router-link to="/">Home</router-link> |
  <router-link to="/about">About</router-link> |
  <a href="/about"> A tag</a>
  <router-view></router-view>
  <h1 class="text-3xl font-bold underline">Hello world!</h1>

  <UserList/>

  <br><br><br>

  <AuthUser />

  <br /><br /><br />
  <Register />

  <br /><br />
  <Greeting />
  <br /><br /><br />
  <Counter />
  <br /><br /><br />
  <HelloWorld msg="Vite + Vue" />
  <br /><br /><br />
  <TextOne name="khan" age="27" designation="software engg" />
  <br /><br /><br />
  <TextState />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
