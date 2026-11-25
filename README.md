# Tournoi Futsal — gestion et co-évaluation

Application web mono-fichier (`index.html`) pour un tournoi de foot en salle à 4 équipes : chrono, scores, classement, finales et co-évaluation des élèves (barème additif de 4 à 6).

## Utilisation
- **Enseignant** : « Nouvelle session » génère un code à 4 caractères. Garder cet écran ouvert pendant la séance (il fait office de serveur).
- **Observateurs** : ouvrent le lien copié (« Copier lien élèves ») ou saisissent le code, puis cochent Cardio / Technique / Gentleman pour chaque joueur.
- **Export** : notes finales en CSV (compatible Excel).

## Barème
4.0 de base, +0.5 cardio, +0.5 technique, +0.5 gentleman / auto-arbitrage, +0.5 capitaine (validé par l'enseignant), malus enseignant. Maximum 6.0.

## Technique
Pas de compte ni de clé : la synchronisation entre téléphones utilise WebRTC (PeerJS, broker public gratuit). Les données restent en localStorage sur l'appareil de l'enseignant. Fonctionne sur GitHub Pages (HTTPS requis).
