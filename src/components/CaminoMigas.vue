<template>
  <section id="camino-migas">
      <a class="inicio" href="#">  <fa icon="bars"></fa>  Todas las categorías </a> >
      <a class="inicio" href="#"> Home </a> >
      <a href="#">Smartphones y Telefonía </a> > 
      <a class="actual" href="#">Ver todos los Accesorios</a> 

  </section>
  <hr>
</template>

<script>
export default {

}
</script>

<style>
section#camino-migas {
    margin-left: 1rem;
    display:flex;
    flex-wrap: wrap;
    align-items: center;
 

}
section#camino-migas a, 
section#camino-migas a:hover, 
section#camino-migas a:visited{
    text-decoration: none;
    font-size: 0.7rem;
    margin-left: 1rem;
    margin-right: 1rem;
    color: #363636;
}
section#camino-migas a.actual {
    font-weight: 700;
}
section#camino-migas {
    margin-left: 0.7rem;
    color: #363636;
}
hr {
  border-color: rgb(46, 46, 46);
}
</style>
