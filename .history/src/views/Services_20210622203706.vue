<template>
  <div class="body">
    <article id="services" class="active">
      <div class="modal-header">
        <h2 class="titre">Mes services</h2>
        <router-link to="/">X</router-link>
        <div id="section">
        <section class="gauche">
          h
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
  width: 50rem;
  height: 40rem;
  // max-width: 50%;
  background-color: rgba(27, 31, 34, 0.85);
  border-radius: 4px;
}

#section{
position: absolute;
// background-color: aqua;
display: flex;
top:20%;
height: 70vh;
width: 55vw;
}
.gauche{
  position: relative;

height: 70vh;
width: 50%;
background-color: white;
width: 50%;
}

.droite{

top:20%;
height: 70vh;
width: 50%;
  background-color: blue;
  width: 50%
}
</style>
