<template>
  <Header />
  <img alt="Vue logo" src="./assets/logo.png" class="mx-auto" />
  <Counter />
</template>

<script>
import Header from "@/components/Header.vue";
// import Counter from "@/components/CounterSetup.vue";
import Counter from "@/components/CounterComposition.vue";

export default {
  name: "App",
  components: {
    Header,
    Counter,
  },
};
</script>

<style src="./styles/globals.css" />
