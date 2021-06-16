<template>
  <div class="body">
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


        </div>
      </div>
    </article>
  </div>

</template>

<script>
// import all from '../components/filterProject/all.vue';
// import cms from '../components/filterProject/cms.vue';
// import frontend from '../components/filterProject/frontend.vue';
// import fullStack from '../components/filterProject/fullStack.vue';
// import mobile from '../components/filterProject/mobile.vue';

new vue({
   el: '#app',
  data: {
    title: ' ',
    strongTag:'<strong>Important !</strong>'
  },
  methods:{
  // on creer une fonction reverse title pour inverser le nom du title. On creer donc une fonction pour qu'elle soit exécutée.
  	reverseTitle: function(){
    	this.title= this.title.split('').reverse().join('')
      //on recupere le nom dans title = ensuite on change le contenu, .split('') va permttre de faire un array de tous les caractères , oon fait un reverse: pour inverser les caractère , puis un .join('') pour les recoller.
  }
  
  })


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
  // background-color: #f1f1f1;
  cursor: pointer;
}

.btn:hover {
  background:#A298A1;
  color:#213550;
}

// .btn.active {
//   background-color: #666;
//   color: rgb(87, 5, 163);
// }
</style>
