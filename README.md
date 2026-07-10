# R&C Advisory — Page vitrine

Site vitrine single-page pour R&C Advisory, cabinet comptable 100% digital basé à Bruxelles.

## Stack

- [Astro](https://astro.build) (template minimal)
- CSS vanilla, mobile-first
- Animations via Intersection Observer (aucune lib externe)

## Développement local

```bash
npm install
npm run dev
```

Le serveur tourne sur `http://localhost:4321`.

## Déploiement sur Vercel

### Option 1 — Via l'interface Vercel (recommandé)

1. Pousser le repo sur GitHub.
2. Aller sur [vercel.com](https://vercel.com) > **Add New Project**.
3. Importer le repo `rc-advisory`.
4. Vercel détecte Astro automatiquement. Laisser les paramètres par défaut.
5. Cliquer **Deploy**.

Aucune variable d'environnement requise. Aucune configuration supplémentaire.

### Option 2 — Via CLI Vercel

```bash
npm i -g vercel
vercel
```

Suivre les prompts. Le `vercel.json` à la racine configure le build Astro.

## Personnalisations avant mise en ligne

- **Numéro WhatsApp** : remplacer `32XXXXXXXXX` dans `src/pages/index.astro` (sections Contact et Footer) par le vrai numéro au format international sans `+` ni espaces (ex. `32477123456`).
- **Email** : déjà configuré sur `ricardo@rc-advisory.be`.
- **Objet du mail** : pré-rempli à `Demande de rendez-vous - R&C Advisory`.

## Structure

```
rc-advisory/
├── src/
│   └── pages/
│       └── index.astro   # Toute la page ici
├── public/
│   └── favicon.svg
├── vercel.json
└── astro.config.mjs
```
