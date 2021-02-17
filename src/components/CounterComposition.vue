<template>
  <div class="max-w-md h-64 flex flex-col items-center justify-center mx-auto">
    <h2>Using Composition API</h2>
    <h3>{{ isOdd }}</h3>
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
export default {
  name: "Using Composition",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    handleIncrement() {
      console.log("handleIncrement Run");
      this.count = this.count + 1;
    },
    handleDecrement() {
      console.log("handleDecrement Run");
      this.count = this.count - 1;
    },
  },
  computed: {
    isOdd() {
      return this.count % 2 === 0
        ? "This number is Even"
        : "This number is Odd";
    },
  },
  watch: () => {
    console.log("value changed", this.count);
  },
};
</script>
