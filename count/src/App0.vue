<template>
  <div class=" grid gap-4 justify-center items-center">
    <h1 class="text-7xl text-center text-red-600 font-bold underline">
      Count
    </h1>


    <div class="text-center text-6xl">{{ count }}</div>
    <div class="s">

      <button @click="increment" class="mt-5 mr-4 px-7 py-4 bg-green-500 rounded-md text-3xl text-white"> increment
      </button>

      <span class="" v-if="count > 0">
        <button @click="decrement" class="mt-5 px-7 py-4 bg-green-500 rounded-md text-3xl text-white"> Decrement
        </button>
      </span>
      <span  v-else>
        <button class="disabled:opacity-0 disabled:cursor-none mt-5 px-7 py-4 bg-green-100 rounded-md text-3xl text-white"> Decrement
        </button>
      </span>

    </div>
   
  </div>

</template>


<script setup>
import { ref } from 'vue'
let count = ref(0);

console.log(count);


const increment = () => {
  count.value++;
}
const decrement = () => {
  count.value--;
}

</script>
