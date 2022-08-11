<template>
  <footer>
    <p>©Le Corps Pilates - Tous droits réservés</p>
  </footer>
</template>

<script>
export default {
  name: 'App__footer',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
footer {
  background: var(--color-primary);
  color: var(--color-text-menu);
  padding-top: 5rem;
  padding-bottom: 8rem;
  border-radius: 3rem 3rem 0 0;
  margin: 1rem;
}
</style>