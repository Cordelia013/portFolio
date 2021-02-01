<template>
<div class="body">
  <article id="about"  class="active">
    <h2 class="titre">A propos</h2>
    <img src="img/pic03.jpg" alt="image">
    <p>
      Je m’appelle Cordelia GUIMS. Je suis une futur développeuse FullStack basé
      à Marseille, en FRANCE, je suis très passionnée et dédiée à mon travail.
      <br/><br />
      Je souhaite continuer mon apprentissage en poursuivant par une formation
      en alternance en vue d'être Conceptrice et développeuse d’application web.
      vous trouver quelques de mes projets professionnels mais également
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

.main {
  
  display: block;
  position: relative;
  left: 0;
  opacity: 0.5;
  top: 0;
  width: 100%;
  height: 100%;
  margin: 2.5rem 0;
}


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

</style>
