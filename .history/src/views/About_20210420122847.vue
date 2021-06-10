<template>

<div class="body">
  <article id="about"  class="active">
    <div class="modal-header ">
          <h2 class="titre">A propos</h2>
          <router-link to="/">X</router-link>

      </div>
    <img src="img/pic03.jpg" alt="image">
    <p>
      Je m’appelle Cordelia GUIMS. Je suis eune developpeur se web junior, basée sur marseille
      <br/><br />
      Je souhaite continuer mon apprentissage en poursuivant par une formation
      en alternance en vue d'être Conceptrice et développeuse d’application web.
      vous trouver quelques de mes projets professionnels mais également

      J'ai menée divers projets en conception et developpement web.
      Je suis à la recherche d'un poste en alternance (CDD ou CDI), qui me permettrai de faire évoluer mes compétences.
      Etre Conceptrice et développeuse d’application web, c'est pouvoir allié mes compétence en management, relation client 
      au competence technique que j'ai acquis lors de 

      <router-link to="/projets">des réalisations personnels</router-link>.
    </p>
    <p>
      J'ai travailler dans divers millieux , notamment : administratif, bancaire
      et sociale et associative.
    </p>
  </article>
  </div>
</template>

<style scoped lang="scss">

article{
  display: block;
}

#about   {
  transition: opacity 0.325s ease-in-out, transform 0.325s ease-in-out;
  padding: 4.5rem 2.5rem 1.5rem 2.5rem;
  position: relative;
  width: 40rem;
  max-width: 100%;
  background-color: rgba(27, 31, 34, 0.85);
  border-radius: 4px;
}

#about article.active {
  transform: translateY(0);
  opacity: 1;
}

h2 {
  border-bottom: solid 1px #ffffff;
  width: max-content;
  padding-bottom: 0.5rem;
  margin: 0 0 2rem 0;
  font-size: 1.5rem;
  line-height: 1.4;
  letter-spacing: 0.5rem;

}
// #about > img:nth-child(2) {
// border-radius: 4px;
// border: 0;
// position: relative;
// display: block;
// margin: 2.5rem 0;
// }
.main {
  // pointer-events: none;
  // background-image: url(".");
  // background-color: rgba(19, 21, 25, 0.5);
  // border-radius: 4px;
  // content: "";
  display: block;
  position: relative;
  left: 0;
  opacity: 0.5;
  top: 0;
  width: 100%;
  height: 100%;
  margin: 2.5rem 0;
}

// #about > img:nth-child(2) {
//     background-image: url("../assets/img/bg.jpg");
//   border-radius: 4px;
//   display: block;
// }
p {
  margin: 0 0 2rem 0;
}
a {
  transition: color 0.2s ease-in-out, background-color 0.2s ease-in-out,
    border-bottom-color 0.2s ease-in-out;
  border-bottom: dotted 1px rgba(255, 255, 255, 0.5);
  text-decoration: none;
  color: inherit;
}
// #about article .close {
//     display: block;
//     position: absolute;
//     top: 0;
//     right: 0;
//     width: 4rem;
//     height: 4rem;
//     cursor: pointer;
//     text-indent: 4rem;
//     overflow: hidden;
//     white-space: nowrap;
// }
// #about article .close::before {

//     content: '';
//     display: block;
//     position: absolute;
//     top: 0.75rem;
//     left: 0.75rem;
//     width: 2.5rem;
//     height: 2.5rem;
//     border-radius: 100%;
//     background-position: center;
//     // background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' width='20px' height='20px' viewBox='0 0 20 20' zoomAndPan='disable'%3E%3Cstyle%3Eline %7B stroke: %23ffffff%3B stroke-width: 1%3B %7D%3C/style%3E%3Cline x1='2' y1='2' x2='18' y2='18' /%3E%3Cline x1='18' y1='2' x2='2' y2='18' /%3E%3C/svg%3E");
//     background-size: 20px 20px;
//     background-repeat: no-repeat;
// }
</style>
