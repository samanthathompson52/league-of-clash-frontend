<template src="./app.html"></template>

<style>
  @import '@/css/base.css';
  @import '@/css/app.css';
</style>

<script>
import HomePage from './views/HomePage/HomePage.vue';
import AboutPage from './views/HomePage/HomePage.vue';
import axios from 'axios';

export default {
  name: 'App',
  components: {
    HomePage,
    AboutPage
  },
  created() {
    axios.get(`http://localhost:8080/helloWorld`)
    .then(response => {
      // JSON responses are automatically parsed.
      this.posts = response.data
      console.log(response);
    })
    .catch(e => {
      this.errors.push(e)
    })
  }
}
</script>


