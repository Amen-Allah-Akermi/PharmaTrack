# PharmaTrack

PharmaTrack est une application web développée par **AKERMI Amen Allah**, permettant aux utilisateurs en Tunisie de rechercher des médicaments disponibles dans les pharmacies proches de leur localisation. Ce site est entièrement conçu et maintenu par son créateur pour fournir une solution innovante au suivi des médicaments.

## Fonctionnalités

- **Interface utilisateur et administrateur** : Deux types de comptes avec des fonctionnalités distinctes.
- **Recherche avancée de médicaments** : Trouvez des médicaments par nom, frome ou laboratoire.
- **Géolocalisation intégrée** : Localisez les pharmacies proches en temps réel tout en calculant la distance entre la localisation de la pharmacie et la localisation de l'utilisateur.
- **Gestion des stocks** : Les pharmacies peuvent gérer leur inventaire.
- **Système de suggestions intelligentes** : Propose des indications aux médicaments recherchés.
- **Interface moderne et responsive** : Adaptée aux ordinateurs, tablettes et smartphones.
- **Animations et effets visuels fluides** : Une expérience utilisateur agréable.

## Prérequis

- **PHP** : Version 7.4 ou supérieure
- **MySQL** : Version 5.7 ou supérieure
- **Serveur Web** : Apache, Nginx, ou tout autre serveur compatible
- **Navigateur Web** : Un navigateur moderne avec support JavaScript

## Installation

1. **Clonez le dépôt** :
    ```bash
    git clone https://github.com/Dr-Amenos/PharmaTrack.git
    cd PharmaTrack
    ```

2. **Configurez la base de données** :
    - Créez une base de données nommée `pharmatrack` dans MySQL.
    - Importez le script SQL depuis `database/schema.sql`.

3. **Configurer les paramètres** :
    - Ouvrez le fichier `php/config.php` et mettez à jour les informations de connexion :
    ```php
    define('DB_HOST', 'localhost');
    define('DB_USER', 'root');
    define('DB_PASS', '');
    define('DB_NAME', 'pharmatrack');
    ```

4. **Pointage du serveur web** :
    - Configurez la racine du serveur web pour pointer vers le répertoire du projet.
    - Assurez-vous que le module `mod_rewrite` est activé (pour Apache).
    - Vérifiez que PHP a les permissions nécessaires pour écrire dans les répertoires importants.

## Structure du projet

```
PharmaTrack/
├── admin_dashboard.html
├── admin_login.html
├── admin_registration.html
├── admin_registration.php
├── check_stock.php
├── choix_admin.html
├── index.html
├── LICENSE.txt
├── README.md
├── update_medicament.php
├── update_schema.sql
├── user_registration.html
├── user_search.html
├── css/
│   └── style.css
├── images/
│   └── logo.png
├── js/
│   └── main.js
├── php/
│   ├── add_medicament.php
│   ├── admin_login.php
│   ├── config.php
│   ├── create_tables.php
│   ├── debug_register.php
│   ├── functions.php
│   ├── get_indications.php
│   ├── get_regions.php
│   ├── get_stock.php
│   ├── insert_regions.php
│   ├── login_admin.php
│   ├── login_pharmacy.php
│   ├── logout.php
│   ├── logout_pharmacy.php
│   ├── recherche.php
│   ├── register_admin.php
│   ├── register_pharmacy.php
│   ├── register_user.php
│   ├── remove_medicament.php
│   ├── search_medicament.php
│   ├── setup_database.php
│   ├── suggestions.php
│   ├── test_connection.php
│   ├── test_register.php
│   └── update_medicament.php
```

## Utilisation

### Pour les utilisateurs

1. Rendez-vous sur la page d'accueil.
2. Cliquez sur "Utilisateur".
3. Créez un compte en remplissant le formulaire d'inscription.
4. Autorisez l'accès à votre géolocalisation.
5. Recherchez des médicaments.

### Pour les pharmacies

1. Rendez-vous sur la page d'accueil.
2. Cliquez sur "Administrateur".
3. Créez un compte pharmacie.
4. Connectez-vous pour gérer votre stock de médicaments.

## Sécurité

- **Hashage des mots de passe** : Les mots de passe sont sécurisés avec `password_hash()`.
- **Validation des entrées utilisateur** : Toutes les données utilisateur sont nettoyées.
- **Protection contre les injections SQL** : Utilisation de PDO pour l'accès à la base de données.
- **Sessions sécurisées** : Gestion stricte des sessions utilisateur.

## Contribution

Ce projet est principalement conçu pour un usage professionel. Cependant, les suggestions des modifications sont les bienvenues. 
1. Forkez le dépôt.
2. Créez une nouvelle branche pour vos modifications.
3. Effectuez vos commits.
4. Poussez votre branche et ouvrez une Pull Request.

## Licence

Ce projet est sous licence MIT. Consultez le fichier `LICENSE.txt` pour plus de détails.

## Support

Pour toute question ou problème, veuillez me contacter directement via mon profil GitHub ou ouvrir une issue.

---
Développé avec ❤️ par **AKERMI Amen Allah**.
