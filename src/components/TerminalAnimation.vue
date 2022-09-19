<template>
  <div class="terminal-wrapper">
    <img src="../assets/hdv.gif" />
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
  .terminal-wrapper {
    /* position: flex;
      top: 0;
      left: 0;
      min-height: 100%; */
    height: 100%;
    color: var(--color-text);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 1.5em;
    background-color: var(--color-frame-background);
    border-radius: 20px;
    /* padding: 20px; */
    max-width: 270px;
  }
  img {
    max-width: 100%;
    max-height: 100%;
  }
</style>
