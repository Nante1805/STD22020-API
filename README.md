# STD22020-API
# Documentation de l'API

Ceci est la documentation de l'API pour STD22020, fournissant des informations sur les étudiants et les enseignants.

## Endpoints

### Étudiants

- **GET /students**
  - Description : Récupérer des informations sur le statut des étudiants.
  - Réponse :
    - Statut 200 : Réponse réussie avec les données de l'étudiant.
    - Statut 500 : Erreur interne du serveur.

- **POST /students**
  - Description : Mettre à jour ou créer des informations sur le statut des étudiants.
  - Corps de la requête : Données JSON avec les informations de l'étudiant.
  - Réponse :
    - Statut 200 : Réponse réussie avec les données de l'étudiant mises à jour.
    - Statut 500 : Erreur interne du serveur.

- **PUT /students**
  - Description : Mettre à jour les informations de l'étudiant.
  - Réponse :
    - Statut 200 : Réponse réussie avec les données de l'étudiant mises à jour.
    - Statut 500 : Erreur interne du serveur.

- **DELETE /students**
  - Description : Supprimer les informations de l'étudiant.
  - Réponse :
    - Statut 200 : Réponse réussie.
    - Statut 500 : Erreur interne du serveur.

### Enseignants

- **GET /teachers**
  - Description : Récupérer des informations sur les enseignants.
  - Réponse :
    - Statut 200 : Réponse réussie avec les données de l'enseignant.
    - Statut 500 : Erreur interne du serveur.

- **POST /teachers**
  - Description : Créer des informations sur les enseignants.
  - Corps de la requête : Données JSON avec les informations de l'enseignant, y compris les cours enseignés.
  - Réponse :
    - Statut 200 : Réponse réussie avec les données de l'enseignant créé.
    - Statut 500 : Erreur interne du serveur.

## Modèles de Données

### Étudiant

- `id` (entier) : Identifiant unique de l'étudiant.
- `name` (chaîne de caractères) : Nom de l'étudiant.
- `Birthday` (date) : Date de naissance de l'étudiant.

### Enseignant

- `id` (entier) : Identifiant unique de l'enseignant.
- `firstName` (chaîne de caractères) : Prénom de l'enseignant.
- `lastName` (chaîne de caractères) : Nom de famille de l'enseignant.
- `courses` (tableau) : Liste des cours enseignés par l'enseignant, comprenant :
  - `code` (chaîne de caractères) : Code du cours.
  - `name` (chaîne de caractères) : Nom du cours.
  - `duration` (entier) : Durée du cours en heures.
  
## Liens
https://petstore.swagger.io/?url=https://raw.githubusercontent.com/Nante1805/STD22020-API/master/openapi.yaml
