<template>
  <div id="app">
    <div class="sidebar"></div>
    <Header />
    <MovieList/>
  </div>
</template>

<script>
import axios from "axios";
import Header from "./components/Header";
import MovieList from "./components/MovieList";
export default {
  name: "app",
  components: {
    Header,
    MovieList
  },
  data() {
    return {
      movies: []
    };
  }
  
};
</script>

<style>
.sidebar {
  height: 25px;
  background: rgb(2, 136, 209);
}
</style>
