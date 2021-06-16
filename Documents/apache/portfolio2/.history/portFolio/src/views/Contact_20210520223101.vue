/* eslint-disable no-console */
<template>
  <div class="body">
    <article id="contact" style="" class="active">
      <div class="modal-header">
        <h2 class="titre">Me contacter</h2>
        <router-link to="/">X</router-link>
      </div>
      <!-- mise en place du formulaire -->
      <div class="sect-proj">
        <form action="form.php" method="post" id="formContact">
          <label for="name">denomination sociale</label>
          <input v-model="entreprise" type="text" name="denomination" />

          <label for="name">Nom</label>
          <input v-model="nom" type="text" name="nom" />

          <label for="name">Prenom </label>
          <input v-model="Prenom" type="text" name="prenom" />

          <label for="name">Telephone </label>
          <input v-model="tel" type="tel" name="tel" />

          <label for="name">Email </label>
          <input v-model="email" type="email" name="email" />

          <div>
            <label class="label" for="textarea">Message with Counter</label>
            <textarea
              class="message"
              name="textarea"
              id="textarea"
              required=""
              v-model="message.text"
              :maxlength="message.maxlength"
            ></textarea>
            <span class="counter"
              >{{ message.text.length }} / {{ message.maxlength }}</span
            >
          </div>

          <ul class="actions">
            <input type="submit" value="envoyer" @click="vald" />
          </ul>
        </form>
      </div>
    </article>
  </div>
</template>

<script>
export default {
  name: 'form',

  prop: {
    errors: [],
    entreprise: undefined,
    nom: undefined,
    prenom: undefined,
    tel: Number,
    email: undefined,
  },
  methods: {
    vald(e) {
      e.preventDefault();
      if (
      (this.entreprise || (this.nom && this.prenom)) 
      && this.tel 
        && this.email
      ) {
        return true;
      }

      this.errors = [];

      if ((!this.nom && !this.prenom) || !this.entreprise) {
        this.errors.push("merci d'ajouter votre nom ou dénomination sociale.");
      }
      if (!this.tel) {
        this.errors.push('contact required.');
      }
      if (!this.email) {
        this.errors.push('email required.');
      }
      return true;
    },
  },
};
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
  background: var(--color-hover-button);
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
