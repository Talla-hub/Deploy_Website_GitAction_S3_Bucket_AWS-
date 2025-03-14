# Deploy_Website_GitAction_S3_Bucket_AWS

Ce projet est une démonstration d'une pipeline CI/CD de bout en bout utilisant GitHub Actions pour déployer un site web statique sur un bucket AWS S3.

## Description

Nous avons construit ce projet pour montrer comment mettre en place une pipeline d'intégration continue et de déploiement continu (CI/CD) avec GitHub Actions. À chaque commit sur la branche principale, le contenu du site statique est automatiquement synchronisé avec un bucket AWS S3, garantissant ainsi une mise à jour rapide et sécurisée de votre site web.

## Fonctionnalités

- **Intégration Continue (CI) et Déploiement Continu (CD)** : Vérification automatique du code et déploiement sur AWS S3 dès que des modifications sont poussées sur la branche main.
- **Déploiement via GitHub Actions** : Utilisation de l'action `jakejarvis/s3-sync-action` pour simplifier le processus de déploiement.
- **Gestion sécurisée des identifiants** : Stockage des informations sensibles (clés AWS, nom du bucket, etc.) sous forme de secrets GitHub.
- **Hébergement d'un site sur AWS avec un nom de domaine personnalisé et sécurisé en HTTPS** :
  - Utilisation de **CloudFront** pour la distribution du contenu avec HTTPS.
  - Configuration d'un utilisateur **IAM** pour gérer les permissions d'accès.
  - Gestion du certificat SSL via **AWS Certificate Manager**.
  - Utilisation d'un **nom de domaine acheté sur IONOS** pour personnaliser l'URL du site web.

## Installation et Configuration

1. **Créer un bucket S3** et activer l'hébergement statique.
2. **Configurer IAM** en créant un utilisateur avec les permissions nécessaires.
3. **Générer un certificat SSL** avec AWS Certificate Manager.
4. **Configurer CloudFront** pour utiliser le bucket S3 comme origine et activer HTTPS.
5. **Configurer un nom de domaine** sur IONOS et le lier à CloudFront.
6. **Mettre en place GitHub Actions** pour automatiser le déploiement.

## Utilisation

1. Cloner le dépôt :
   ```bash
   git clone <repo-url>
   cd Deploy_Website_GitAction_S3_Bucket_AWS
   ```
2. Configurer les secrets GitHub pour AWS (`AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, `AWS_BUCKET_NAME`, etc.).
3. Pousser les modifications sur la branche `main` pour déclencher la pipeline.

## Auteur

Projet développé pour démontrer l'automatisation du déploiement d'un site web statique sur AWS avec CI/CD.

---

Ce guide vous aidera à héberger un site web avec un domaine personnalisé et sécurisé sur AWS en utilisant GitHub Actions et les services AWS nécessaires.

