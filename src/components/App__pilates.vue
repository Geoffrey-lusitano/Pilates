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
        <div class="bulle_img">
            <img src="../assets/carousel1.jpg" alt="">

        </div>
    </section>
</template>

<script>
export default {
    name: 'App__pilates',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#pilates {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
    margin: 1rem;
    color: var(--color-text-menu);
    border: 1px solid var(--color-primary);
    border-radius: 3.1rem;
}

/* ==========  ========== */
.bulle_one {
    background: var(--color-primary);
    border-radius: 3rem;
    text-align: left;
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
}
.bulle_content h3 {
    margin: 2rem;
}
.bulle_content ul li {
    margin: 2rem;
    text-align: left;
}
/* ==========  ========== */
.bulle_img {

}
img {
    width: 100%;
    max-height: 700px;
    border-radius: 3rem;
    margin: 0 auto;
    margin-bottom: -1rem;
    object-fit: cover;
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

}
</style>