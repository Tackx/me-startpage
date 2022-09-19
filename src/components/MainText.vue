<template>
  <div class="mainText">
    <h1>Alliance Military Personnel Database ***N7***</h1>
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
  .mainText {
    width: 100%;
    color: var(--color-text-main);
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin-top: 3em;
  }
  h1 {
    font-size: 2em;
  }
</style>
