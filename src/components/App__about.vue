<template>
    <section id="about">
        <!-- <h2>Présentation</h2> -->
            <div class="people_gauche">
                <h3>Professeur</h3> <br>
                <h4>Marie Noëlle Dumortier</h4>
                <br>
                <ul>
                    <li>Certifiée Pilates depuis 2017</li>
                    <br>
                    <br>
                    <li>Brevet d'État Sportif</li>
                    <br>
                    <br>
                    <li>Diplômée d'État de Professeur de danse Classique</li>
                    <br>
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
                    <br>
                    <br>
                    Très vite l'envie d'enseigner est devenue évident pour moi, j'ai donc obtenu un diplôme d'État
                    en 1992 et j'ai eu la joie de diriger une école de danse à Orange dans le Vaucluse.
                    <br>
                    <br>
                    Durant mon parcours, je me suis toujours intéressée aux différentes techniques qui contribuaient
                    à améliorer la qualité du mouvement et une plus grande conscience du corps.
                    <br>
                    <br>
                    En 2012 j'ai donné une nouvelle orientation à ma vie et me suis intéressée à la méthode Pilates
                    qui était en parfaite harmonie entre mon travail acquis dans la danse et le désir de retrouver
                    une activité qui respecte l'anatomie et la physiologie du corps.
                    <br>
                    <br>
                    Aujourd'hui, j'enseigne cette technique à Grabels et à Prades-Le-Lez.
                </p>
            </div>
    </section>
</template>

<script>
export default {
    name: 'App__about',
    props: {
        msg: String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#about {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.5rem;
}
img {
    max-width: 100%;
}
</style>