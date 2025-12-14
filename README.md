### CI/CD Spring Boot avec Jenkins, Docker et GitHub Webhook
Objectif du TP

Ce projet a pour objectif de mettre en place un pipeline CI/CD complet pour une application Spring Boot, en utilisant Jenkins, Maven, Docker, GitHub Webhook et ngrok.

Le pipeline permet :

l’intégration continue (CI) : build et tests automatiques

la livraison/déploiement continu (CD) : création et exécution d’un conteneur Docker

le déclenchement automatique à chaque push GitHub

Outils et technologies utilisés

Java JDK

Maven

Spring Boot

Git & GitHub

Jenkins

Docker

ngrok

### Étapes de réalisation
1. Installation de Jenkins

Téléchargement et installation de Jenkins sur Windows

Accès à Jenkins via http://localhost:8080

Configuration initiale (mot de passe admin et plugins recommandés)

<img width="1366" height="728" alt="Tableau de bord - Jenkins - Google Chrome 14_12_2025 21_55_59" src="https://github.com/user-attachments/assets/fa09d730-0f87-4dce-82cf-811e0b1dc5b9" />

### 2. Configuration de Maven dans Jenkins

Accès au menu Manage Jenkins

Ajout de Maven dans la section Tools

Activation de l’installation automatique de Maven
<img width="1366" height="728" alt="Tableau de bord - Jenkins - Google Chrome 14_12_2025 21_58_15" src="https://github.com/user-attachments/assets/873d6c2a-cd4f-4158-8383-3725c4a7ce2d" />


3. Préparation du projet Spring Boot

Récupération du projet de base depuis GitHub

Vérification du build Maven en local

Création d’un dépôt GitHub personnel

Publication du projet sur le dépôt GitHub


4. Création du job Pipeline Jenkins

Création d’un nouveau job de type Pipeline

Ajout de l’URL du projet GitHub

Activation du déclencheur GitHub hook trigger for GITScm polling

Définition du pipeline CI/CD

<img width="1366" height="728" alt="Tableau de bord - Jenkins - Google Chrome 14_12_2025 22_14_53" src="https://github.com/user-attachments/assets/cc14c099-4bec-4502-a6cf-71129608b7cd" />
<img width="1366" height="728" alt="Tableau de bord - Jenkins - Google Chrome 14_12_2025 22_19_19" src="https://github.com/user-attachments/assets/ea9a16a2-687d-49c2-9c70-c3c918beb120" />

5. Exécution du pipeline CI/CD

Le pipeline exécute les étapes suivantes :

Récupération du code depuis GitHub

Build et tests du projet avec Maven

Création d’une image Docker

Lancement d’un conteneur Docker
<img width="1366" height="728" alt="Tableau de bord - Jenkins - Google Chrome 14_12_2025 22_23_01" src="https://github.com/user-attachments/assets/9c4cf6ff-a903-493e-80c0-202f2216459c" />
<img width="1366" height="728" alt="Tableau de bord - Jenkins - Google Chrome 14_12_2025 23_16_41" src="https://github.com/user-attachments/assets/0df1e544-66e4-48fb-ac6d-8e568cdfd557" />
<img width="1366" height="728" alt="my-project - Jenkins - Google Chrome 14_12_2025 22_39_39" src="https://github.com/user-attachments/assets/ce787a84-65ba-4e2c-abd3-0ce88e6899ca" />
<img width="1366" height="728" alt="my-project - Jenkins - Google Chrome 14_12_2025 22_38_57" src="https://github.com/user-attachments/assets/8f641c3d-79c1-4054-919c-76801cc25c72" />


6. Exposition de Jenkins avec ngrok

Installation et configuration de ngrok

Création d’un tunnel sécurisé vers Jenkins

Obtention d’une URL publique pour Jenkins


7. Configuration du webhook GitHub

Ajout d’un webhook dans le dépôt GitHub

Configuration de l’URL ngrok avec /github-webhook/

Sélection de l’événement push

Activation du webhook
<img width="1366" height="728" alt="Add webhook - Google Chrome 14_12_2025 23_01_41" src="https://github.com/user-attachments/assets/63be535a-c80f-4cac-aa7c-8141849d5ea4" />
<img width="1366" height="728" alt="Add webhook - Google Chrome 14_12_2025 23_01_52" src="https://github.com/user-attachments/assets/05cb1087-917b-4969-95f5-4bd423bfcb68" />



<img width="1366" height="728" alt="Images - Docker Desktop 14_12_2025 23_16_35" src="https://github.com/user-attachments/assets/5f1cf838-ecdc-4243-9ab2-69d45dc529f7" />


