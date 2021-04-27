**Etape 1**
> Vérifier la version de PHP

```php -v```

Symhphony fonctionne à partir de la version 7.2.5, sauf sur la version 7.4.0

Pour mettre à jour PHP : https://brew.sh/index_fr



**Etape 2**
> Installer Composer

https://getcomposer.org/download/

Sur mac, utiliser les commandes décrites. Sur Windows, utiliser l'executable

Terminer par la commande : ```mv composer.phar /usr/local/bin/composer```



**Etape 3**

> Installer Symphony

https://symfony.com/download

Pareil que pour Composer : Lignes de commandes sur Mac, executable sur Windows

Pour finaliser, utiliser la commande donnée commençant par ```mv``` (après "Or install it globally on your system:")



**Etape 4**
> Créer un nouveau projet Symfony

```symfony new nomDuDossierCréé --full```



**Etape 5**
> Créer la base de donnée

Dans le fichier ```.env```, mettre la ligne 31 en commentaire et décommenter la ligne 30. Modifier la ligne avec les informations de la bdd voulue

Une fois fait, utiliser la commande ```php bin/console doctrine:database:create````



**Etape 6**
> Créer le serveur Symfony

```symfony server:start```