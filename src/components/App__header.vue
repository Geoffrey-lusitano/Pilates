<template>
    <div class="container header__container">
        <div class="logo">
            <img src="../assets/logo.png" alt="logo" />
        </div>
        <h1>
            <span class="typed__text"> :{{ typeValue }}</span>
        </h1>


    </div>
</template>

<script>
export default {
  name: 'App__header',
  data: () => {
    return {
        typeValue: '',
        typeStatus: false,
        typeArray: ['Concentration', 'Centrage', 'Respiration', 'Isolation', 'Précision', 'Fluidité'],
        typingSpeed: 50,
        erasingSpeed: 50,
        newTextDelay: 2000,
        typeArrayIndex: 0,
        charIndex: 0,
    }
  },
  methods: {
    typeText() {
        if(this.charIndex < this.typeArray[this.typeArrayIndex].length) {
            if(!this.typeStatus)
                this.typeStatus = true;

            this.typeValue += this.typeArray[this.typeArrayIndex].charAt(this.charIndex);
            this.charIndex += 1;

            setTimeout(this.typeText, this.typingSpeed);
        } else {
            this.typeStatus = false;
            setTimeout(this.eraseText, this.newTextDelay);
        }
    },
    eraseText() {
        if(this.charIndex > 0) {
            if(!this.typeStatus)
                this.typeStatus = true;
            this.typeValue = this.typeArray[this.typeArrayIndex].substring(0, this.charIndex - 1);
            this.charIndex -= 1;

            setTimeout(this.eraseText, this.erasingSpeed);
        } else {
            this.typeStatus = false;
            this.typeArrayIndex += 1;
            if(this.typeArrayIndex >= this.typeArray.length)
                this.typeArrayIndex = 0;
            
            setTimeout(this.typeText, this.typingSpeed + 1000);
        }
    },
  },
  created() {
    setTimeout(this.typeText, this.newTextDelay + 200);
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
.typed__text {
    color: var(--color-primary);
    font-weight: 500;
}
/* ================ TABLETTE ============ */
@media screen and (min-width: 1025px) {
img {
    max-width: 1000px;
    margin: 0 auto;
}
}


/* ================ TABLETTE ============ */
@media screen and (max-width: 1024px) {

}

/* ================ PHONE ============ */
@media screen and (max-width: 600px) {
.typed__text {
    font-size: 1rem;
}


}
</style>
