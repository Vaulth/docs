---
description: In-depth documentation on vaulth back-end
---

# Vaulth back-end

Afin de centraliser l’accès et de gérer les données, le backend se connecte à un nœud IPFS et Ethereum. Il écoute les événement des contrats et stocke certaines données en conséquence pour optimiser les appels aux APIs et faire en sorte que la solution soit fiable.

Express.js
Le framework backend le plus populaire, nous permet de mettre en place très rapidement des routes.

Déploiement du backend et API
En revanche, pour ce qui est de l’API et du backend, l’application est hébergée sur Amazon EC2 couplé à Cloud 66. EC2 est un service de VPS simple d’utilisation mettant à disposition du stockage et de la puissance de calcul. Cloud 66 est un service s’intégrant à EC2 permettant la gestion de l’instance EC2 mettant à disposition des fonctionnalités pratiques non disponibles par défaut sur EC2, tel que le déploiement en continu, tests, pare-feu, autorisations et une interface simple en ligne pour gérer le serveur.

