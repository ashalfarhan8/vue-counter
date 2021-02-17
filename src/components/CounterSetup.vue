<template>
  <div class="max-w-md h-64 flex flex-col items-center justify-center mx-auto">
    <h2>Using Setup</h2>
    <div class="text-5xl font-mono">
      <h1>{{ count }}</h1>
    </div>
    <div class="w-full grid grid-cols-2 mt-12 text-5xl">
      <button
        @click="handleIncrement"
        class="bg-blue-500 flex items-center justify-center py-2 rounded-2xl focus:outline-none"
      >
        +
      </button>
      <button
        @click="handleDecrement"
        class="bg-red-500 flex items-center justify-center py-2 rounded-2xl focus:outline-none"
      >
        -
      </button>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const count = ref(0);
    const handleIncrement = () => count.value++;
    const handleDecrement = () => count.value--;

    return {
      count,
      handleIncrement,
      handleDecrement,
    };
  },
};
</script>
