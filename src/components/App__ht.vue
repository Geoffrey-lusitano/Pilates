<template>
    <div class="container ">
      <div id="ht">
                <!-- <h2>Horaires & Tarifs</h2> -->

                <div class="horaires">
                    <h3>Horaires</h3>
                    <ul>
                        <li> <h4>Grabels</h4>
                            <ul>
                                <li>Mardi 10-11h</li>
                                <li>Mardi 18h-19h</li>
                                <li>Mercredi 10h-11h</li>
                                <br>
                                <li>135 rue Antoine Jérome Balard 34830 Grabels </li> 
                            </ul>
                        </li>
                        <li> <h4>Prades-Le-Lez</h4>
                            <ul>
                                <li>Mercredi 18h-19h</li>
                                <li>Vendredi 18h30-19h30</li>
                                <br>
                                <li>25 rue de Sauvielle 34730 Prades-Le-Lez</li>
                            </ul>
                        </li>
                        <li> <h4>Prades-Le-Lez</h4> 
                            <ul>
                                <li>Lundi 18h-19h</li>
                                <li>Jeudi 18h-19h</li>
                                <br>
                                <li>8 Avenue des Baronnes 34730 Prades-Le-Lez</li>
                            </ul>
                        </li>
                    </ul>

                </div>
                <div class="photo">
                    <div class="photo_case">
                        <a href="img/grabels.jpg"><img src="img/grabels.jpg" alt=""></a>
                    </div>
                    <div class="photo_case">
                        <a href="img/sauvielle.jpeg"><img src="img/sauvielle.jpeg" alt=""></a>
                    </div>
                    <div class="photo_case">
                        <a href="img/Atelier.jpg"><img src="img/Atelier.jpg" alt=""></a>
                    </div>
                    

                </div>
       
                   
                <div class="tarifs">
                    <h3>Tarifs</h3>
                    <br>
                    <br>
                    <ul>
                        <li>Cours à l'unité</li>
                        <br>
                        <li>15 €</li>
                        <br>
                        <li>Carte de 10 cours</li>
                        <br>
                        <li>120 €</li>
                        <br>
                        <li>A l'année 1 cour/semaine</li>
                        <br>
                        <li>390 €</li>
                        <br>
                        <li>A l'année 2 cours/semaine</li>
                        <br>
                        <li>570 €</li>
                        <br>
                        <li>Cours individuel à Domicile</li>
                        <br>
                        <li>30 €</li>
                    </ul>
                </div>

                

            </div>
    </div>
</template>

<script>
export default {
  name: 'App__ht',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>