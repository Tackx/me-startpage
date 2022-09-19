<template>
  <button v-text="text"></button>
</template>

<script lang="ts">
  import { defineComponent } from 'vue';

  export default defineComponent({
    data() {
      return {};
    },
    props: {
      text: String
    },
    // mounted() {},
    methods: {}
  });
</script>

<style scoped>
  button {
    font-family: ME;
    color: var(--color-text-main);
    font-size: 1em;
    background-color: var(--color-frame-background-button);
    border-radius: 10px;
    padding: 0.2em;
    cursor: pointer;
    border: 10px solid var(--color-text-main);
    width: 20em;
  }
  button:hover,
  button:active {
    color: rgb(138, 141, 145);
  }
</style>
