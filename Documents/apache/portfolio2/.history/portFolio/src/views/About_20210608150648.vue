<template>
  <div class="body">
    <article id="about" class="active">
      <div class="modal-header">
        <h2 class="titre">A propos</h2>
        <router-link to="/">X</router-link>
      </div>
      <section class="main">
<img src="img/pic03.jpg" alt="image" />
      </section>
      <section class=>
      <p>
        Je m’appelle Cordelia GUIMS. Je suis developpeuse web ,
        basée sur marseille.
        <br /><br />
        2021, je suis Freelance en tant que conceptrice de site web.
        Je travail principalement  avec des TPE/ PME, artisants, associations et créateurs.

        CMS, no-code, developpement front-end , back-end et intégation web. <br>
        Vous pouvez trouver ici certaines mes differentes
        <router-link to="/projets"> réalisations </router-link>.

      </p>
      </section>
    </article>
  </div>
</template>

<style scoped lang="scss">
article {
  display: block;
}

#about {
  transition: opacity 0.325s ease-in-out, transform 0.325s ease-in-out;
  padding: 2.5rem 2.5rem 1.5rem 2.5rem;
  position: relative;
  width: 100%;
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
  width: 100%;
  // width: max-content;
  text-align: center;
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
