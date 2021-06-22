<template>
  <div id="header">
   <section class="stage">
<svg viewBox="0 0 160 160" width="160" height="160">
  <circle cx="80" cy="80" r="50" />
  <g transform=" matrix(0.866, -0.5, 0.25, 0.433, 80, 80)">
    <path d="M 0,70 A 65,70 0 0,0 65,0 5,5 0 0,1 75,0 75,70 0 0,1 0,70Z" fill="#FFF">
  <animateTransform attributeName="transform" type="rotate" from="360 0 0" to="0 0 0" dur="3s"
  repeatCount="indefinite" />
    </path>
  </g>
<path d="M 50,0 A 50,50 0 0,0 -50,0Z" transform="matrix(0.866, -0.5, 0.5, 0.866, 80, 80)" />
</svg>
</section>


    <div class="content">
      <div class="text">
        <h1>{{ msg }}</h1>
        <h2>DEVELOPPEUSE WEB ET WEB MOBILE ET CMS WORDPRESS</h2>
         <h2>Freelance</h2>
<!-- <p>
         Je travail principalement  avec des TPE/ PME, artisants, associations et créateurs.

        CMS, no-code, developpement front-end , back-end et intégation web. <br>
 </p> -->
      </div>
    </div>
    <div class="nav_middle">
      <router-link class="is-middle" to="/services">Mes services</router-link>
      <router-link to="/projets">Mes projets</router-link>
      <router-link to="/contact">Me contacter</router-link>
    </div>

<ul class="icons">
<li >
      <a
        href="../img/Cordelia guims.cv.CDC3.pdf"
        class="icon brands fa-cv"
        target="_blank"
      >
        <span class="label">CV</span></a
      >
    </li>
    <li>
      <a
        href="https://www.linkedin.com/in/cordelia-aurelie-guims-de-medeiros-10955a110/"
        class="icon brands fa-linkedin-f"
        target="_blank"
        ><span class="label">Linkedin</span></a
      >
    </li>
    <li>
      <a href="#" class="icon brands fa-instagram" target="_blank"
        ><span class="label">Agence</span></a
      >
    </li>
    <li>
      <a
        href="https://github.com/Cordelia013"
        class="icon brands fa-github"
        target="_blank"
        ><span class="label">GitHub</span></a
      >
    </li>
  </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
};

</script>

// <!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped lang="scss">

#header > * {
  // transition: opacity 0.325s ease-in-out;
  position: relative;
  // margin-top: 3.5rem;
}

#header {
  display: flex;
  justify-content: left;
  flex-direction: column;
  align-items: center;
  // transition: transform 0.325s ease-in-out, filter 0.325s ease-in-out,
  //   opacity 0.325s ease-in-out;
  background-image: radial-gradient(
    rgba(0, 0, 0, 0.25) 27%,
    rgba(0, 0, 0, 0) 60%
  );
  width: min-content;
  text-align: center;
}
// rond logo 3D
.stage {
  top:4rem;
  width: 16.5rem;
  height: 19.5rem;
  display: inline-block;
  margin: 20px;
  perspective: 1200px;
  perspective-origin: 50% 50%;
}
.logo .shadow {
  position: absolute;
  // width: 100%;
  // height: 100%;
  background: radial-gradient(circle at 50% 50%, rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.1) 40%,
  rgba(0, 0, 0, 0) 50%);
  transform: rotateX(90deg) translateZ(-150px);
  z-index: -1;
  }
  svg {
  position: fixed;
  bottom: 5%;
  height: 250px;
  right: 5%;
  width: 250px;
  }
