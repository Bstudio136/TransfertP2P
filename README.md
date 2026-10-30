# Transfert P2P 📱➡️📱

Une application web légère et sécurisée pour transférer des fichiers directement d'un appareil à un autre (Peer-to-Peer), sans passer par un serveur de stockage.

## ✨ Fonctionnalités

*   **100% Pair-à-Pair** : Les fichiers voyagent directement entre les téléphones via WebRTC.
*   **Sécurisé** : Le canal de communication est chiffré avec DTLS.
*   **Aucun stockage** : Aucun fichier n'est sauvegardé sur un serveur.
*   **Mode Manuel** : Possibilité d'échanger les codes d'appairage à la main (via SMS, messagerie, etc.) sans utiliser de serveur de signalisation.
*   **Multilingue** : Interface disponible en Français, Anglais, Italien et Turc.
*   **Thème clair / sombre** : S'adapte aux préférences de l'utilisateur.
*   **Progression en temps réel** : Suivi de la vitesse, de la taille et de l'état des transferts.

## 🚀 Comment l'utiliser ?

Puisqu'il s'agit d'un fichier unique (HTML/CSS/JS), vous pouvez :
1. Télécharger le fichier et l'ouvrir directement dans votre navigateur.
2. Ou utiliser la version hébergée sur **GitHub Pages** (voir ci-dessous).

### Utilisation
1. Ouvrez l'application sur les deux appareils.
2. Sur l'appareil A, cliquez sur **"Envoyer des fichiers"**. Un code à 6 chiffres s'affiche.
3. Sur l'appareil B, cliquez sur **"Recevoir des fichiers"** et entrez le code.
4. Glissez-déposez ou sélectionnez vos fichiers pour commencer le transfert !

## 🛠️ Technologies utilisées

*   HTML5 / CSS3 / Vanilla JavaScript
*   WebRTC (API de communication en temps réel)
*   ntfy.sh (pour la signalisation par défaut)
*   openrelay.metered.ca (Serveur TURN pour traverser les NAT stricts)

## 📄 Licence

Ce projet est sous licence MIT.
