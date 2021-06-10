<template>
  <div class="body">
    <article id="projets" style="" class="active">
      <div class="modal-header">
        <h2 class="titre">Mes projets</h2>
        <router-link to="/">X</router-link>
      </div>

      <div class="grid-container">
        <!-- Boutton de controle filtrage -->
        <div id="myBtnContainer">

           <button
        v-for="tab in tabs"
        v-bind:key="tab"
        v-bind:class="['tab-button', { active: currentTab === tab }]"
        v-on:click="currentTab = tab"
      >
        {{ tab }}
      </button>

      <component v-bind:is="currentTabComponent" class="tab"></component>
    </div>
<!--
          <button  class="btn active" onclick="filterSelection('all')">
            Show all
          </button>

          <button  class="btn" onclick="filterSelection('front')">Front</button>

          <button  class="btn" onclick="filterSelection('fullStack')">
            full stack
          </button>

          <button  class="btn" onclick="filterSelection('cms')">Cms</button> -->

      <!-- projet filtrer, par cathégorie -->

        <!--   -->
        <!-- <section class="card card1">
          <h4>calendrier html/css</h4>
          <a href="https://naughty-lamport-ded569.netlify.app">
          <img src="/img/tableauHTML_CSS.png" alt="calendrier html/css"/>
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem,
            ipsa.
          </p>
        </section> -->
        <!--
        <section class="card card2">
          <h4>Projets Actutu</h4>
          <br>
          <a href="https://friendly-nightingale-653f36.netlify.app">
            <img src="/img/actutu.png " alt="Projets Actutu" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt,
            veritatis.
          </p>
        </section> -->

        <!-- <section class="card card3">
          <h4>Projets Nucleotics</h4>
          <a href="https://gallant-bartik-bf5396.netlify.app">
            <img src="/img/nucleotic.png " alt="Projets Nucleotics" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim,
            distinctio.
          </p>
        </section> -->

        <!-- <section class="card card4">
          <h4>Projets egghead.io</h4>
          <a href="https://hungry-ptolemy-f05569.netlify.app">
            <img src="/img/egghead.io.png " alt="Projets egghead.io" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!
          </p>
        </section> -->
        <!-- <section class="card card5">
          <h4>Projets café Florette</h4>
          <a href="https://hungry-ptolemy-f05569.netlify.app">
            <img src="/img/egghead.io.png " alt="Projets egghead.io" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!
          </p>
        </section> -->
        <!-- <section class="card card6">
          <h4>agence immobilière</h4>
          <a href="https://hungry-ptolemy-f05569.netlify.app">
            <img src="/img/egghead.io.png " alt="Projets egghead.io" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!
          </p>
        </section> -->
        <!-- <section class="card card7">
          <h4> projet Immersive colab</h4>
          <a href="https://hungry-ptolemy-f05569.netlify.app">
            <img src="/img/egghead.io.png " alt="Projets egghead.io" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!
          </p>
        </section> -->
        <!-- <section class="card card8">
          <h4>Projet poney fringeant</h4>
          <a href="https://hungry-ptolemy-f05569.netlify.app">
            <img src="/img/egghead.io.png " alt="Projets egghead.io" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!
          </p> -->
        <!-- </section>
         <section class="card card8">
          <h4>projet portFolio</h4>
          <a href="https://hungry-ptolemy-f05569.netlify.app">
            <img src="/img/egghead.io.png " alt="Projets egghead.io" />
          </a>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!
          </p>
        </section> -->
      </div>
    </article>
  </div>
</template>

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
  color: #ffffff;
  width: 100px;
  line-height: 100px;
  text-align: center;
  margin: 2px;
  display: none;
}

.show {
  display: block;
}

.container {
  margin-top: 20px;
  overflow: hidden;
}

/* Style the buttons */
.btn {
  width: 5rem;
  border: none;
  outline: none;
  padding: 8px 10px;
  background-color: #f1f1f1;
  cursor: pointer;
}

.btn:hover {
  background-color: #ddd;
}

.btn.active {
  background-color: #666;
  color: white;
}
</style>
