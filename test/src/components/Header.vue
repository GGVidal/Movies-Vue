<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand text-primary" href="#">Navbar</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item">
        <a class="nav-link" href="#">Lancamentos</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Populares</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Melhores avaliados</a>
      </li>
    </ul>
  </div>
</nav>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style>
.navbar-brand {
  color: rgb(2, 136, 209);
  padding-left: 140px;
  font-size: 40px;
}
.nav-link {
  color: rgb(229, 230, 231);
  font-size: 25px;
  padding-right: 40px;
}
</style>