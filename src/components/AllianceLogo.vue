<template>
  <div class="logo-wrapper">
    <img src="../assets/me.png" alt="Systems Alliance Logo" />
  </div>
</template>

<script lang="ts">
  import { defineComponent } from 'vue';

  export default defineComponent({
    data() {
      return {};
    },
    // mounted() {},
    methods: {}
  });
</script>

<style scoped>
  .logo-wrapper {
    /* position: flex;
      top: 0;
      left: 0;
      min-height: 100%; */
    /* width: 100%; */
    color: var(--color-text);
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    background-color: var(--color-frame-background);
    max-width: 270px;
  }
  img {
    /* width: 35%;
    height: 35%; */
    max-width: 100%;
    max-height: 100%;
  }
</style>
