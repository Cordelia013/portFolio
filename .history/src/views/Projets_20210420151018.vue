<template>
  <div class="body">
    <article id="projets" style="" class="active">
      <div class="modal-header">
        <h2 class="titre">Mes projets</h2>
        <router-link to="/">X</router-link>
      </div>

      <div class="grid-container">
          <div id="myBtnContainer">
            
             <all id="all"/>
            <frontend id="frontend"/>
            <fullStack id="fullStack"/>
            <mobile id="mobile"/>
            <cms id="cms"/>
    </div>
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

      </div>
    </article>
  </div>
</template>

<script>
import all from '../components/filterProject/all'
import cms from '../components/filterProject/cms'
import frontend from '../components/filterProject/frontend'
import fullStack from '../components/filterProject/fullStack'
import mobile from '../components/filterProject/mobile'

export default {
  components: 
  { all, cms, frontend, fullStack, mobile }
}
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
  width: 6rem;
  border: none;
  outline: none;
  padding: 8px 5px;
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
