# Hameau Retrouvé — Mountain Modern

Un site vitrine statique, rapide et immersif pour mettre en avant le chalet Hameau Retrouvé aux Carroz d'Arâches.

## Structure du projet

```
site-chalet/
├─ index.html           # Page principale (navigation par onglets)
├─ mentions-legales.html # Mentions légales complètes
├─ assets/
│  ├─ css/
│  │  └─ main.css       # Styles globaux (variables, layout, responsive)
│  ├─ js/
│  │  └─ main.js        # Navigation, lightbox, animations et lazy loading
│  ├─ images/           # Photothèque du chalet (hero, galerie, activités)
│  └─ favicon.svg       # Icône "HR" pour les navigateurs
└─ README.md            # Documentation projet
```

## Caractéristiques clés

- Hero fullscreen avec effet de zoom et CTA "Voir le chalet".
- Navigation fixe avec changement d'apparence au scroll.
- Galerie 9 images avec visionneuse (lightbox) et légendes.
- Sections complètes : accueil, localisation, activités, contact.
- Formulaire Netlify prêt à être connecté.
- Animations douces au scroll via `IntersectionObserver`.
- 100 % responsive (desktop, tablette, mobile).
- Favicon personnalisé "HR" pour renforcer l'identité visuelle.

## Fonctionnalités techniques

- HTML5 sémantique + CSS Grid/Flexbox + variables CSS.
- JavaScript vanilla (aucune dépendance externe).
- Lazy loading des images et reveal progressif des blocs.
- Navigation par onglets côté client (`showTab` dans `main.js`).
- Carte OpenStreetMap intégrée (iframe) et liens contextuels.

## Prise en main

1. Ouvrir `index.html` dans votre navigateur.
2. Déposer vos photos dans `assets/images/` en conservant les mêmes noms (ou mettre à jour les `src`).
3. Adapter les textes (tarifs, disponibilités, liens Airbnb) directement dans `index.html`.
4. Ajuster les couleurs/typographies dans `assets/css/main.css` si nécessaire.
5. Mettre à jour les informations légales dans `mentions-legales.html` (éditeur, SIRET, hébergeur, données personnelles).
6. Personnaliser le `assets/favicon.svg` si vous souhaitez un autre pictogramme.

## Déploiement Netlify

1. Pousser ce dossier sur GitHub.
2. Créer un site Netlify et connecter le repo (aucun build requis).
3. Netlify détecte automatiquement le formulaire `name="contact"`.
4. Ajouter un domaine personnalisé ou utiliser celui fourni.

## SEO & bonnes pratiques

- Balises `meta` description + attributs `alt` sur toutes les images.
- Contenu structuré par sections pour une lecture claire.
- CSS et JS uniques (faciles à minifier avant production).
- Pas de librairies lourdes pour garder des temps de chargement courts.

## Support / évolutions

- Ajouter d'autres pages statiques en dupliquant `index.html` si besoin.
- Pour passer à un générateur statique (11ty, Astro, etc.), réutiliser les assets actuels.
- Besoin d'aide ? Documentez vos changements dans ce README pour garder l'historique clair.

---

**Dernière mise à jour : 17 novembre 2025**
