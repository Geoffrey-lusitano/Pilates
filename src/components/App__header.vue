<template>
    <div class="container header__container">
        <div class="logo">
            <img src="../assets/logo.png" alt="logo" />
        </div>
        <h1>Les valeurs :
            <span class="typed__text"></span>
        </h1>


    </div>
</template>

<script>
export default {
  name: 'App__header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
    width: var(--container-width-lg);
    margin: 0 auto;
}

img {
    display: block;
    width: 100%;
    object-fit: cover;
}

h1 {
    font-size:4rem;
    
}
</style>
