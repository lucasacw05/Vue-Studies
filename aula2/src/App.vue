<template>

  <ul>
    <li v-for="event in events" :key="event.id">
      <EventItem :event="event"/>
    </li>
  </ul>

  
</template>

<!--SCRIPT BEGINNING-->
<script>
import EventItem from './components/Event-item.vue';

export default {
  name: 'App',
  components: {
    EventItem,
  },

  data() {
    return {
      events: eventList,
    }
  }

}

// eslint-disable-next-line no-unused-vars
const eventList = [
   {
     id: 1,
     name: "Graduation",
     details: "wooohoo!!!",
     date: "2020-09-25",
     background: "#F34949",
   },
   {
     id: 22,
     name: "Holidays",
     details: "wooohoo!!!",
     date: "2021-12-30",
     background: "#f9f970",
   },
   {
     id: 3,
     name: "HolidayYYYY",
     details: "Get me outta here!",
     date: "2020-09-12",
     background: "#7AD3F0",
   },
   {
     id: 4,
     name: "Birthday",
     details: "My birthday party",
     date: "2020-10-02",
     background: "#F07AEC",
   },
   {
     id: 5,
     name: "Christmas",
     details: "ho ho ho",
     date: "2020-03-5",
     background: "#EB9A0F",
   },
   {
     id: 6,
     name: "Conference Talk",
     details: "dont flop",
     date: "2021-02-28",
     background: "#68EE94",
   },
 ];
</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  max-width: 600px;
  margin: 0 auto;
}

ul {
  padding: 0;
}

li {
  list-style: none;
  cursor: pointer
}



</style>
