<template>
  <div class="body">
    <article id="services" class="active">
      <div class="modal-header">
        <h2 class="titre">Mes services</h2>
        <router-link to="/">X</router-link>
        <div id="section">
        <section class="gauche">

        </section>
        <section class="droite">

     </section>
     </div>
      </div>
    </article>
  </div>
</template>

<style lang="scss">
#services {

  transition: opacity 0.325s ease-in-out, transform 0.325s ease-in-out;
  padding: 4.5rem 2.5rem 1.5rem 2.5rem;
  position: relative;
  width: 40rem;
  max-width: 100%;
  background-color: rgba(27, 31, 34, 0.85);
  border-radius: 4px;
}

#section{
position: absolute;
background-color: aqua;
height: 20vh;
width: 20vw;
}
.gauche{

background-color: white;
width: 50%;
}

.droite{

  background-color: blue;
  width: 50%
}
</style>
