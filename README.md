****Création de la base de données****

php bin/console doctrine:database:create
php bin/console doctrine:schema:update --force

****Dans Postman****

***Créer un groupe***
**POST**                *localhost/APIFonctionnelle/web/groups*

{
    "nom": "createdGroup"
}


***Afficher tous les groupes***
**GET**                *localhost/APIFonctionnelle/web/groups*



***Afficher un groupe*** 
**GET**                 *localhost/APIFonctionnelle/web/groups/1*



***Modifier un groupe***
***PATCH***             *localhost/APIFonctionnelle/web/groups/1*

{
    "nom": "modifiedGroup"
}

=================================================================

***Créer un utilisateur***
**POST**                *localhost/APIFonctionnelle/web/users*

La date de création est automatiquement définie à l'initialisation de l'objet

{
        "email": "devaux_a@etna-alternance.net",
        "nom": "Devaux",
        "prenom": "Adrien",
        "actif": true
}


***Afficher tous les utilisateurs***
**GET**                *localhost/APIFonctionnelle/web/users*



***Afficher un utilisateur*** 
**GET**                 *localhost/APIFonctionnelle/web/users/1*



***Modifier un utilisateur***
***PATCH***             *localhost/APIFonctionnelle/web/users/1*

{
        "email": "devaux_a@etna-alternance.net",
        "nom": "modifiedLastName",
        "prenom": "modifiedFirstName",
        "actif": false
}
