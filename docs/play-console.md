# Foldbox — Play Console (Phase 2)

Copier-coller pour la fiche store. Privacy :
https://cuizinierr.github.io/foldbox-gallery/privacy.html

Package : `com.cuizinier.foldbox`  
Version : `1.4.0` (versionCode `6`)

---

## 1. Data safety (réponses recommandées)

### Vue d’ensemble
- L’app **collecte-t-elle des données utilisateur ?** → **Oui**.
- Les préférences et favoris de tutoriels restent **sur l’appareil** (AsyncStorage).
- L’ouverture de la galerie crée un identifiant technique pseudonyme Supabase. Les J’aime de la galerie sont synchronisés avec cet identifiant.
- Connexions réseau **à l’initiative de l’utilisateur / pour le contenu** :
  - GitHub (catalogue galerie)
  - Supabase (authentification pseudonyme, J’aime, soumissions et photos)
  - YouTube (lorsqu’une vidéo de tutoriel est ouverte)

### Types de données
Déclarer pour la soumission facultative :
- photos ;
- contenu généré par l’utilisateur (nom du jeu, description, origamis utilisés) ;
- nom ou pseudonyme facultatif ;
- identifiant utilisateur pseudonyme Supabase.

Déclarer également :
- **Activité dans l’application → Autres actions** pour les J’aime de la galerie ;
- **Identifiants → ID utilisateur** pour l’identifiant Supabase.

Finalités : fonctionnalité de l’application, authentification, sécurité/prévention des abus, modération et publication communautaire. Les contenus et photos sont facultatifs et déclenchés par l’utilisateur. L’identifiant pseudonyme est créé lors de l’utilisation de la galerie. Les données ne sont pas utilisées pour la publicité ou l’analyse d’audience.

Les données sont **liées à un identifiant pseudonyme**, mais ne servent pas au suivi publicitaire. Supabase agit comme prestataire de service ; la publication d’une réalisation approuvée est demandée et autorisée par l’utilisateur. Vérifier les réponses « partage » dans le formulaire Play selon ces exceptions officielles.

Ne pas déclarer de collecte pour la localisation, les contacts, les fichiers audio, le calendrier, les identifiants publicitaires ou les favoris de tutoriels.

### Sécurité
- Données chiffrées en transit (HTTPS) pour les appels réseau de l’app.
- Les utilisateurs peuvent demander la suppression → **Oui** : données locales via la suppression des données de l’app ; données Supabase et soumissions via l’adresse de contact et la référence affichée après l’envoi.
- Les contenus publics peuvent être signalés depuis leur fiche dans l’application.
- Engagement à respecter la politique destinée aux familles : **Non** (app grand public / hobby, pas ciblée enfants en priorité) — adapter si tu coches « conçu pour les enfants ».

### Privacy policy URL
`https://cuizinierr.github.io/foldbox-gallery/privacy.html`

### User-generated content
- Demander l’acceptation des règles avant chaque soumission.
- Modérer chaque texte et photo avant publication.
- Traiter les signalements reçus depuis l’application.
- URL des règles : `https://cuizinierr.github.io/foldbox-gallery/community-guidelines.html`

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
