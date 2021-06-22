<template>
  <div class="body">
    <router-view />
  </div>
</template>

<style lang="scss">

* {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}

*,
*::before,
*::after {
  box-sizing: content-box;
  font: inherit;
}

a {
  transition: color 0.15s ease-in-out, border-color 0.15s ease-in-out;
  color: #ffffff;
  text-decoration: none;
  border-bottom: dotted 1px;
}
body {
  display: flex;
  background: url("/img/bg.jpg" );
  box-shadow: 0 0 0.2em 0 rgba(0, 0, 0, 0.15);
  color: #ffffff;
  // width: 100vw;
  font-family: "open sans", sans-serif;
  font-weight: 300;
  font-size: 1rem;
  line-height: 1.65;
}
body,
input,
select,
textarea {
  color: #ffffff;
  font-family: "Source Sans Pro", sans-serif;
  font-weight: 300;
  font-size: 1rem;
  line-height: 1.65;
}
input[type="text"],
input[type="password"],
input[type="email"],
input[type="tel"],
select,
textarea {

  appearance: none;
  -moz-transition: border-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out,
    background-color 0.2s ease-in-out;
  -webkit-transition: border-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out,
    background-color 0.2s ease-in-out;
  -ms-transition: border-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out,
    background-color 0.2s ease-in-out;
  transition: border-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out,
    background-color 0.2s ease-in-out;
  background-color: transparent;
  border-radius: 4px;
  border: solid 1px #ffffff;
  color: inherit;
  display: block;
  outline: 0;
  padding: 0 1rem;
  text-decoration: none;
  width: 100%;
}
input[type="text"],
input[type="password"],
input[type="email"],
select {
  height: 2.75rem;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  color: #ffffff;
  font-weight: 600;
  line-height: 1.5;
  margin: 0 0 1rem 0;
  text-transform: uppercase;
  letter-spacing: 0.2rem;
}
h1.titre,
h2.titre,
h3.titre,
h4.titre,
h5.titre,
h6.titre {
  border-bottom: solid 1px #ffffff;
  width: -moz-max-content;
  width: -webkit-max-content;
  width: -ms-max-content;
  width: max-content;
  padding-bottom: 0.5rem;
  margin: 0 0 2rem 0;
  width: 100rem;
  // width: max-content;
  text-align: center;
  font-size: 1.5rem;
  line-height: 1.4;
  letter-spacing: 0.5rem;
}

// #projets, #contact{

// transition: opacity 0.325s ease-in-out, transform 0.325s ease-in-out;
// padding: 4.5rem 2.5rem 1.5rem 2.5rem;
// position: relative;
// width: 40rem;
// max-width: 100%;
// background-color: rgba(27, 31, 34, 0.85);
// border-radius: 4px;
// }
#about,
#contact,
#projets,
#services {
  transition: opacity 0.125s ease-in-out, transform 1.325s ease-in-out;
  padding: 4.5rem 2.5rem 1.5rem 2.5rem;
  position: relative;
  //  max-width: 100%;
  background-color: rgba(20, 21, 22, 0.85);
  box-shadow: 12px 12px 24px #191c20, -12px -12px 24px #353e45;
  border-radius: 4px;

  > img {
width: 100%;
}
}

.modal-header{
  display: flex;
justify-content: space-between;

   > a {
 color: #a7b9d1;
 font-weight:700;
 font-size: 1.4rem;
}
}
#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  min-height: 100vh;
  width: 100vw;
  // z-index: 3;
}

#app::before {
  content: "";
  display: block;
}
</style>
