<template>
    <section id="about">
        <!-- <h2>Présentation</h2> -->
        <div class="people_gauche">
            <h2>Professeur</h2>
            <h3>Marie Noëlle Dumortier</h3>
            <ul>
                <li>Certifiée Pilates depuis 2017</li>
                <br>
                <li>Matwork I. II. III</li>
                <br>
                <li>Adaptation :</li>
                <li>- Femme enceinte</li>
                <li>- Sénior</li>
                <li>- Rose Pilates</li>
                <li>- Post-thérapie</li>
                <br>
                <li>Brevet d'État Sportif</li>
                <br>
                <li>Diplômée d'État de Professeur de danse Classique</li>
                <br>
                <li>Directrice d'une École de danse de 2006 à 2012 à Orange</li>
                <br>
            </ul>
        </div>
        <div class="photo">
            <img src="../assets/mnd.jpg" alt="Marie-Noel Dumortier">
        </div>
        <div class="people_droite">
            <p>
                J'ai découvert la danse Classique à l'âge de 9 ans et j'ai tout de suite été passionnée par cet
                univers.
            </p>
            <p>
                Très vite l'envie d'enseigner est devenue évident pour moi, j'ai donc obtenu un diplôme d'État
                en 1992 et j'ai eu la joie de diriger une école de danse à Orange dans le Vaucluse.
            </p>
            <p>
                Durant mon parcours, je me suis toujours intéressée aux différentes techniques qui contribuaient
                à améliorer la qualité du mouvement et une plus grande conscience du corps.
            </p>
            <p>
                En 2012 j'ai donné une nouvelle orientation à ma vie et me suis intéressée à la méthode Pilates
                qui était en parfaite harmonie entre mon travail acquis dans la danse et le désir de retrouver
                une activité qui respecte l'anatomie et la physiologie du corps.
            </p>
            <p>
                Aujourd'hui, j'enseigne cette technique à Grabels, Prades-Le-Lez, et à Montferrier-sur-lez.
            </p>
        </div>
    </section>
</template>

<script>
export default {
    name: 'App__about',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#about {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.5rem;
    margin: 1rem;
}
/********************************                         ******************************/
.people_gauche {
    background: var(--color-primary);
    color: var(--color-text-menu);
    border-radius: 0 3rem 0 3rem ;
    height: min-content;
    text-align: left;
box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
}
.people_gauche h2,h3 {
    margin-top: 2rem;
    margin-bottom: 1rem;
    margin-left: 1.5rem;
}
.people_gauche h4 {
    margin-top: 1rem;
    margin-bottom: 1rem;
    margin-left: 1.5rem;
}
.people_gauche ul {
    margin: 1.5rem;
}
/************* *******************/
img {
    max-width: 100%;
    border-radius: 3rem;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
}
/********** **************/
.people_droite {
    background: var(--color-secondary);
    color: var(--color-text-sombre);
    border-radius: 3rem 0 3rem 0;
    height: min-content;
    text-align: left;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
}
.people_droite p {
    margin: 1.5rem;
}

/* ================ TABLETTE ============ */
@media screen and (max-width: 1024px) {
#about {
    display: grid;
    grid-template-columns: 1fr;
    gap: 0rem;
    margin: 1rem;
}
.people_gauche {
    border-radius: 3rem 3rem 0 0;
}
img {
    border-radius: 0;
    margin-top: 0;
    margin-bottom: -1rem;
}
.people_droite {
    margin-top: 0;
    border-radius: 0 0 3rem 3rem;
    height: 100%;
}
}

/* ================ PHONE ============ */
@media screen and (max-width: 600px) {

}
</style>