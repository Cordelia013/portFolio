/* eslint-disable no-console */
<template>
  <div class="body">
    <article id="contact" style="" class="active">
      <div class="modal-header">
        <h2 class="titre">Contactez moi</h2>
        <router-link to="/">X</router-link>
      </div>
      <!-- mise en place du formulaire -->
       <div class="container">

  <div class="columns">
    <div class="column is-6 has-text-left is-family-code">
      <br>
      <h1 class="has-text-weight-bold is-size-3">
        Email:
      </h1>
      <a class="is-size-4" href="mailto:cordeliaguims@yahoo.com">
        <fa :icon="['fas', 'envelope']"></fa>
        contact@cordeliaguims.com
      </a>
      <br>
      <br>

      <h1 class="has-text-weight-bold is-size-3">
        Github:
      </h1>
      <a class="is-size-4" href="https://github.com/Cordelia013">
        <fa :icon="['fab', 'github']"></fa>
        Cordelia013
      </a>
      <br>
      <br>
    </div>

    <div class="column is-6 has-text-left">
      <br>
      <div class="field">
        <div class="control has-icons-left">
          <input class="input" type="text" placeholder="Nom">
          <span class="icon is-left">
            <fa :icon="['fas', 'user']"></fa>
          </span>
        </div>
      </div>

      <div class="field">
        <div class="control has-icons-left">
          <input class="input" type="email" placeholder="Email">
          <span class="icon is-left">
            <fa :icon="['fas', 'envelope']"></fa>
          </span>
        </div>
      </div>

      <div class="field">
        <div class="control">
          <textarea class="textarea" placeholder="message"></textarea>
        </div>
      </div>

      <button class="button ">Envoyer</button>
    </div>

  </div>
    </div>
    </article>
  </div>
</template>

<script>

</script>

<style scoped lang="scss">
button {
  border: 1px solid #fff;
  padding: 10px 20px;
  font-weight: bold;
  background:transparent;
  cursor
}
</style>

// form {
//   margin: 0 0 2rem 0;
// }
// body {
//   display: flex;
//   flex-wrap: wrap;
//   width: calc(100% + 3rem);
//   margin: -1.5rem 0 2rem -1.5rem;
// }
// #contact {
//   width: 40rem;
//  }
// .sect-contact {
//   width: calc(50% - 0.75rem);
//   flex-grow: 0;
//   flex-shrink: 0;
//   padding: 1.5rem 0 0 1.5rem;
// }
// label {
//   display: block;
//   font-size: 0.8rem;
//   font-weight: 300;
//   letter-spacing: 0.2rem;
//   line-height: 1.5;
//   margin: 1rem 0 0.6rem 0;
//   text-transform: uppercase;
// }
// * {
//   text-align: left;
// }
// label {
//   display: block;
//   width: calc(100% - 42px);
// }
// ul.actions {
//   display: flex;
// }
// ul.actions li {
//   list-style-type: none;
// }
// ul.actions li > button {
//   border: 0;
//   padding: 10px 20px;
//   font-weight: bold;
//   background: #ddd;
// }
