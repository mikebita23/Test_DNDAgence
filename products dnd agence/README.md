Test DND'Agence products/CSV
============================

Dans ce project Créer sous Symfony 4 avec Flex, je simule une commande CLI pour l'importation des données via le fichier products.csv. Ceci est quelque peu représentatif du travail fait dont je continue à m'auto-former avec d'atteindre un niveau plus meilleur. Une adaptation rapide par des strategie d'apprentissage.

Problèmes connus
================
1. Problème de versions, certaines commandes adaptées à CVS ne fonctionnent plus depuis la version 4.0 de symfony.
2. Procédure de commande pour la configuration cvs du fichier en raison du conflit de version.
3. J'aurais aimé le travailler avec une version plus récente afin d'avoir plus de lumière.
4. Problème de gestion de gros fichiers

Aide
====
1. Documentation du site officiel (je continue à apprendre et à pratiquer)
2. Forums (une communauté forte)
3. Connaissances (enseignant, amis et collègue)
4. Youtube

Exigences
=========
● Supporter la version 7.2 de PHP
● Respecter les normes PSR
● Prendre en compte les problématiques de performance et de sécurité
● Respecter les best practices de Symfony

Installation
=================
1. Pour installer mon projet, il vous faudrait premièrement faire un clone à partir de mon github
Projet de clonage
git clone https://github.com/dbrumann/product-importer.git
2. Installer les dépendances
    composer install (NB:Attention à la bonne version)
        Exécutez la commande console
            php bin/console products:import var/products.csv
Vous pouvez remplacer var/sample.csvpar l'emplacement de tout fichier csv correspondant aux exigences pour l'importation du produit.

Exemple de sortie
$ bin/console products:import var/product.csv

Apperçu après la commande
=========================

 Reads a CSV file and imports the contained products into our database.
 This command will alter your database! Please be careful when using it in production.

.....


 [OK] Finished importing products.

Si vous avez ce message, mission accompli !