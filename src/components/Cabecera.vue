<template>
  <section id="cabecera">
      <div class="container top flex_item_centrado flex_row">
      <!--  <img src="../assets/logo01.png" alt="Logo de la empresa"> -->
        <h4>Recuerda, ahora envíos gratis a partir de 50€ - Ver condiciones</h4>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style>
.top{ 
  background: black;
    z-index:999;
    padding:0.1rem;
    color: white;
}

 .flex_row{
      display: flex;
      flex-direction: row;
    }

    .flex_col{
      display: flex;
      flex-direction: column;
      
    }
    .flex_item_centrado{
      align-items: center;
      align-content: stretch;
      justify-content: center;
    }


section#cabecera img {
    margin: 1rem;
}

</style>
