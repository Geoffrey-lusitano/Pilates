<template>
    <section id="contact">
        <div class="coord">
            <h3>Contact</h3>
            <div class="coord_2">
                <div class="i1">
                    <i class="fa-solid fa-phone"> 06 72 77 51 42</i>
                </div>
                <div class="i2">
                    <i class="fa-solid fa-envelope-circle-check"> lecorpspilates@outlook.fr</i>
                </div>
            </div>

        </div>
        <div class="adresse">
            <h3>Lieux d'activité</h3>
            <br>
            <p>
                Tropic Land 135 Rue Antoine Jérôme Balard 34790 Grabels
            </p>
            <p>
                Culture & Convivialité 6B pôle d'activités Sainte Julie 34980 Montferriez-sur-Les
            </p>
            <p>
                L'Atelier du bien- être 8 Avenue des Baronnes 34730 Prades-Le-Lez
            </p>
        </div>
    </section>
</template>

<script>
export default {
    name: 'App__contact',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#contact {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
    margin: 1rem;
    color: var(--color-text-menu);
    border-radius: 3.1rem;
    background: var(--color-secondary);
    padding: 1rem;
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
}
.coord h3 {
    padding-top: 1rem;
    padding-bottom:1rem;
}
.i1 {
    padding-bottom: 1rem;
}
.adresse h3 {
    padding-bottom: 1rem;
}
.adresse p {
    padding-bottom: 1rem;
}
</style>