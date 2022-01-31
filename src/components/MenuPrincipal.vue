<template>
<section id="menu-principal">
    <div class="container">
        
        <img src="../assets/logo01.png" alt="Logo de la empresa">
     
    <nav>
        <ul>
            <li><a href="#">INICIO</a></li>
            <li><a href="#">MOVIL</a></li>
            <li><a href="#">CARGADORES</a></li>
            <li><a href="#">FUNDAS</a></li>
            <li><a href="#">AURICULARES</a></li>
            <li><a href="#">OTROS</a></li>
          
        </ul>
    </nav>
    <div class=grupo>
        <a class="registro" href="#"> <fa icon="user-edit"></fa>REGISTRO</a>
        
        <a class="login" href="#"> <fa icon="user"></fa> INICIAR SESIÓN</a>
    </div>
    
</div>
</section>
<hr>
  
</template>

<script>
export default {

}
</script>

<style>
hr {
  border-color: rgb(46, 46, 46);
}
section#cabecera img {
    margin: 1rem;
}
section#menu-principal {
    background: #fafafa;
    z-index:999;
    padding:0.7rem;
}

section#menu-principal .container {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
  justify-content: center;
    flex-direction: row;
    justify-content: space-between;
}

section#menu-principal .container nav ul {
    display:flex;
    flex-wrap: wrap;
    flex-direction: row;
    list-style: none;
    padding: 0;
    margin:0rem 0.7rem;
}
section#menu-principal .container nav ul li a, .registro:hover, .login:hover{
    background-color: #fafafa;
    text-decoration: none;
    color:rgb(107, 107, 107);
    font-weight: 700;
    padding-left: 1rem;
    padding-right: 1rem;
}
section#menu-principal .container nav ul li a:hover,.active {

    background-color:orange;
    text-decoration: none;
    border-radius: 4px;
        border-color: none;
        padding: 0.5rem 2rem;
        border: none;
        margin-left: 0rem;
}

section#menu-principal a:hover,.registro, .login {

        background: #FEB100;
        border-radius: 4px;
        border-color: none;
        padding: 0.5rem 2rem;
        border: none;
        margin-left: 1rem;
        text-decoration: none;
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

</style>
