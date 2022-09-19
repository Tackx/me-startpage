<template>
  <div class="notification">
    <h1>Classified TOP SECRET</h1>
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
  .notification {
    color: var(--color-text-error);
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    background-color: var(--color-frame-background-error);
    border-radius: 7px;
    padding: 1em;
  }
  h1 {
    font-size: 2em;
  }
</style>
