<template>
    <section id="pilates">
        <!-- <h2>La méthode Pilate</h2> -->
        <div class="bulle_one">
            <h3>Qu'est ce que le Pilates ?</h3>
            <p>C'est une méthode douce ( placement précis, mouvement lent, respiration profonde)
                qui vise à renforcer les chaînes musculaires profondes du corps et redonne de la mobilité à
                l'ensemble du corps.
                Tous les exercices sont observés, adaptés et corrigés afin que chacun puisse progresser
                rapidement en toute sécurité.
            </p>
            <p>
                <strong>Un mot sur JOSEPH PILATES</strong>
            </p>
            <p>
                La méthode Pilates porte le nom de son créateur, Joseph Pilates, gymnaste, boxeur et
                plongeur allemand qui vécut au début du XXe siècle. Selon lui, tout être humain naît avec un
                droit universel, le droit de rester en bonne santé. À partir de cette idée, il crée un
                répertoire complet de centaines de mouvements spécifiques pour permettre à la colonne
                vertébrale et aux articulations d’un adulte de s’assouplir. Pour lui, cela signifie parvenir
                à un développement harmonieux du corps, où l’équilibre règne entre le corps et les facultés
                mentales et spirituelles, et l’entretenir.
            </p>
            <p>
                "Après dix séances, vous sentirez la différence, après vingt séances, vous verrez la
                différence, après trente
                séances, vous aurez un corps tout neuf."
            </p>
            <p>
                C’est d’abord le monde de la danse (Martha Graham, Balanchine…) qui comprit l’impact de ses
                travaux sur le mouvement dansé. Joseph Pilates continua d’enseigner jusqu’à sa mort en 1967
                et laissa derrière lui quelques héritiers. Il fallut attendre que les stars hollywoodiennes
                découvrent cette technique dans les années 1990 pour que le grand public y ait enfin accès.
            </p>
        </div>
        <div class="bulle">
            <div class="bulle_content">
                <h3>Objectifs</h3>
                <ul>
                    <li>Développer la musculature profonde et amener le coprs dans un alignement idéal afin de
                        rectifier la posture.</li>
                    <li>Améliorer la force et la mobilité.</li>
                    <li>Augmenter l'énergie et restaurer les fonctions physiques.</li>
                    <li>Stimuler la conscience du corps.</li>
                </ul>
            </div>
            <div class="bulle_content">
                <h3>Bienfaits</h3>
                <ul>
                    <li>Agit à la fois sur le corps et l'esprit, et permet d'harmoniser la silhouette.</li>
                    <li>Diminue les douleurs.</li>
                    <li>Apporte une grande force intérieure, affine, assouplit.</li>
                    <li>Détend et améliore la qualité du souffle.</li>
                </ul>
            </div>
            <div class="bulle_content">
                <h3>Destiné à qui ?</h3>
                <ul>
                    <li>Aux sportifs ou non sportifs.</li>
                    <li>Aux personnes qui soufrent de stress, fatigues et raideurs.</li>
                    <li>Aux femmes enceintes ou qui viennent d'accoucher.</li>
                    <li>Aux personnes âgées, blessées ou en convalescence.</li>
                </ul>
            </div>
        </div>

            <App__carousel class="carousel" v-slot="{currentSlide}">
                <App__slide v-for="(slide, index) in carouselSlides" :key="index">
                    <div v-show="currentSlide === index + 1" class="slide_info">
                        <img :src="require(`../assets/${slide}.jpg`)" alt="">
                    </div>
                </App__slide>
            </App__carousel>


    </section>
</template>

<script>
import App__slide from '../components/App__slide.vue';
import App__carousel from '../components/App__carousel.vue';
export default {
    name: 'App__pilates',
    components: {
        App__carousel,
        App__slide,
    },
    setup() {
    const carouselSlides = ['carousel1', 'carousel2', 'carousel3', 'carousel4', 'carousel5', 'carousel6'];

    return { carouselSlides };
  }
    

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style language="scss" scoped>
#pilates {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
    margin: 1rem;
    color: var(--color-text-menu);
    border-radius: 3.1rem;
}

/* ==========  ========== */
.bulle_one {
    background: var(--color-primary);
    border-radius: 3rem;
    text-align: left;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
}
.bulle_one h3 {
    margin: 2rem;
}
.bulle_one p {
    margin: 2rem;
}
/* ==========  ========== */
.bulle {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.5rem;
    margin: 1rem;
}
.bulle_content {
    background: var(--color-secondary);
    border-radius: 3rem;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
}
.bulle_content h3 {
    margin: 2rem;
}
.bulle_content ul li {
    margin: 2rem;
    text-align: left;
}
/* ==========  ========== */

.carousel {
    position: relative;
    max-height: 50vh;
    height: 50vh;
    
}
.slide_info {
    position: absolute;
    width: 100%;
    max-height: 100%;
    height: 100%;
}
img {
    min-width: 100%;
    height: 100%;
    object-fit: cover;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
    border-radius: 3rem;
}
/* ================ TABLETTE ============ */
@media screen and (max-width: 1024px) {
.bulle {
    display: grid;
    grid-template-columns: 1fr;
    margin: 0;
}
.people_droite {
    margin-top: 0;
}
}

/* ================ PHONE ============ */
@media screen and (max-width: 600px) {
.carousel {
    position: relative;
    max-height: 25vh;
    height: 25vh;
    
}
.slide_info {
    position: absolute;
    width: 100%;
    max-height: 100%;
    height: 100%;
}
img {
    min-width: 100%;
    height: 100%;
    object-fit: cover;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
    border-radius: 3rem;
}
}
</style>