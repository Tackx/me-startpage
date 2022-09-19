<template>
  <div class="datetime">
    <span id="weekday">{{ weekday }},</span>
    <span id="date">{{ date }}</span>
    <span id="time">{{ time }}</span>
  </div>
</template>

<script lang="ts">
  import { defineComponent } from 'vue';

  export default defineComponent({
    data() {
      return {
        weekday: '',
        date: '',
        time: ''
      };
    },
    mounted() {
      this.setDate();
      this.setTime();
      setInterval(this.setTime, 1000);
    },
    methods: {
      setDate() {
        const today = new Date();
        const weekday = today.toLocaleDateString(undefined, { weekday: 'long' });
        const month = today.toLocaleDateString(undefined, { month: 'long' });
        const day = today.getDate();
        const year = today.getFullYear();
        this.weekday = weekday;
        this.date = day + ' ' + month + ' ' + year;
      },
      setTime() {
        const now = new Date();
        const hours = now.getHours() < 10 ? '0' + now.getHours() : now.getHours();
        const minutes = now.getMinutes() < 10 ? '0' + now.getMinutes() : now.getMinutes();
        this.time = hours + ':' + minutes;
      }
    }
  });
</script>

<style scoped>
  .datetime {
    /* position: flex;
    top: 0;
    left: 0;
    min-height: 100%; */
    width: 100%;
    color: var(--color-text-main);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 1.5em;
    background-color: var(--color-frame-background);
    border-radius: 20px;
    padding: 20px;
  }
  #weekday {
    font-size: 2em;
  }
  #date {
    font-size: 2em;
  }
  #time {
    font-size: 2em;
  }
</style>
