<template>
  <div class="body">
    <article id="services" class="active">
      <div class="modal-header">
        <h2 class="titre">mes services</h2>
        <router-link to="/">X</router-link>
        <div id="section">
          <section class="gauche">
            <h3>Mes compétences</h3>
          </section>
          <section class="droite">
            <h3>Mes technos </h3>
            <img src="./img" alt="html/css">
              <img src="" alt="html/css">
                <img src="" alt="html/css">
                  <img src="" alt="html/css">
                    <img src="" alt="html/css">
                      <img src="" alt="html/css">
                        <img src="" alt="html/css">
                          <img src="" alt="html/css">
                            <img src="" alt="html/css">
          </section>
        </div>
      </div>
    </article>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Bad+Script&display=swap');
#services {
  transition: opacity 0.325s ease-in-out, transform 0.325s ease-in-out;
  padding: 4.5rem 2.5rem 1.5rem 2.5rem;
  width: 50rem;
  height: 40rem;
  // max-width: 50%;
  background-color: rgba(27, 31, 34, 0.85);
  border-radius: 4px;
}

#section {
  position: absolute;

  display: flex;
  top: 20%;
  height: 70vh;
  width: 55vw;
}

.gauche {
  position: relative;
  height: 70vh;
  width: 50%;
  background-color: white;
  width: 50%;
}

.droite {
  top: 20%;
  height: 70vh;
  width: 50%;
  background-color: blue;
  width: 50%;
}
h3{
  padding: 20px;
  text-align: center;
  color: black;
  font-family:'Bad Script', cursive;
  font-weight: 700;
}
</style>
