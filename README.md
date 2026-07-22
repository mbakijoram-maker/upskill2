# UPskill v3 — UI premium + UPSKILL IA (Gemini)

Réseau social + plateforme freelance, **stockage local**, **avatars illustrés**,
**stories style Instagram**, **chat IA intégré**.

## 🆕 Nouveautés v3

- **UPSKILL IA** : chat intelligent intégré (basé sur Gemini) — toujours en tête des messages
- **Avatars illustrés** : motifs colorés générés automatiquement quand pas de photo
- **Cartes longues animées** dans Explorer, style Instagram Stories preview
- **Strip stories** horizontal en haut de l'Explorer avec rings animés
- **Glow subtil** sur toutes les cartes (très léger, pas agressif)
- **Animations d'apparition** (fade + slide) sur les listes
- **15 utilisateurs démo** (vs 4) — plus aucun post / commentaire / conversation fictifs
- **Cible mobile** : ergonomie tactile, bottom nav, touch targets 44+

## 🚀 Lancement

```powershell
flutter create . --platforms=web
flutter pub get
flutter run -d chrome
```

## 🤖 UPSKILL IA

L'IA est branchée sur Gemini 1.5 Flash. Elle :
- répond toujours en français, chaleureuse et concise
- ne révèle jamais qu'elle est basée sur Gemini
- garde l'historique de la conversation dans localStorage
- peut être effacée via l'icône poubelle en haut à droite du chat

⚠️ **Sécurité de la clé API** : la clé Gemini est embarquée côté client. Pour un
usage personnel/démo c'est OK, mais pour publier : restreins la clé dans Google
Cloud Console (à un domaine, une IP) ou passe par un backend proxy.

## 📱 Cible mobile

Le projet est conçu **pour iOS/Android** ; le web n'est qu'un aperçu. Pour
compiler iOS, il te faudra un Mac (Flutter ne compile iOS que sur macOS).

## 🧪 Comptes démo (mot de passe : `demo1234`)

15 profils diversifiés : Freelancers (Léa, Maxime, Camille, Hugo) · Artistes (Arthur,
Yuki, Sofia, Noah) · Entreprises (StudioCréa, PixelForge, LumièreCom) · Clients
(Sophie, Karim, Elena, Tom).

Tu peux te connecter avec n'importe lequel : `lea@upskill.app`, `arthur@upskill.app`,
`pixelforge@upskill.app`, etc.

## 🗂️ Structure

```
lib/main.dart    ~2400 lignes — tout est ici (data, UI, IA)
pubspec.yaml     6 dépendances
```
