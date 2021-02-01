<template>
  <div class="body">
    <article id="projets" style="" class="active">
        <div class="modal-header ">
          <router-link to="/">X</router-link>

      </div>
      <h2 class="titre">Mes projets</h2>

      <div class="grid-container">

        <section class="card card1">
          <h4>calendrier html/css</h4>
          <a href="https://naughty-lamport-ded569.netlify.app">
          <img src="/img/tableauHTML_CSS.png" alt="calendrier html/css"/>
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem,
            ipsa.
          </p>
        </section>

        <section class="card card2">
          <h4>Projets Actutu</h4>
          <a href="https://friendly-nightingale-653f36.netlify.app">
            <img src=" " alt="Projets Actutu" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt,
            veritatis.
          </p>
        </section>

        <section class="card card3">
          <h4>Projets Nucleotics</h4>
          <a href="https://gallant-bartik-bf5396.netlify.app">
            <img src=" " alt="Projets Nucleotics" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim,
            distinctio.
          </p>
        </section>

        <section class="card card4">
          <h4>Projets egghead.io</h4>
          <a href="https://hungry-ptolemy-f05569.netlify.app">
            <img src=" " alt="Projets egghead.io" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!
          </p>
        </section>
      </div>
    </article>
  </div>
</template>

<style lang="scss" scoped>

router-link {
color: black;
}
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1fr;
  gap: 16px 21px;
  grid-template-areas:
    ". . ."
    ". . ."
    ". . ."
    ". . .";
}
section{

  border: 1px solid black;

  >h4, p{
    text-align: center;
  }

> a{

  > img{
    width: 100%;
  }
}

}

</style>
