# Power Informatique — prototype Android

Ce dossier contient un prototype d'application Android (projet Android Studio) pour réunir une vitrine de services et des fonctions pratiques.

## Fonctionnalités incluses
- Accueil et présentation des services
- Conseils informatiques et sécurité
- Formulaire de demande de devis (prépare un e-mail)
- Demande de rendez-vous (prépare un e-mail)
- Contact rapide par téléphone / e-mail
- Accès au site web
- Espace client présenté comme une fonctionnalité à connecter à un futur système sécurisé

## Important
- Le projet est un **prototype de départ**, pas un APK déjà compilé.
- Les demandes de devis et de rendez-vous ouvrent l'application e-mail du téléphone avec un message prérempli.
- L'espace client n'est pas connecté à une base de données ni à un système d'authentification.
- Le domaine `power-informatique.com` n'a pas pu être consulté automatiquement lors de la préparation. Vérifiez les coordonnées et le contenu avant publication.
- Avant diffusion, le propriétaire du site doit valider le nom, le logo, les textes, les coordonnées, la politique de confidentialité et les autorisations.

## Compiler l'APK
1. Installer Android Studio.
2. Ouvrir le dossier `PowerInformatiqueAndroid` dans Android Studio.
3. Laisser Gradle synchroniser le projet.
4. Dans le menu **Build**, choisir **Build APK(s)**.
5. Android Studio indiquera l'emplacement de l'APK généré.

## Personnalisation à faire avant publication
- Confirmer le bon site officiel et ses coordonnées.
- Ajouter le logo officiel autorisé.
- Connecter l'espace client à une API sécurisée si nécessaire.
- Ajouter une vraie politique de confidentialité et tester les formulaires.

## Compilation depuis un téléphone uniquement (GitHub Actions)
Cette archive inclut un workflow `.github/workflows/android-apk.yml` qui compile l'APK dans le cloud.
Il faut un compte GitHub et créer un dépôt, puis y téléverser les fichiers du projet en conservant leur arborescence (y compris le dossier caché `.github`).
Après l'envoi, ouvrir l'onglet **Actions**, choisir **Build Android APK**, puis **Run workflow** si nécessaire.
Quand l'exécution est terminée avec succès, ouvrir l'exécution et télécharger l'artefact **PowerInformatique-debug-apk**. Décompresser l'artefact pour récupérer `app-debug.apk`.
L'APK debug sert aux tests. Pour une publication sur Google Play, il faudra préparer une version signée et vérifier les exigences de publication.
