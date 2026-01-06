# IVS Studio

Application web de streaming en temps réel utilisant Amazon IVS Real-time.

## Fonctionnalités (v35)

- **Mode Viewer** : Regarder les flux en direct
- **Mode Contributeur** : Diffuser sa caméra/micro
- **Gestion des stages** : Créer, supprimer, lister les stages IVS
- **Design System** : Thème dark/light, responsive
- **VU-mètre** : Indicateur de niveau audio en temps réel
- **Chat** : Panel de discussion (local uniquement pour l'instant)

## À corriger (TODO)

- [ ] **Plein écran** : Comportement à améliorer
- [ ] **Couper le son** : Problème avec le mute global/individuel
- [ ] **Mode mobile** : Optimisations iOS/Safari nécessaires (autoplay, tap-to-play)
- [ ] **Chat** : Synchronisation entre participants (actuellement local uniquement)

## Déploiement

Le fichier est déployé sur S3 et accessible via CloudFront :
- URL : `https://d3qqm87g3cjlxj.cloudfront.net/IVS-realtime-35-contributor.html`

## Stack technique

- Amazon IVS Web Broadcast SDK v1.24.0
- HTML/CSS/JavaScript vanilla
- API Gateway + Lambda pour la gestion des tokens

## Historique

- **v35** : Redesign complet UI/UX, fix mediaStreamTrack, fix autoplay iOS
- **v34** : Fusion viewer/contributor, VU-mètre
- **v33** : Thème toggle, chat panel
