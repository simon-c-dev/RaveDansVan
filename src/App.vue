<script setup>
import AppTopBar from "./components/AppTopBar.vue";
import TourDates from "./components/TourDates.vue";
import TourDatesTimeline from "./components/TourDatesTimeline.vue";
</script>

<template>
  <AppTopBar/>
    <div class="bg-surface-50 dark:bg-surface-950 min-h-screen p-8 flex flex-col gap-6">
      <TourDates/>
      <TourDatesTimeline/>
    </div>
</template>
<style>
@font-face {
  font-family: saira;
  src: url('src/assets/fonts/SairaStencilOne-Regular.ttf');
}
</style>
