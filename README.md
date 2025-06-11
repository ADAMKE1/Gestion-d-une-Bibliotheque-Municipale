# Gestion d'une Bibliothèque Municipale - Projet Java

## 📝 Description du Projet
Ce projet consiste en un système de gestion de documents pour une bibliothèque municipale, développé en Java avec une interface utilisateur JavaFX et une base de données PostgreSQL. L'application permet de gérer les documents, les utilisateurs, les emprunts et les réservations.

## 👥 Membres du Groupe
- **KERROUM Adam**  
- **MALIKI Omar**  
- **BARHOINE Ayoub**  
- **MOUSSA Yassine**  

---

## 🛠 Configuration Requise

### Environnement de Développement
- **IDE** : IntelliJ IDEA (recommandé)
- **JDK** : Java Development Kit (version 8 ou supérieure)
- **Base de données** : PostgreSQL
- **JavaFX SDK** (pour l'interface graphique)

---

## 🗃 Base de Données

### Configuration
- **Nom de la base de données** : `BibliothequeMunicipale`
- **Fichier SQL fourni** : `Query.sql` (contient les scripts de création des tables)

### Étapes d'Installation
1. **Créer la base de données** :
   - Ouvrir pgAdmin 4.
   - Créer une nouvelle base de données nommée `BibliothequeMunicipale`.

2. **Importer les tables** :
   - Ouvrir le Query Tool dans pgAdmin.
   - Charger et exécuter le fichier `Query.sql` pour créer les tables.

3. **Ajouter un administrateur** :
   - Exécuter la requête fournie dans le fichier SQL pour ajouter un administrateur dans la table `personnes`.

---

## ⚙ Installation et Configuration

### 1. Configurer IntelliJ IDEA
- **Importer le projet** : Ouvrir IntelliJ et importer le dossier du projet.
- **Configurer le JDK** :
  - Vérifier que la variable d'environnement `JAVA_HOME` est définie.
  - Ajouter le chemin du JDK au `PATH`.

### 2. Pilote PostgreSQL
- **Ajouter le pilote JDBC** :
  - Dans IntelliJ, aller dans `File > Project Structure > Libraries`.
  - Ajouter le fichier `.jar` du pilote PostgreSQL (ex: `postgresql-42.x.x.jar`).

### 3. Configurer JavaFX
- **Télécharger le SDK JavaFX** :
  - Télécharger la version correspondante à votre JDK depuis [openjfx.io](https://openjfx.io/).
  - Décompresser le SDK dans un dossier accessible.

- **Ajouter JavaFX au projet** :
  - Dans IntelliJ, aller dans `File > Project Structure > Libraries`.
  - Ajouter le dossier `lib` du SDK JavaFX.

- **Configurer les options VM** :
  - Avant d'exécuter l'application, modifier la configuration de lancement pour inclure :
    ```
    --module-path /chemin/vers/javafx-sdk/lib --add-modules javafx.controls,javafx.fxml
    ```
    (Adapter le chemin selon l'emplacement du SDK sur votre machine.)

---

## 📁 Structure des Répertoires
- **`app/`** : Classe principale de l'application.
- **`DAO/`** : Classes pour la gestion des accès aux données.
- **`documents/`** : Gestion des documents de la bibliothèque.
- **`enums/`** : Énumérations utilisées dans le projet.
- **`lib/`** : Bibliothèques externes.
- **`out/`** : Fichiers compilés.
- **`personnes/`** : Gestion des utilisateurs, membres, bibliothécaires.
- **`Services/`** : Classes métiers / services applicatifs.
- **`transactions/`** : Gestion des emprunts, retours, réservations.

---

## 🔧 Fichiers à Modifier
- **`DBConnection.java`** : Mettre à jour le mot de passe de la base de données PostgreSQL.
- **Configuration JavaFX** : Vérifier les chemins d'accès au SDK.

---

## 🙏 Remerciements
Nous tenons à remercier notre encadrant **M. EL KAFHALI Said** pour son soutien et ses conseils tout au long de ce projet.

