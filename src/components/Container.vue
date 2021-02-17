<template>
  <div class="w-11/12 mx-auto" :class="moreClass">
    <slot />
  </div>
</template>

<script>
export default {
  props: {
    moreClass: String,
  },
};
</script>
