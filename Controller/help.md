# Controller

> `Edited by Norro valentin`

## `Comprendre` : 
> https://symfony.com/doc/current/controller.html
* Fichier classe PHP

## `Syntaxe` :
* Créer une contrôleur : `php bin/console make:controller [name]Controller`
* `Annotations` : 
    * `@Route` : Chemin d'accès
* Les méthodes des contrôleurs retournent toujours des objets `Response`
    > https://symfony.com/doc/current/components/http_foundation.html#response
* Pour rendre une vue :`$this->render("path")`
    > https://symfony.com/doc/current/templates.html#rendering-templates

### `Route` :
* Les routes se configurent soit par les annotations, ou en YAML
    > https://fr.wikipedia.org/wiki/YAML
    * Location : `./config/route.yaml`
    ```
    nomDeLaRoute (peu importe):
        path : "requête" (exemple : "/")
        controller : App\Controller\NomDuController::méthode
    ```
