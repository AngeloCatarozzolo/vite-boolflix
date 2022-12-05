<script>
import { store } from "../store";
export default {
  name: "AppHeader",
  data() {
    return {
      store,
    };
  },
};
</script>

<template>
  <form @submit.prevent="$emit('performSearch')">
    <input
      type="text"
      placeholder="Inizia la ricerca..."
      v-model="store.textToSearch"
      required
    />
    <button type="submit">Cerca</button>
  </form>
</template>

<style lang="scss" scoped>

</style>