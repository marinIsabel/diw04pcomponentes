<template>
  <section id="producto-datos">
      <h1>Mobile Tech Cristal Templado 9H Full Glue 2.5D Borde Negro para Realme 8/ 8 PRO</h1>
      <h2>750,69€ <span class="iva">sin IVA: 620,41€</span></h2>
      <div class="center">
         <img class="estrellas" src="../assets/estrellas.png" alt="Logo de la empresa">
        <span class="iva"> 6 Opiniones | Review</span>

      </div>
<br>
      <div class="wrapper">
          <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
          <input class="cantidad" type="text" name="name" :value="contador">
          <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
      </div>
      <br>
      <button class="boton"><fa icon="cart-arrow-down"></fa> AÑADIR CARRITO</button>
      <br> <br>
      <p>
        Protector de vidrio templado con gran sensibilidad y transparencia. Resistente a impactos, golpes y caídas. Sus 0,3 mm de grosor aseguran el perfecto funcionamiento de la pantalla táctil ofreciendo una gran protección... 
      <a class="actual" href="#">Ver más</a> 
      </p> 
      <video width="480px" controls="controls" preload="auto" autoplay>
          <source src="../assets/video.mp4" type="video/mp4" />
          <source src="C../assets/video.ogv" type="video/ogg" />
          Si tu navegador no soporta HTML puedes descargarte video pinchando en los siguientes enlaces.
          <a href="../assets/video.mp4">Formato MP4</a>
          <a href="../assets/video.ogv">Formato OGG</a>
      </video>
  </section> 
</template>

<script>
export default {
  Name: 'ProductoDatos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }


}
</script>

<style scoped>

a{
  color: #ff7f34;
}

 .estrellas{
  width: 70px;
}
.center{
    
    display:flex;
    flex-wrap: wrap;
    align-items: center;
 

}

section#producto-datos {
  flex: 1 1 18rem;
}
h1 {
  font-size: 1.2rem;
}
h2 {
  font-size:1.9rem;
  line-height: 0.1rem;
  color: #ff7f34;
}
span.iva {
  font-size:1rem;
  font-weight: normal;
  
  color: #282828
}
.wrapper {
  height: 2rem;
  display: flex;
}

.cantidad {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  border: 1px solid #d8d8d8;
}
.btn {
  border: 1px solid #d8d8d8;
  width: 1.8rem;
  
}
button:focus, input:focus {
  outline: 0;
}

</style>
