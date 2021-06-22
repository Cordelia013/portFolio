<template>
  <div class="body">
    <article id="services" class="active">
      <div class="modal-header">
        <h2 class="titre">mes services</h2>
        <router-link to="/">X</router-link>
        <div id="section">
          <section class="gauche">
            <h3>Mes compétences</h3>
              <h3>Mes <LOGICIEL>
              <OUTIL></OUTIL></h3>
            <button class="fill">HTML5</button>
            <button class="pulse">CC3</button>
            <button class="close">JAVASCRIPT</button>
            <button class="raise">SASS</button>
            <button class="up">REACTJS</button>
            <button class="up">VUEJS</button>
          </section>
          <section class="droite">
            <h3>Mes technos FRONT</h3>
            <button class="fill">HTML5</button>
            <button class="pulse">CC3</button>
            <button class="close">JAVASCRIPT</button>
            <button class="raise">SASS</button>
            <button class="up">REACTJS</button>
            <button class="up">VUEJS</button>

            <h3>Mes technos BACK</h3>
            <button class="slide">PHP</button>
            <button class="offset">LARAVEL</button>
            <button class="offset">NODEJS</button>
            <button class="offset">MARIAdb/MYSQL</button>

            <h3>Mes technos CMS/NOCODE</h3>
            <button class="offset">WORDPRESS</button>
            <button class="offset">PRESTASHOP</button>
            <button class="offset">DRUPAL</button>
            <button class="offset">SQL</button>
            <button class="offset">ADALO</button>

            <h3>Mes technos MOBILE</h3>
            <button class="offset">SWIFT 4</button>
            <button class="offset">FLUTTER</button>


            <h3>Mes technos EN PLUS</h3>
            <button class="offset">LINUX_UBUNTU</button>
            <button class="offset">APACHE</button>
            <button class="offset">FLUTTER</button>
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
h3 {
  padding: 20px;
  text-align: center;
  color: black;
  font-family: "Bad Script", cursive;
  font-weight: 700;
}
// section copetence
// Animate the size, inside
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

// Animating from the bottom
.up:hover,
.up:focus {
  box-shadow: inset 0 -3.25em 0 0 var(--hover);
}

// And from the left
.slide:hover,
.slide:focus {
  box-shadow: inset 6.5em 0 0 0 var(--hover);
}

// Multiple shadows, one on the outside, another on the inside
.offset {
  box-shadow: 0.3em 0.3em 0 0 var(--color), inset 0.3em 0.3em 0 0 var(--color);

  &:hover,
  &:focus {
    box-shadow: 0 0 0 0 var(--hover), inset 6em 3.5em 0 0 var(--hover);
  }
}

//=== Set button colors
// If you wonder why use Sass vars or CSS custom properties...
// Make a map with the class names and matching colors
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

//=== Pen styling, ignore
body {
  color: #fff;
  background: hsl(227, 10%, 10%);
  font: 300 1em "Fira Sans", sans-serif;

  // Center everything ever
  justify-content: center;
  align-content: center;
  align-items: center;
  text-align: center;
  min-height: 100vh;
  display: flex;
}

// Basic button styles
button {
  background: none;
  border: 2px solid;
  font: inherit;
  line-height: 1;
  margin: 0.5em;
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
