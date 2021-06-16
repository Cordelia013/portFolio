<template>
  <div id="header">
   <figure class="logo">
 </figure>
    <div class="content">
      <div class="text">
        <h1>{{ msg }}</h1>
        <h2>DEVELOPPEUSE WEB ET WEB MOBILE ET CMS WORDPRESS</h2>
         <h2>Freelance</h2>
          <p>
         Je travail principalement  avec des TPE/ PME, artisants, associations et créateurs.

        CMS, no-code, developpement front-end , back-end et intégation web. <br>
        <!-- Vous pouvez trouver ici certaines mes differentes
        <router-link to="/projets"> réalisations </router-link>. -->

      </p>
      </div>
    </div>
    <div class="nav_middle">
      <!-- <router-link to="/">Home</router-link> | -->
      <!-- <router-link to="/About">A propos</router-link> -->
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
  margin-top: 3.5rem;
}

#header > *::before {
  content: " ";
  display: block;
  position: absolute;
  bottom: calc(-3.5rem - 2px);
  left: calc(50% - 4px);
  width: 1px;
  height: calc(2rem + 24px);
  background: #ffffff;
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
  max-width: 100%;
  text-align: center;
}

#header .logo {
  width: 5.5rem;
  height: 5.5rem;
  line-height: 5.5rem;
  border: solid 1px #ffffff;
  border-radius: 100%;
  margin-top: 0;
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
  // transition: max-height 0.75s ease, padding 0.75s ease,
  //   opacity 0.325s ease-in-out;
  transition-delay: 0.25s;
  padding: 3rem 2rem;
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
  -webkit-filter: opacity(59%);
  -moz-filter: opacity(59%);
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
  height: 4rem;
  width: 4rem;
}
a:hover {
  border-bottom-color: transparent;
}
ul.icons li a:hover {
  background-color: rgba(255, 255, 255, 0.075);
}
.fa-instagram {
  margin-left: 7rem;
}
</style>
