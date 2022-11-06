<script>
export default {
  name: "TextOne",
  props: {
    name: { type: String, required: true },
    age: { type: Number, required: true },
    designation: { type: String, required: true },
  },
};
</script>

<template>
  <h2 class="text-2xl">TextOne component: send props</h2>
  <div class="grid grid-rows-4 grid-flow-col gap-4">
      <ul class="list-none hover:list-disc">
        <li class="list-decimal">Name: {{name}}</li>
        <li class="list-decimal">age: {{age}}</li>
        <li class="list-decimal">designation: {{designation}}</li>
      </ul>
    </div>
</template>

<style>
</style>