<template>
  <div class="container">
    <div class="row mt-5 justify-content-left">
      <div class="card card-custom mx-2 mb-3">
        <div class="card" style="width: 18rem;">
          <img class="card-img-top" src="" alt="Imagem de capa do card" />
          <div class="card-body">
            <h5 class="card-title">{{movie.popularity}} </h5>
            <p
              class="card-text"
            >Um exemplo de texto rápido para construir o título do card e fazer preencher o conteúdo do card.</p>
            <a href="#" class="btn btn-primary">Visitar</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MovieItem",
  props : ['movie'],
  data() {
    return {
      movie1: this.movie
    }
  }
}
</script>

<style>
.card-deck {
  padding-left: 150px;
}
.container {
  margin-left: 140px;
}
/* .card-deck {
  height: 20px;
  width: 1200px;
}
.card-body {
  height: 250px;
} */
</style>