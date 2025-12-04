# Projet d'Intégration Web - Gestion des Réclamations Esprit

Ce projet est une interface web pour la gestion des réclamations au sein de l'université Esprit, réalisée avec HTML5 et Tailwind CSS.

## 👥 Liste des membres de l’équipe et leurs responsabilités

- **[Nom du Membre 1]** : [Description des responsabilités, ex: Conception de la page Login, Intégration Dashboard]
- **[Nom du Membre 2]** : [Description des responsabilités, ex: Page Détails du Profil, Responsive Design]
- **[Nom du Membre 3]** : [Description des responsabilités, ex: Formulaire d'ajout de réclamation, Charte graphique]
- **[Nom du Membre 4]** : [Description des responsabilités]

_(Veuillez compléter cette liste avec les noms réels et les tâches spécifiques de chaque membre)_

## 🚀 Instructions pour exécuter le projet

Ce projet est statique (HTML/CSS/JS), il est donc très simple à lancer.

### Prérequis

- Un navigateur web moderne (Chrome, Firefox, Edge, Safari).
- (Optionnel) **Node.js** et **npm** si vous souhaitez recompiler le CSS Tailwind.

### Étapes pour lancer le projet

1.  **Télécharger ou cloner le projet** sur votre machine locale.
2.  **Ouvrir les fichiers HTML** :
    - Naviguez dans le dossier du projet.
    - Double-cliquez sur `index.html` pour voir la page d'accueil/login.
    - Vous pouvez également ouvrir directement les fichiers dans le dossier `pages/` :
      - `pages/Dashboard.html` : Tableau de bord principal.
      - `pages/AddreclamationDashboard.html` : Formulaire de nouvelle réclamation.
      - `pages/ProfileDetails.html` : Gestion du profil utilisateur.

### (Développement) Modification du CSS Tailwind

Si vous devez modifier les styles Tailwind et régénérer le fichier CSS :

1.  Ouvrez un terminal à la racine du projet.
2.  Installez les dépendances :
    ```bash
    npm install
    ```
3.  Lancez la compilation en mode "watch" (surveillance) :
    ```bash
    npm run build-css
    ```

## 🛠️ Problèmes rencontrés et solutions apportées

Voici une liste des défis techniques rencontrés durant le développement et comment nous les avons résolus :

1.  **Sidebar Responsive sur Mobile**

    - **Problème** : La barre latérale (sidebar) prenait trop de place sur les petits écrans et cassait la mise en page.
    - **Solution** : Nous avons implémenté un menu "hamburger" pour mobile. La sidebar est désormais cachée par défaut sur mobile (`-translate-x-full`) et s'affiche avec une animation fluide lors du clic sur le bouton, accompagnée d'un overlay sombre pour focaliser l'attention.

2.  **Mise en page des Formulaires Complexes**

    - **Problème** : Aligner correctement les champs de saisie, les zones de texte et les boutons d'upload (comme sur la page "Nouvelle réclamation") était difficile avec du CSS standard.
    - **Solution** : Utilisation intensive de **CSS Grid** (`grid-cols-1`, `md:grid-cols-3`) et **Flexbox** via Tailwind CSS pour créer des mises en page réactives qui s'adaptent automatiquement à la taille de l'écran (passage de 3 colonnes à 1 colonne sur mobile).

3.  **Cohérence du Design (Couleurs et Polices)**

    - **Problème** : Maintenir l'identité visuelle d'Esprit (Rouge `#D2232A`, Police `Inter`) sur toutes les pages.
    - **Solution** : Utilisation des classes utilitaires de Tailwind pour les couleurs (`text-[#D2232A]`, `bg-[#D2232A]`) et importation globale de la police Google Fonts "Inter" dans le `<head>` de chaque page.

4.  **[Autre Problème Rencontré]**
    - **Problème** : [Description du problème]
    - **Solution** : [Description de la solution]

_(N'hésitez pas à ajouter d'autres défis spécifiques que vous avez rencontrés)_
