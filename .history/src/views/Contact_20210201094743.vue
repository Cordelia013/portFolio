/* eslint-disable no-console */
<template>
  <div class="body">
     <div class="sect-proj">
    <h2>contact</h2>
<form action="" method="post">
      <label for="name">Nom ou Dénomination sociale </label>
      <input type="text" name="name" id="name" />

      <label for="name">Prenom </label>
      <input type="text" name="prenom" id="prenom" />

      <label for="name">Telephone </label>
      <input type="tel" name="tel" id="tel" />

      <label for="name">Email </label>
      <input type="email" name="mail" id="mail" />

      <ul class="actions">
        <li><button>Envoyer</button></li>
      </ul>
    </form>
  </div>
</template>

<script>
// export default {
//   data: () => {
//     return {
//       mailEnvoye: false,
//       professionnel: false,
//     };
//   },
//   methods: {
//     envoiFormulaire() {
//       console.log('envoi du form');
//       // alert('coincoin')
//       fetch('https://api.asciiparait.fr/contact.php')
//         .then(response => response.json())
//         .then(data () => {
//           // Afficher que l'on a bien envoyé le message
//         });
//       this.mailEnvoye = true;
//     },
//   },
// };

</script>

<style scoped lang="scss">
form {
  margin: 0 0 2rem 0;
}
body {
  display: flex;
  flex-wrap: wrap;
  width: calc(100% + 3rem);
  margin: -1.5rem 0 2rem -1.5rem;
}
#contact {
  transition: opacity 0.325s ease-in-out, transform 0.325s ease-in-out;
  padding: 4.5rem 2.5rem 1.5rem 2.5rem;
  position: relative;
  width: 40rem;
  max-width: 100%;
  background-color: rgba(27, 31, 34, 0.85);
  border-radius: 4px;
}
.sect-contact {
  width: calc(50% - 0.75rem);
  flex-grow: 0;
  flex-shrink: 0;
  padding: 1.5rem 0 0 1.5rem;
}
label {
  color: #ffffff;
  display: block;
  font-size: 0.8rem;
  font-weight: 300;
  letter-spacing: 0.2rem;
  line-height: 1.5;
  margin: 0 0 1rem 0;
  text-transform: uppercase;
}
* {
  text-align: left;
}
label {
  display: block;
  width: calc(100% - 42px);
}
ul.actions {
  display: flex;
}
ul.actions li {
  list-style-type: none;
}
ul.actions li > button {
  border: 0;
  padding: 10px 20px;
  font-weight: bold;
  background: #ddd;
}
ul.actions li > button.active {
  color: #fff;
  background: var(--color-active-button);
}
ul.actions li > button.inactive {
  color: #888;
  background:var( --color-hover-button);
}
ul.actions li > button:hover {
  cursor: pointer;
  background: var(--color-hover-button);
}
ul.actions li:first-child > button {
  border-radius: 8px 0 0 8px;
}
ul.actions li:last-child > button {
  border-radius: 0 8px 8px 0;
}
</style>
