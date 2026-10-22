# PI PIONEER HUB — Prototype 1.0

**Slogan :** Les pionniers réunis, Pi rendu utile.

Interface responsive en français pour un hub communautaire indépendant destiné aux pionniers de Pi Network. Le prototype contient six modules : PI SAFE, PI MARKET, PI COMMUNITY, PI ACADEMY, PI APPS et PI OPPORTUNITY. Design violet, blanc et doré.

## Important
- Ceci est un prototype de démonstration côté interface, pas encore un service en production.
- Il ne réalise pas de connexion officielle à Pi Network, de paiement, de transfert de Pi, de KYC ni de stockage de données personnelles.
- Ne demandez jamais aux utilisateurs leur phrase secrète de portefeuille.
- L'utilisation de la marque et les intégrations Pi officielles doivent respecter les règles et autorisations applicables. Le projet est présenté comme indépendant.

## Lancer sur ordinateur
Prérequis : Node.js 20+ et npm.

```bash
npm install
npm run dev
```
Ouvrir l'adresse locale affichée par Vite.

Pour préparer la version web :
```bash
npm run build
npm run preview
```
Le dossier `dist/` généré est à déployer sur un hébergeur HTTPS pour permettre l'installation PWA sur Android via le navigateur.

## Installer comme application sur Android
1. Déployer le site construit (`dist/`) sur un domaine HTTPS.
2. Ouvrir le site dans Chrome sur Android.
3. Ouvrir le menu ⋮ puis choisir « Installer l'application » ou « Ajouter à l'écran d'accueil » selon le navigateur.

## Pour obtenir un APK Android natif
Cette archive est la base front-end. L'étape suivante consiste à intégrer le projet à Capacitor/Android Studio, tester sur appareils réels, signer l'application et produire un APK/AAB. Un APK signé n'est pas inclus dans cette archive.

## Feuille de route recommandée
1. Valider les écrans et le contenu avec des pionniers.
2. Définir la modération, les signalements, les conditions d'utilisation et la politique de confidentialité.
3. Créer un backend sécurisé, des comptes et des outils d'administration si nécessaires.
4. Ajouter les fonctionnalités une par une et tester la sécurité.
5. Vérifier séparément l'éligibilité et les exigences de toute intégration officielle Pi avant de l'annoncer.
6. Publier la version web, puis Android et iOS après tests et contrôles requis.

## Structure
- `src/main.jsx` : interface et navigation des modules.
- `src/style.css` : design responsive.
- `public/manifest.webmanifest` : paramètres PWA.
- `public/icon.svg` : icône provisoire.
