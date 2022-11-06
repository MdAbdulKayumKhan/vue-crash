<script>
export default {
  name: "Greeting",
  data: function(){
    return {
        msg: " "
    }
  },
  methods: {
    greet: function(value){
        this.msg = value;
    } 
  }
};
</script>

<template>
  <div class="flex justify-center">
   
    <div class="block p-6 rounded-lg shadow-lg bg-white max-w-sm">
      <h5 class="text-gray-900 text-xl leading-tight font-medium mb-2">
         <h1> Click event</h1>
        Msg {{this.msg}}
      </h5>
      <p class="text-gray-700 text-base mb-4">
        Some quick example text to build on the card title and make up the bulk
        of the card's content.
      </p>
      <button
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
        @click="greet('Goog Morning')"
      >
        Good Morning
      </button>
      <button
        type="button"
        class="
          inline-block
          px-6
          py-2
          border-2 border-purple-600
          text-purple-600
          font-medium
          text-xs
          leading-tight
          uppercase
          rounded
          hover:bg-black hover:bg-opacity-5
          focus:outline-none focus:ring-0
          transition
          duration-150
          ease-in-out
        "
        @click="greet('Good Afternoon')"
      >
        Good Afternoon
      </button>
      <button
        type="button"
        class="
          inline-block
          px-6
          py-2
          border-2 border-yellow-500
          text-yellow-500
          font-medium
          text-xs
          leading-tight
          uppercase
          rounded
          hover:bg-black hover:bg-opacity-5
          focus:outline-none focus:ring-0
          transition
          duration-150
          ease-in-out
        "
        @click="greet('Good Evening')"
      >
        Good Evening
      </button>
    </div>
  </div>
</template>