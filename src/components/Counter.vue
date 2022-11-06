<script>
export default {
  name: "Counter",
  data: function () {
    return {
      count: 0,
    };
  },
  methods: {
    incre : function(){
        this.count = this.count + 1;
    },
    decre : function(){
        this.count = this.count - 1;
    }
  }
};
</script>

<template>
  <div class="shadow-sm">
    <h1>Event Count</h1>
    <p>Count: {{this.count}}</p>
    <button
      type="button"
      class="
        inline-block
        px-6
        py-2.5
        bg-green-500
        text-white
        font-medium
        text-xs
        leading-tight
        uppercase
        rounded
        shadow-md
        hover:bg-green-600 hover:shadow-lg
        focus:bg-green-600 focus:shadow-lg focus:outline-none focus:ring-0
        active:bg-green-700 active:shadow-lg
        transition
        duration-150
        ease-in-out
      "
      @click="this.incre" 
    >
      Increment
    </button>
    <button
      type="button"
      class="
        inline-block
        px-6
        py-2.5
        bg-red-600
        text-white
        font-medium
        text-xs
        leading-tight
        uppercase
        rounded
        shadow-md
        hover:bg-red-700 hover:shadow-lg
        focus:bg-red-700 focus:shadow-lg focus:outline-none focus:ring-0
        active:bg-red-800 active:shadow-lg
        transition
        duration-150
        ease-in-out
      "
      @click="decre"
    >
      Decrement
    </button>
  </div>
</template>

<style>
</style>