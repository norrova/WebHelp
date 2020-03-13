# `Doctrine` In progress
> `Edited by Norro valentin` 

> Object-Relational Mapping : `Illusion d’une base de données orientée objet à partir d’une base relationnelle classique`
> https://www.developpez.com/actu/46628/Etes-vous-pour-ou-contre-les-ORM-Un-blogueur-invite-a-tenir-le-baton-par-le-milieu/

## `Comprendre` : 
* Entité : `Table`
* Manager : `Insert, Delete` => Manipuler les données d'une table
* Repository : `Select` => Récupérer des informations

## `Commandes` :

* Créer une `base de données` :
 `php bin/console doctrine:database:create`
    > https://symfony.com/doc/current/doctrine.html

    * Créer une entité : `Ensemble homogène d’informations` | `nom unique`
        * `php bin/console make:entity`
        > https://www.base-de-donnees.com/entite/
        * Location : `src/Entity/[name].php`
        * Relation : cf `./Doctrine ORM/database.md`
* `Migration`
* `Fixtures` : Fake data
    > https://symfony.com/doc/current/bundles/DoctrineFixturesBundle/index.html
    * Install : `composer require --dev orm-fixtures`
        * Create fixtures : `php bin/console make:fixtures
        * Création des données :
            * Inclure l'entité (la table)
            * Créer une instanciation de la classe d'une entité
        * Insérer les fixtures dans la base de données: `php bin/console doctrine:fixtures:load` 
            * ☢️ Purge la base de données
    