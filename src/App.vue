<script setup lang="ts">
  import AllianceLogo from './components/AllianceLogo.vue';
  import MainText from './components/MainText.vue';
  import ClassifiedNotification from './components/ClassifiedNotification.vue';
  import TerminalAnimation from './components/TerminalAnimation.vue';
  import DefaultButton from './components/DefaultButton.vue';
  import DateTime from './components/DateTime.vue';
  import LinksBar from './components/LinksBar.vue';
</script>

<template>
  <div class="wrapper">
    <MainText />
    <ClassifiedNotification />
    <div class="items">
      <div class="row">
        <TerminalAnimation />
        <DefaultButton text="Connect to database" />
      </div>
      <AllianceLogo />
    </div>
    <DateTime />
    <LinksBar />
  </div>
</template>

<style scoped>
  .wrapper {
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 100%;
    justify-content: top;
    align-items: center;
    gap: 13em;
  }
  .items {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 1em;
  }
  .row {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 1em;
    height: 100%;
  }
</style>
