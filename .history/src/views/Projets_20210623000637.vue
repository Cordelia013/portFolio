<template>
  <div class="body">
    <article id="projets" style="" class="active">
      <div class="modal-header">
        <h2 class="titre">Mes projets</h2>
        <router-link to="/">X</router-link>
      </div>

      <div class="grid-container">
        <section class="card card1">
          <h4>calendrier html/css</h4>
          <a href="https://naughty-lamport-ded569.netlify.app">
            <img src="/img/tableauHTML_CSS.png" alt="calendrier html/css" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem,
            ipsa.
          </p>
        </section>

        <section class="card card2">
          <h4>Projets Actutu</h4>
          <br />
          <a href="https://friendly-nightingale-653f36.netlify.app">
            <img src="/img/actutu.png " alt="Projets Actutu" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt,
            veritatis.
          </p>
        </section>

        <section class="card card3">
          <h4>Projets Nucleotics</h4>
          <a href="https://gallant-bartik-bf5396.netlify.app">
            <img src="/img/nucleotic.png " alt="Projets Nucleotics" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim,
            distinctio.
          </p>
        </section>
      </div>
    </article>
  </div>

  <!-- <div class="body">
    <article id="projets" style="" class="active">
      <div class="modal-header">
        <h2 class="titre">Mes projets</h2>
        <router-link to="/">X</router-link>
      </div>

      <div class="grid-container">
        <div id="myBtnContainer">
          <button class="btn" >Tous</button>
            <button class="btn">Tous</button>
              <button class="btn">Tous</button>
                <button class="btn">Tous</button>

        </div>
        <div id="myContainerProject">
            card
        </div>
      </div>
    </article>
  </div> -->
</template>

<script>
// import all from '../components/filterProject/all.vue';
// import cms from '../components/filterProject/cms.vue';
// import frontend from '../components/filterProject/frontend.vue';
// import fullStack from '../components/filterProject/fullStack.vue';
// import mobile from '../components/filterProject/mobile.vue';
</script>

<style lang="scss" scoped>
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
section {
  border: 1px solid black;

  > h4,
  p {
    text-align: center;
  }

  > a {
    > img {
      width: 100%;
      height: 7rem;
    }
  }
}
// boutton filtre

#myBtnContainer {
  display: flex;
}
.filterDiv {
  background-color: #2196f3;
  // color: #ffffff;
  width: 100px;
  line-height: 100px;
  text-align: center;
  margin: 2px;
  display: none;
}

// .show {
//   display: block;
// }

// .container {
//   margin-top: 20px;
//   overflow: hidden;
// }

.card:hover {
  background: #a298a1;
  color: #213550;
}
// card
.card {
  padding: 30px;
  border-radius: 21px;
  background: linear-gradient(145deg, #29292c, #303134);
  box-shadow: 15px 15px 39px #212224, -15px -15px 39px #393a3e;
}

</style>
