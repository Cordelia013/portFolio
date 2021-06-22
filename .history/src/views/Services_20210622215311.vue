<template>
  <div class="body">
    <article id="services" class="active">
      <div class="modal-header">
        <h2 class="titre">mes compétences</h2>
        <router-link to="/">X</router-link>
        <div id="section">
          <section class="gauche">
            <h3>Mes LOGICIELS/OUTILS</h3>

            <button class="fill">VSCODE</button>
            <button class="offset">XCODE</button>
            <button class="close">CANVA</button>
            <button class="raise">PHOTOSHOP</button>
            <button class="fill">DISCORD/ZOOM/SLACK</button>
            <button class="up">TRELLO</button>
            <button class="offset">MARVEL</button>
            <button class="raise">FIGMA</button>
            <button class="close">GSUITE</button>

            <h3>Mes technos MOBILE</h3>
            <button class="offset">SWIFT 4</button>
            <button class="raise">FLUTTER</button>
               <button class="pulse">REACT NATIVE</button>

            <h3>Mes technos EN PLUS</h3>
            <button class="offset">LINUX_UBUNTU</button>
            <button class="fill">APACHE</button>
               <button class="pulse">WORDPRESS</button>

          </section>
          <section class="droite">
            <h3>Mes technos FRONT</h3>

            <button class="fill">HTML5</button>
            <button class="pulse">CC3</button>
            <button class="close">JAVASCRIPT</button>
            <button class="raise">SASS</button>
            <button class="up">REACTJS</button>
            <button class="raise">VUEJS</button>

            <h3>Mes technos BACK</h3>
            <button class="slide">PHP</button>
            <button class="offset">LARAVEL</button>
            <button class="fill">NODEJS</button>
            <button class="raise">MARIAdb/MYSQL</button>

            <h3>Mes technos CMS/NOCODE</h3>
            <button class="pulse">WORDPRESS</button>
            <button class="up">PRESTASHOP</button>
            <button class="close">DRUPAL</button>
            <button class="offset">SQL</button>
            <button class="pulse">ADALO</button>
          </section>
        </div>
      </div>
    </article>
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Bad+Script&display=swap");
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
  // background-color: white;
  width: 50%;
}

.droite {
  top: 20%;
  height: 70vh;
  width: 50%;
  // background-color: blue;
  width: 50%;
}
h3 {
  padding: 9px;
  margin: 20px 0px;
  text-align: center;
  font-family: "Bad Script", cursive;
  font-weight: 700;
}
// section copetence

.fill:hover,
.fill:focus {
  box-shadow: inset 0 0 0 2em var(--hover);
}

// Animate the size, outside
.pulse:hover,
.pulse:focus {
  animation: pulse 1s;
  box-shadow: 0 0 0 2em rgba(#fff, 0);
}

@keyframes pulse {
  0% {
    box-shadow: 0 0 0 0 var(--hover);
  }
}

// Stack multiple shadows, one from the left, the other from the right
.close:hover,
.close:focus {
  box-shadow: inset -3.5em 0 0 0 var(--hover), inset 3.5em 0 0 0 var(--hover);
}

// Size can also be negative; see how it's smaller than the element
.raise:hover,
.raise:focus {
  box-shadow: 0 0.5em 0.5em -0.4em var(--hover);
  transform: translateY(-0.25em);
}

.up:hover,
.up:focus {
  box-shadow: inset 0 -3.25em 0 0 var(--hover);
}

.slide:hover,
.slide:focus {
  box-shadow: inset 6.5em 0 0 0 var(--hover);
}

.offset {
  box-shadow: 0.3em 0.2em 0 0 var(--color), inset 0.1em 0.2em 0 0 var(--color);

  &:hover,
  &:focus {
    box-shadow: 0 0 0 0 var(--hover), inset 6em 3.5em 0 0 var(--hover);
  }
}

$colors: (
  fill: #a972cb,
  pulse: #ef6eae,
  close: #ff7f82,
  raise: #ffa260,
  up: #e4cb58,
  slide: #8fc866,
  offset: #19bc8b,
);

@each $button, $color in $colors {
  .#{$button} {
    --color: #{$color};
    --hover: #{adjust-hue($color, 45deg)};
  }
}

button {
  color: var(--color);
  transition: 0.25s;

  &:hover,
  &:focus {
    border-color: var(--hover);
    color: #fff;
  }
}

body {
  justify-content: center;
  align-content: center;
  align-items: center;
  text-align: center;
  min-height: 100vh;
  display: flex;
}

button {
  background: none;
  border: 2px solid;
  font: inherit;
  line-height: 1;
  margin: 0.26em;
  padding: 0.5em;
}

h1 {
  font-weight: 400;
}
code {
  color: #e4cb58;
  font: inherit;
}
</style>
