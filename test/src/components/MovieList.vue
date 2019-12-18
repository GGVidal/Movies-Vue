<template>
  <div class="movieList">
    <div class="title">
      <h1>Lista de Filmes</h1>
      <input type="text" name="search" id="ip1" placeholder="Buscar por nome do filme">
    </div>
    <MovieItem v-bind:movie="movies"/>
  </div>

</template>

<script>
import MovieItem from './MovieItem';
import axios from 'axios';
export default {
  name: "MovieList",
  components: {
    MovieItem
  },
  data() {
    return {
      movies: []
    }
  },
  created() {
      axios.get("https://api.themoviedb.org/3/movie/now_playing", {
        params: {
          'api_key': '216c669ac3afc192884e527269ef74f1'
        }
      }).then((res) => {
        this.movies = res.data.results[0]
      })
    }
}
</script>

<style>
.movieList {
  background: rgb(238, 238, 238);
  padding-top: 20px;
  height: 500px;
}
.movieList .title {
  display: flex;
}
.movieList h1 {
  color: rgb(97, 97, 97);
  padding: 0px 650px 0px 150px;
}
#ip1 {
    border-radius: 25px;
    border: 2px solid rgb(2, 136,209);
    padding: 20px;
    width: 250px;
    height: 15px;
    outline-width: 0;
}

</style>