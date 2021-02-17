<template>
  <header class="px-4 py-4">
    <Container>
      <div class="flex justify-center items-center">
        <h1 class="text-3xl font-bold">
          This is a counter app using
          <span class="uppercase text-green-600">vue</span> for my exercise
        </h1>
      </div>
    </Container>
  </header>
</template>

<script>
import Container from "./Container";

export default {
  name: "Header",
  components: {
    Container,
  },
};
</script>
