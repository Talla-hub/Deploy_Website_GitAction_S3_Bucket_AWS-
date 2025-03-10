# Deploy_Website_GitAction_S3_Bucket_AWS

Ce projet est une démonstration d'une pipeline CI/CD de bout en bout utilisant GitHub Actions pour déployer un site web statique sur un bucket AWS S3.

## Description

Nous avons construit ce projet pour montrer comment mettre en place une pipeline d'intégration continue et de déploiement continu (CI/CD) avec GitHub Actions. À chaque commit sur la branche principale, le contenu du site statique est automatiquement synchronisé avec un bucket AWS S3, garantissant ainsi une mise à jour rapide et sécurisée de votre site web.

## Fonctionnalités

- **Intégration Continue (CI) et Déploiement Continu (CD)** : Vérification automatique du code et déploiement sur AWS S3 dès que des modifications sont poussées sur la branche `main`.
- **Déploiement via GitHub Actions** : Utilisation de l'action [jakejarvis/s3-sync-action](https://github.com/jakejarvis/s3-sync-action) pour simplifier le processus de déploiement.
- **Gestion sécurisée des identifiants** : Stockage des informations sensibles (clés AWS, nom du bucket, etc.) sous forme de secrets GitHub.


