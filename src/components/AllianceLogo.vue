<template>
  <div class="links-wrapper">
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
  .links-wrapper {
    /* position: flex;
      top: 0;
      left: 0;
      min-height: 100%; */
    width: 100%;
    color: var(--color-text);
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
    color: white;
  }
  .link:hover,
  .link:active {
    color: rgb(138, 141, 145);
  }
</style>
