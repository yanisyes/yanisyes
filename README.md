DUREE_ATTENTE représente la durée en millisecondes à attendre entre deux affichages.
Constante Entier_16bits DUREE_ATTENTE  2000
FONCTION vide : loop(vide) Déclarations locales
XX mémorisé XX tempsPrecedent  millis() //remplacer XX par le type requis Entier_8bits mémorisé nbreSecondes  0
XX tempsActuel //remplacer XX par le type requis XX tempsEcoule //remplacer XX par le type requis Entier valBouton
Actions
tempsActuel  millis()
tempsEcoule  tempsActuel – tempsPrecedent
SI tempsEcoule >= DUREE_ATTENTE ALORS nbreSecondes  nbreSecondes + 2
Afficher sur la console « Nombre de secondes écoulées : » suivi du contenu de la variable nbreSecondes.
tempsPrecedent  tempsActuel FSI
            // début tâche de fond
valBouton  valeur de l’entrée reliée au bouton poussoir Recopier valBouton sur la LED
// fin tâche de fond
      FIN ACTIONS
FIN FONCTION
