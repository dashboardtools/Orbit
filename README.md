# JavaSuite - Outil de gestion des bases de données

JavaSuite est une application Java qui facilite l'accès aux bases de données via des connecteurs JDBC. L'application permet aux utilisateurs d'interroger plusieurs bases de données en toute simplicité, sans avoir à écrire de code complexe. Elle est destinée aux organisations cherchant à déployer rapidement des accès sécurisés aux bases de données de leurs systèmes d'information.

## Fonctionnalités principales

- **Connexion multi-bases de données** : Se connecte à différentes bases de données via des connecteurs JDBC.
- **Génération de requêtes SQL automatisée** : Créez des requêtes SQL sans avoir à écrire manuellement du code.
- **Analyse des résultats en temps réel** : Affiche les résultats des requêtes sous forme de tableaux ou graphiques avec JFreeChart.
- **Sauvegarde et export des requêtes** : Sauvegardez et exportez vos requêtes SQL et résultats dans divers formats (CSV, Excel).
- **Interface utilisateur intuitive** : Application Java Swing ergonomique avec un tableau de bord complet.
  
## Installation

### Prérequis

Avant de commencer, assurez-vous que vous avez installé les éléments suivants :

- **Java 8+** installé
- **JDBC Drivers** pour vos bases de données (MySQL, PostgreSQL, Oracle, etc.)
- **Maven** (si vous souhaitez compiler le projet)

### Étapes d’installation

1. **Clonez le repository GitHub** :

    ```bash
    git clone https://github.com/tonnom/JavaSuite.git
    ```

2. **Accédez au répertoire du projet** :

    ```bash
    cd JavaSuite
    ```

3. **Compilez et exécutez l’application** :

    ```bash
    mvn clean install
    java -jar target/JavaSuite-1.0.jar
    ```

4. **Configuration des connecteurs JDBC** :

    Ajoutez les drivers JDBC pour chaque base de données que vous souhaitez utiliser dans le dossier `lib`.

5. **Lancement de l’application** :

    Après avoir exécuté la commande précédente, l'application devrait se lancer avec une interface graphique.

---

## Tutoriel : Comment utiliser JavaSuite

### Étape 1 : Connexion à une base de données

1. **Lancez l’application** et accédez à l’onglet **"Connexion"**.
2. Remplissez les champs de connexion avec les informations de votre base de données (nom du serveur, nom de la base, utilisateur et mot de passe).
3. Sélectionnez le **type de base de données** (par ex., MySQL, PostgreSQL).

![Connexion à une base de données](images/connexion.png)

4. Cliquez sur **"Connecter"**. Si la connexion est réussie, un message de succès s’affichera.

### Étape 2 : Génération d'une requête SQL

1. Allez à l'onglet **"Requête SQL"**.
2. Choisissez les tables disponibles dans la base de données connectée via le menu déroulant.
3. Utilisez l’assistant pour sélectionner les colonnes que vous souhaitez interroger.

![Sélection des tables et colonnes](images/requete_sql.png)

4. Cliquez sur **"Exécuter"** pour lancer la requête et afficher les résultats.

### Étape 3 : Visualisation des résultats

Une fois la requête exécutée, les résultats seront affichés sous forme de tableau. Vous pouvez également utiliser l’onglet **"Graphique"** pour visualiser les données sous forme de diagrammes.

![Affichage des résultats sous forme de graphique](images/graphique.png)

### Étape 4 : Export des résultats

1. Cliquez sur **"Exporter"** dans le tableau de bord.
2. Choisissez le format de sortie (CSV, Excel).
3. Sélectionnez l’emplacement pour sauvegarder le fichier.

![Export des résultats](images/export.png)

---

## Ressources supplémentaires

- [Documentation complète](https://github.com/tonnom/JavaSuite/wiki)
- [Guide pour ajouter de nouveaux connecteurs JDBC](https://github.com/tonnom/JavaSuite/wiki/Adding-JDBC-Drivers)

## Support

Si vous avez des questions ou des problèmes, n’hésitez pas à ouvrir une **issue** sur GitHub, ou à me contacter directement via [email](mailto:support@tonnom.com).

---

## Contribuer

Les contributions sont les bienvenues ! Veuillez lire le fichier [CONTRIBUTING.md](https://github.com/tonnom/JavaSuite/CONTRIBUTING.md) pour plus de détails sur le processus de contribution.

---

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](https://github.com/tonnom/JavaSuite/LICENSE.md) pour plus d’informations.
