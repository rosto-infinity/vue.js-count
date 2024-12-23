

 <template>
  <div class=" grid gap-4 justify-center items-center"> 
          <h1 class="text-7xl text-red-600 font-bold underline">
        Count 
        </h1>
        <button @click="increment" class="mt-5 px-7 py-4 bg-green-500 rounded-md text-3xl text-white" > increment = {{ count }}</button>
  </div>
</template>


  <script setup>
  import { ref } from 'vue'
  const count = ref(0);

  const increment = () => {
    count.value++;
  }
  
  </script>
