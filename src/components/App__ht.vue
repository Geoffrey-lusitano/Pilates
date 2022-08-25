<template>
    <section id="ht">
        <!-- <h2>Horaires & Tarifs</h2> -->
        <div class="horaires">
            <h3>Horaires</h3>
            <small>Reprise des cours à partir du lundi 29/08/22</small>
            <ul class="horaires_list">
                <li class="horaires_lieu">
                    <h4>Grabels</h4>
                    <ul>
                        <li>Mardi 10-11h</li>
                        <li>Mardi 18h-19h</li>
                        <li>Mercredi 10h-11h</li>
                        <br>
                        <li>135 rue Antoine Jérome Balard 34830 Grabels </li>
                        <a class="img_box" ><img src="../assets/grabels.jpg" alt="Tropic Land"></a>
                    </ul>
                </li>
                <li class="horaires_lieu">
                    <h4>Montferrier-sur-Lez</h4>
                    <ul>
                        <li>Mercredi 18h-19h</li>
                        <li>Jeudi 18h-19h</li>
                        <li>Vendredi 18h30-19h30</li>
                        <br>
                        <li>6B pôle d'activités Sainte Julie 34980 Montferrier-sur-Lez</li>
                        <br>
                        <a class="img_box" ><img src="../assets/sauvielle.jpeg" alt="Culture et Convivialité à Montferriez"></a>
                    </ul>
                </li>
                <li class="horaires_lieu">
                    <h4>Prades-Le-Lez</h4>
                    <ul>
                        <li>Lundi 18h-19h</li>
                        <br>
                        <li>8 Avenue des Baronnes 34730 Prades-Le-Lez</li>
                        <br>
                        <br>
                        <a class="img_box" ><img src="../assets/Atelier.jpg" alt="L'Atelier du bien- être"></a>
                    </ul>
                </li>
            </ul>
        </div>
        <div class="tarifs">
            <h3>Tarifs</h3>
            <ul>
                <li>Cours à l'unité 15 €</li>
                <li>Carte de 10 cours 125 €</li>
                <li>(valable 1 an)</li>
                <li>A l'année 1 cour/semaine 400 €</li>
                <li>A l'année 2 cours/semaine 590 €</li>
                <li>Cours individuel à Domicile 35 €</li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'App__ht',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#ht {
    color: var(--color-text-menu);
    margin: 1rem;
    margin-top: 2rem;
}
.horaires {
    background: var(--color-secondary);
    border-radius: 3rem;
    padding-bottom: 2rem;
    color: var(--color-text-sombre);
}
.horaires h3 {
    padding-top: 2rem;
    padding-bottom: 1rem;
}
.horaires_list {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.5rem;
    margin: 1rem 1rem 0 1rem;
}
.horaires h4 {
    padding-bottom: 1rem;
}
.img_box {
    border-radius: 3rem;
}
img {
    border-radius: 3rem;
    margin-top: 2rem;
    max-width:100%;
    object-fit: fill;
    
}
/* ================ Tarifs ============ */
.tarifs {
    margin-top: 1rem;
    padding-top: 2rem;
    padding-bottom: 2rem;
    background: var(--color-primary);

    width: auto;
    border-radius: 3rem;
}
.tarifs ul li {
    margin: 1rem;
}
@media screen and (max-width: 1024px) {
.horaires_list {
    display: grid;
    grid-template-columns: 1fr;
    gap: 0rem;
    margin: 1rem 1rem 0 1rem;
}

}
</style>