# Qui-Ose

Qui-Ose est une application web conçue pour aider les élèves à trouver des stages correspondant à leurs programmes d'études.

## Technologies utilisées

- **React** : Front-end
- **Java** : Back-end (Spring Boot)
- **PostgreSQL** : Base de données
- **JWT** : Sécurité

---

## Comment faire fonctionner l'application

### 1. Installation des dépendances

Clonez le dépôt du projet depuis le dépôt GitHub :
```bash
git clone <url_du_depot>
cd <nom_du_projet>
```

#### Pour le Front-end (React) :
```bash
cd frontend
npm install
```

#### Pour le Back-end (Java) :
Assurez-vous d’avoir Maven ou Gradle configuré et exécutez :
```bash
mvn install
```

---

### 2. Configuration de la base de données

- Installez PostgreSQL.
- Créez une base de données dédiée pour l’application.
- Mettez à jour les fichiers de configuration dans le dossier **back-end** (par exemple, `application.properties` ou `application.yml`) avec vos informations :
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/<nom_base>
spring.datasource.username=<votre_utilisateur>
spring.datasource.password=<votre_mot_de_passe>
```

---

### 3. Démarrage de l'application

#### Démarrage du serveur Back-end (Spring Boot) :
Depuis le dossier du back-end, lancez :
```bash
mvn spring-boot:run
```
Par défaut, le serveur sera disponible sur **http://localhost:8080**.

#### Démarrage du serveur Front-end (React) :
Depuis le dossier `frontend`, lancez :
```bash
npm start
```
L'application front-end sera disponible sur **http://localhost:3000**.

---

### 4. Connexion et utilisation

- Ouvrez l’interface web (React) dans votre navigateur : [http://localhost:3000](http://localhost:3000).
- Inscrivez-vous ou connectez-vous pour accéder aux fonctionnalités :
  - **Recherche de stages**
  - **Soumission de candidatures**
  - **Gestion des profils étudiants et employeurs**

---

### 5. Déploiement

Pour déployer l'application en production, suivez ces étapes :

#### Utilisation de Docker :
- Créez des fichiers `Dockerfile` et `docker-compose.yml` pour containeriser le front-end, le back-end et la base de données.

#### Hébergement :
- Utilisez une plateforme comme **Heroku**, **AWS**, ou **Google Cloud** pour déployer vos services.

---

### Bonnes pratiques

- **Mise à jour** : Gardez vos dépendances (npm et Maven) à jour pour éviter les vulnérabilités.
- **Sauvegardes** : Effectuez des sauvegardes régulières de votre base de données PostgreSQL.
- **Tests** : Testez l'application dans différents environnements (développement, production) avant le déploiement.

---

## Auteur

Développé par Mikhail Kurilenko.
