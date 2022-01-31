<template>
  <section id="producto-imagen">
      <div class="img-big"> 
          <img v-bind:src="fotos[0]" alt="Portátil Huawei MateBoot X">
      </div>
        <div class="img-mini">
          <a @click="cambiarFoto(1)"><img  v-bind:src="fotos[1]" alt="Mobile Tech Cristal Templado frontal"></a>
          <a @click="cambiarFoto(2)"><img  v-bind:src="fotos[2]" alt="Mobile Tech Cristal Templado lateral izquierdo"></a>
          <a @click="cambiarFoto(3)"><img  v-bind:src="fotos[3]" alt="Mobile Tech Cristal Templado lateral derecho"></a>
          <a @click="cambiarFoto(4)"><img  v-bind:src="fotos[4]" alt="Mobile Tech Cristal Templado ladeado"></a>
        </div>
      </section>    
</template>

<script>
export default {
    Name: 'ProductoImagen',
    data () {
        return {
            fotos: [
                require ('../assets/e1.jpeg'),
                require ('../assets/e1.jpeg'),
                require ('../assets/e2.jpeg'),
                require ('../assets/e3.jpeg'),
                require ('../assets/e4.jpeg')]
        }
    },
    methods: {
        cambiarFoto(id) {
            this.fotos[0] = this.fotos[id]
        }
    }

}
</script>

<style escoped>
#producto-imagen {
    border-radius: 25px;
    padding: 1rem;
    margin: 1rem;
    flex: 0 1 50%;
}
.img-mini {
    display: flex;
    justify-content: start;
    align-items: flex-start;
}
.img-mini img {
    width: 70px;
    margin-right: 0.3rem;
    border:2px solid #d8d8d8;
    
}
</style>
