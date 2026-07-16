# Foldbox — Play Console (Phase 2)

Copier-coller pour la fiche store. Privacy :
https://cuizinierr.github.io/foldbox-gallery/privacy.html

Package : `com.cuizinier.foldbox`  
Version : `1.4.0` (versionCode `6`)

---

## 1. Data safety (réponses recommandées)

### Vue d’ensemble
- L’app **collecte-t-elle des données utilisateur ?** → **Non** (pas de compte, pas d’analytics in-app, pas d’envoi de likes/favoris vers un serveur Foldbox).
- Les préférences, likes et favoris restent **sur l’appareil** (AsyncStorage).
- Connexions réseau **à l’initiative de l’utilisateur / pour le contenu** :
  - GitHub (catalogue galerie)
  - Google Forms (soumission volontaire d’une réalisation)
  - YouTube (vidéos désactivées dans la bêta actuelle)

### Types de données
Ne **pas** déclarer de collecte pour :
- Localisation, contacts, photos de l’appareil, fichiers audio/vidéo locaux, calendrier, etc.
- Identifiants appareil / pub / analytics Foldbox

**Soumission galerie (optionnelle)** : si Play Console demande les données transmises à un tiers via formulaire externe, indiquer que l’utilisateur ouvre **Google Forms** dans le navigateur et y fournit volontairement texte/photos — traité par Google, hors app. Pas de SDK Google Forms embarqué.

### Sécurité
- Données chiffrées en transit (HTTPS) pour les appels réseau de l’app.
- Les utilisateurs peuvent demander la suppression → **Oui** pour les données locales : désinstaller l’app / effacer le stockage app.
- Engagement à respecter la politique destinée aux familles : **Non** (app grand public / hobby, pas ciblée enfants en priorité) — adapter si tu coches « conçu pour les enfants ».

### Privacy policy URL
`https://cuizinierr.github.io/foldbox-gallery/privacy.html`

---

## 2. Listing FR

**Titre de l’application** (max 30)  
`Foldbox`

**Description courte** (max 80)  
`Tutoriels d’origami pour ranger vos boîtes de jeux.`

**Description longue**  
```
Foldbox vous guide pas à pas pour plier vos propres boîtes, séparateurs et pochettes — idéales pour organiser les composants de vos jeux de société.

• Tutoriels clairs avec illustrations
• Calculateur de dimensions (cm ou pouces)
• Mode pas-à-pas confortable
• Galerie d’inspirations de la communauté
• Thème clair / sombre et interface en français ou anglais

Aucun compte requis. Vos likes et préférences restent sur votre appareil.

Politique de confidentialité :
https://cuizinierr.github.io/foldbox-gallery/privacy.html
```

**Catégorie**  
Jeux → (ou) Loisirs / Productivité selon le classement Play le plus proche — recommandé : **Loisirs** ou **Mode de vie**.

**Tags / mots-clés** (si proposés)  
origami, pliage, jeux de société, boardgame, organisation, tutoriel

**E-mail de contact**  
À renseigner (obligatoire) — ton e-mail développeur.

**Site web** (optionnel)  
https://cuizinierr.github.io/foldbox-gallery/

---

## 3. Listing EN (optionnel)

**Short description**  
`Origami tutorials to organize your board game boxes.`

**Full description**  
```
Foldbox guides you step by step to fold your own boxes, dividers, and sleeves — perfect for organizing board game components.

• Clear illustrated tutorials
• Dimension calculator (cm or inches)
• Comfortable step-by-step mode
• Community inspiration gallery
• Light / dark theme and French or English UI

No account required. Likes and preferences stay on your device.

Privacy policy:
https://cuizinierr.github.io/foldbox-gallery/privacy.html
```

---

## 4. Assets visuels

| Asset | Spec | Statut |
|-------|------|--------|
| Feature graphic | 1024 × 500 | à générer / déposer |
| Screenshots téléphone | min. 2 (idéalement 4–8), PNG/JPEG | dossier `store-assets/` dans l’app |
| Icône | adaptive + monochrome | OK (Phase 1) |

Écrans suggérés : bibliothèque, fiche tutoriel, calculateur, étapes, galerie, réglages.
