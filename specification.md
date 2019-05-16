# UNE APPLICATION POUR MESSAGE DE FOULE ?

Vous avez déjà vu ce genre de message visible du ciel, écrit par des attroupements. C'est un bon moyen de communication mais ça demande de la préparation.

# L'IDÉE est de développer en logiciel libre, une application web qui permet d'organiser facilement ce genre de happening et d'aller plus loin.
Ce n'est pas très difficile.

# LE PRINCIPE

Grâce à Google Maps on dispose des vues aériennes d'une grande partie de la planète et des coordonnées GPS associées. 
Imaginez que vous superposiez un texte sur une vue arérienne et qu'un logiciel envoie à chaque participant les coordonnées GPS de la position qu'elle doit prendre avec l'idée que 1 personne = 1 pixel.
Le logiciel tiendrait compte du nombre de personnes disponibles pour calculer les positions à occuper de manière à rendre le message le plus lisible.
Lorsqu'une personne rejoint le groupe qui compose le message, le serveur web lui attribue une position.
Une fois que la personne a reçu sa position en coordonnées GPS, elle utilise son smartphone pour s'y placer.

#  CÔTÉ PARTICIPANTS : l'adresse d'un site web
La version la plus simple de réaliser cette coordination consiste en un site web qui reçoit une demande de participation et 
renvoie une position GPS. Il n'y a pas de communication des identifiants et de la position GPS de l'utilisateur.
Le site web se contente de compter le nombre de personnes connectées et de renvoyer des positions GPS.

# CÔTÉ ORGANISATEUR: le logiciel qui alimente le site web prend une message positionné sur une vue aérienne et en déduit une liste de position à occuper.

# ENCORE PLUS FORT MAIS PAS BEAUCOUP PLUS DIFFICILE
Sur le même principe on peut imaginer plus ambitieux avec des messages évolutant dans le temps.
Chaque personne connectée au site reçoit une position GPS pour un premier message et quelques minutes plus tard, elle reçoit une nouvelle position
pour un autre texte et ainsi de suite. Par rapport à la version précédente le logiciel doit en plus minimiser les déplacements des personnes.
