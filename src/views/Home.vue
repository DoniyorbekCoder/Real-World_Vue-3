<template>
  <h1>Events For Good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'

export default {
  name: 'Home',
  components: {
    EventCard
  },
  data() {
    return {
      events: [
        {
          id: 5928101,
          category: 'animal welfare',
          title: 'cat adoption day',
          description: 'Find your new alone',
          location: 'Meow Town',
          date: 'January 28, 2022',
          time: '12:00',
          petsAllowed: true,
          organizer: 'D Coder'
        },
        {
          id: 5928102,
          category: 'animal welfare 1',
          title: 'cat adoption day 1',
          description: 'Find your new alone 1',
          location: 'Meow Town 1',
          date: 'January 28, 2022 1',
          time: '12:00 1',
          petsAllowed: true,
          organizer: 'D Coder 1'
        },
        {
          id: 5928103,
          category: 'animal welfare 2',
          title: 'cat adoption day 2',
          description: 'Find your new alone 2',
          location: 'Meow Town 2',
          date: 'January 28, 2022 2',
          time: '12:00 2',
          petsAllowed: true,
          organizer: 'D Coder 2'
        }
      ]
    }
  }
}
</script>
<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
