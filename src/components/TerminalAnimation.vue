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
    width: 100%;
    height: 100%;
    color: var(--color-text);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 1.5em;
    background-color: var(--color-frame-background);
    border-radius: 20px;
    padding: 20px;
  }
  #searchBar {
    font-size: 2em;
    border-radius: 10px;
    background-color: var(--color-frame-background);
    caret-color: var(--color-text);
    color: var(--color-text);
    border: none;
    padding: 10px;
  }
  #searchBar:focus {
    outline: none;
  }
  #searchButton {
    color: var(--color-text);
    font-size: 2em;
    background-color: var(--color-frame-background);
    border-radius: 10px;
    margin-left: 0.5em;
    padding-left: 0.2em;
    padding-right: 0.2em;
    cursor: pointer;
    border: none;
    width: 2em;
    height: 100%;
  }
  #searchButton:hover,
  #searchButton:active {
    color: rgb(138, 141, 145);
  }
</style>
