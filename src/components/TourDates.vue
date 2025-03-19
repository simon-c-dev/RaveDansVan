<script setup>
import { ref } from 'vue';

const concerts = ref([
  { date: '2023-11-01', state: 'CA', city: 'Los Angeles', venue: 'Hollywood Bowl' },
  { date: '2023-11-05', state: 'NV', city: 'Las Vegas', venue: 'MGM Grand' },
  { date: '2023-11-10', state: 'TX', city: 'Austin', venue: 'Austin City Limits' },
  { date: '2023-11-15', state: 'NY', city: 'New York', venue: 'Madison Square Garden' },
]);

const formatDate = (dateString) => {
  const date = new Date(dateString);
  const options = { year: 'numeric', month: 'short', day: '2-digit' };
  const formattedDate = date.toLocaleDateString('en-US', options).toUpperCase().replace(',', '').split(' ');
  return [formattedDate[0], formattedDate[1], formattedDate[2]];
};
</script>

<template>
  <div class="tour-dates-container text-center p-4">
    <h1 class="text-2xl mb-5">Tour Dates</h1>
    <div class="flex flex-col items-center">
      <div v-for="(concert, index) in concerts" :key="concert.date" class="tour-date w-full max-w-4xl relative">
        <div class="date-info">
          <div class="day">{{ formatDate(concert.date)[2] }}</div>
          <div class="month">{{ formatDate(concert.date)[0] }}</div>
          <div class="year">{{ formatDate(concert.date)[1] }}</div>
        </div>
        <div class="venue text-xs sm:text-l w-30">{{ concert.venue }}</div>
        <div class="location text-xs sm:text-l w-20">{{ concert.city }}, {{ concert.state }}</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.tour-dates-container {
  border-radius: 8px;
  padding: 16px;
}

.tour-date {
  display: flex;
  align-items: center;
  padding: 16px 0;
  border-bottom: 1px solid #e5e7eb;
}

.tour-date:last-child {
  border-bottom: none;
}

.date-info {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-right: 16px;
  font-weight: bold;
  color: #374151;
}

.date-info .day {
  font-size: 12px;
  color: #9ca3af;
}

.date-info .month,
.date-info .year {
  font-size: 20px;
  color: #1f2937;
}

.venue {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  text-align: center;
  color: #6b7280;
}

.location {
  margin-left: auto;
  color: #6b7280;
}
</style>