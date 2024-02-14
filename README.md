#unités de mesure sur css

##unité absolue
px / cm / pica / point
- ne change pas peut-importe la taille de l'écran
- utilisé sur des dimensions fixes

##pourcentage
%
- se réfère à la taille de l'élement parent

##unité textuelle
ch / em / rem
- em : se réfère par rapport à la taille du police parent
    - se calcul par chiffre*taille du police de l'element parent

- rem : se réfère par rapport à la taille du police racine (html)
    - se calcul par chiffre*taille de la balise
    - par exemple la taille du police racine d'un balise h1 est très grande par rapport à la taille d'un balise p donc avec
    h1{
        font-size : 2rem;
    }
    p{
        font-size : 2rem;
    }
    la différence de taille entre h1 et p reste la même même si leur tailles se sont multipliées

- ch : se réfère par rapport à la taille du police utilisé
    - se calcul par chiffre*taille du police utilisé

##unité viewport
vh / vw
- vh : se réfère à la longueur de la fenêtre
    - 1vh représente 1% de la longueur de la fenêtre

- vw : se réfère à la largeurr de la fenêtre
    - 1vw représente 1% de la largeur de la fenêtre

##unité par rapport au document
dvh / dvw
- dvh : se réfère à la longueur du document ou du contenu plutôt que la longueur de la fenêtre
- dvw : se réfère à la largeur du document

##meilleur pratique et unités à éviter

situation : pour faire des responsives design
- utiliser les unités de viewport pour ne pas corrompre le design
- éviter les unités absolues comme les pixels

situation : pour faire le design (les mieux recommandés selon moi)
- privilégier l'usage des unités par rapport au document (dvh,dvw) pour avoir des unités adaptables à divers contenus et pour éviter les espacements non conformes entre certains contenus
- utiliser rem pour les textes pour conserver la différence de la taille entre les balises
