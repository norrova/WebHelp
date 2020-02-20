# Twig

> `Edit by Norro valentin`

> Moteur de templating

## `Syntaxe` :
* `{{ variable }}` : Afficher du contenu
    * `Filtres` : `{{ variable|filter }}` :
        > https://twig.symfony.com/doc/3.x/filters/index.html
        * `upper` : AAA
        * `lower` : aaa`
        * `title` : Je Suis Un Titre
        * `length` : Longueur chc
        * `escape("")` ou `e("")` :  Echapper du code HTML
            > https://twig.symfony.com/doc/2.x/filters/escape.html
        * ...
    
* `{% command %}` : Ecrire des commandes, affectations...
    * `Filtres block` : `{% Filter filter %}`
        > https://twig.symfony.com/doc/2.x/tags/filter.html
        * `{% Filter filter|filter %}`
    * `Escape Block` : `{% autoescape false|true(base)} ... {% endautoescape %}`
        > https://twig.symfony.com/doc/2.x/filters/escape.html
* `{# commentary #}` : Commentaire
---
### `Condition` :
> https://twig.symfony.com/doc/3.x/tags/if.html
* `{% if ...}` ... `{% else|elseif %}` ... `{% endif %}`

---
### `Built-in tests` :
> https://twig.symfony.com/doc/2.x/tests/index.html
* `{% if variable is (not) test %}`
    * empty : Test si une variable est vide
    * defined : Test si une variable est défini
    * ...
### `Boucle for` : 
> https://twig.symfony.com/doc/3.x/tags/for.html
* `{% for i in 0..10 %}` ... `{% endfor %}`
