<template>
  <div class="links-wrapper">
    <a class="link" href="https://www.reddit.com"><mdicon size="64" name="reddit" /></a>
    <a class="link" href="https://www.youtube.com"><mdicon size="64" name="youtube" /></a>
    <a class="link" href="https://www.savla.dev"><mdicon size="64" name="satellite-variant" /></a>
    <a class="link" href="https://www.github.com"><mdicon size="64" name="github" /></a>
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
  .links-wrapper {
    /* position: flex;
      top: 0;
      left: 0;
      min-height: 100%; */
    width: 100%;
    color: var(--color-text-main);
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 4em;
    background-color: var(--color-frame-background);
    border-radius: 20px;
    padding: 20px;
  }
  .link,
  .link:visited {
    color: var(--color-text-main);
  }
  .link:hover,
  .link:active {
    color: rgb(138, 141, 145);
  }
</style>