#header .logo {
  display: block;
  background: black;
  background: radial-gradient(circle at 100px 100px, #5cabff, #000);
  width: 10.5rem;
  height: 10.5rem;
  line-height: 5.5rem;
  // border: solid 1px #ffffff;
  border-radius: 100%;
  // margin-top: 0;
}
#header .content {
  border-style: solid;
  border-color: #ffffff;
  border-top-width: 1px;
  border-bottom-width: 1px;
  max-width: 100%;
}
#header .content h3 {
  text-transform: uppercase;
  letter-spacing: 0.2rem;
  font-size: 0.8rem;
  line-height: 2;
  margin: 0 0 2em 0;
}
#header .text {
  transition-delay: 0.25s;
  padding: 2rem 3rem;
  max-height: 40rem;
  overflow: hidden;
}
h1 {
  font-size: 2.25rem;
  line-height: 1.3;
  letter-spacing: 0.5rem;
}
#header .nav_middle {
  display: flex;
  margin-bottom: 0;
  list-style: none;
  padding-left: 0px;
  border: solid 1px #ffffff;
  border-radius: 5px;
  filter: opacity(59%);
  -webkit-filter: opacity(69%);
   margin-top: 17px;
}
#header .nav_middle a {
  display: block;
  min-width: 7.8rem;
  height: 2.75rem;
  line-height: 2.75rem;
  padding: 0 1.25rem 0 1.45rem;
  text-transform: uppercase;
  letter-spacing: 0.2rem;
  font-size: 0.8rem;
  border-bottom: 0;
}
a.router-link-active.router-link-exact-active {
  border-left: 0;
  font-size: 16px;
}

#header .nav_middle a {
  border-radius: 3px;
  overflow: hidden;
  position: relative;
  font-size: 14px;
}

#header .nav_middle a::after,
#header .nav_middle a::before {
  content: " ";
  display: block;
  height: 0;
  position: absolute;
  width: 120%;
  z-index: 0;
}

#header .nav_middle a::before {
  background: rgba(200, 200, 255, 0.9);
  top: 50%;
  left: 0%;
  // -webkit-transition: all 200ms 125ms ease-in-out;
  // transition: all 200ms 125ms ease-in-out;
}

#header .nav_middle a:hover {
  border-radius: 12px;
  background: #4f4848;
  box-shadow: inset 6px 6px 7px #443e3e, inset -6px -6px 7px #5a5252;
}
#header .nav_middle a:hover::after {
  background: rgba(104, 101, 101, 0.1);
  bottom: -10%;
  height: 120%;
  position: relative;
  right: -10%;
}
.icon {
  text-decoration: none;
  border-bottom: none;
  border-bottom-color: currentcolor;
  position: relative;
}
ul.icons {
  cursor: default;
  list-style: none;
  padding-left: 17px;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  margin: 4rem;
}
ul.icons li {
  display: inline-block;
  padding: 0 1.5em 0 0;
}
ul.icons li a {
  border-radius: 100%;
  box-shadow: inset 0 0 0 1px #ffffff;
  display: inline-block;
  line-height: 4rem;
  text-align: center;
  padding: 5px;
  height: 4rem;
  width: 4rem;
}
a:hover {
  border-bottom-color: transparent;
}
ul.icons li a:hover {
  background-color: rgba(255, 255, 255, 0.13);
}
.fa-instagram {
  margin-left: 7rem;
}

// /* ###### Responsive 360px ###### */
 @media screen and (max-width: 360px) {
.nav_middle {
    display: block;
   }
.stage {
    top: 6rem;
    margin: 15px;
    height: 16.5rem;
     }
.stage > svg:nth-child(1) {
    top: -20%;
   }
#header .nav_middle{
    display: block;
    margin-top: 51px;
}
h1 {
    font-size: 1.8em;
    line-height: 1.3;
    letter-spacing: 0rem;
  }
.text>h2:nth-child(2) {
 width:55%;
 position:relative;
 left:24%;
}
#header .nav_middle{
 display:block;
 }
.fa-instagram{
 margin-left:0rem;
}
ul.icons li{
 padding: 0 0.8em 0 0;
}

 }
 /* ###### Responsive 480px ###### */

@media screen and (max-width: 480px) {
.stage{
    top:0;
  }
.text > p:nth-child(4) {
 display: flex;
 justify-content: center;
 align-items: center;
width: 19em;
margin-left: 2em;
padding: 2%;
margin-top: 3em;
}
#header .nav_middle{
    display: block;
  }
    }
/* ###### Responsive 736px ###### */
 @media screen and (max-width: 736px) {

}
/* ###### Responsive 736px ###### */
 @media screen and (max-width: 736px) {

}
@media screen and (max-width: 840px) {
    /* body,input,select,textarea {
     font-size:12pt
    } */
}
/* ###### Responsive 1680px ###### */
@media screen and (max-width: 1680px) {
}
</style>
