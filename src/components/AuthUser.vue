<script>
export default {
  name: "AuthUser",
  data(){
    return {
        isLoggedIn: false
    }
  },
  methods: {
    login(){
        this.isLoggedIn = true;
    },
    logout(){
        this.isLoggedIn = false;
    }
  }
};
</script>

<template>
<!-- <pre>{{this.isLoggedIn}}</pre> -->
  <div class="flex justify-center">
    <div>
        <h2> Conditional check</h2>
    <div v-if="isLoggedIn" class="block p-6 rounded-lg shadow-lg bg-white max-w-sm">
      <h5 class="text-gray-900 text-xl leading-tight font-medium mb-2">
        Welcome User
      </h5>
      <p class="text-gray-700 text-base mb-4">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eveniet ipsa
        cum, est facere eos ut ea maxime adipisci vero in provident quisquam
        tenetur maiores, ullam atque pariatur at nemo corporis?
      </p>
    </div>
    <div v-if="!isLoggedIn" class="block p-6 rounded-lg shadow-lg bg-white max-w-sm">
      <h5 class="text-gray-900 text-xl leading-tight font-medium mb-2">
        Than You
      </h5>
      <p class="text-gray-700 text-base mb-4">
        Some quick example text to build on the card title and make up the bulk
        of the card's content. Lorem ipsum dolor sit amet, consectetur
        adipisicing elit. Ipsa doloribus quae soluta molestias dignissimos
        ducimus.
      </p>
    </div>
    <div>
        <button
        v-if="!isLoggedIn"
      type="button"
      class="
        inline-block
        px-6
        py-2.5
        bg-blue-600
        text-white
        font-medium
        text-xs
        leading-tight
        uppercase
        rounded
        shadow-md
        hover:bg-blue-700 hover:shadow-lg
        focus:bg-blue-700 focus:shadow-lg focus:outline-none focus:ring-0
        active:bg-blue-800 active:shadow-lg
        transition
        duration-150
        ease-in-out
      "
      @click="login()"
    >
      Login
    </button>
    <button
    v-if="isLoggedIn"
      type="button"
      class="
        inline-block
        px-6
        py-2.5
        bg-blue-600
        text-white
        font-medium
        text-xs
        leading-tight
        uppercase
        rounded
        shadow-md
        hover:bg-blue-700 hover:shadow-lg
        focus:bg-blue-700 focus:shadow-lg focus:outline-none focus:ring-0
        active:bg-blue-800 active:shadow-lg
        transition
        duration-150
        ease-in-out
      "
      @click="logout()"
    >
      Logout
    </button>
    </div>
    
    </div>
    
  </div>
</template>

<style>
</style>