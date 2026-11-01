<div align="center">
  <h3>🌍 Choose your language / Choisissez votre langue</h3>
  <a href="#english">🇬🇧 English</a> | <a href="#francais">🇫🇷 Français</a>
</div>

---

<div id="english"></div>
🇬🇧<br>
# 🌟 Transfert P2P | Bstudio136

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=for-the-badge&logo=webrtc&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-121013?style=for-the-badge&logo=github&logoColor=white)

A lightweight web application for peer-to-peer (P2P) file transfers between phones and computers. The file data is sent over a DTLS-encrypted WebRTC channel and is not stored by the signaling service. WebRTC may use a TURN relay when a direct network path is unavailable.

## 🔗 Live Demo
👉 **[Visit the live page](https://bstudio136.github.io/TransfertP2P/)**

## ✨ Features

- **WebRTC transfers**: Files travel over an encrypted WebRTC data channel. A TURN relay may carry encrypted traffic when a direct path is unavailable; files are not stored by the signaling service.
- **Secure Pairing**: Uses a cryptographically secure 6-digit random code. The pairing code expires after 5 minutes.
- **Device Verification (SAS)**: After connecting, a Short Authentication String (SAS) is generated from the DTLS fingerprints of both devices. Users must visually compare this 6-digit security code shown on both screens and confirm they match to unlock the transfer. This prevents Man-in-the-Middle (MITM) attacks.
- **Integrity check**: Transfer data is checked with a chunked SHA-256 fingerprint to ensure the file arrives exactly as sent.
- **Manual Mode**: Exchange WebRTC offer/answer data manually without using `ntfy.sh` for signaling.
- **QR pairing**: Scan a temporary pairing link with the device camera.
- **Dark/Light Theme**: Toggle between modes with a dedicated button. The choice is saved in the browser's `localStorage`.
- **Multi-language**: Interface available in French, English, Italian, and Turkish.
- **Transfer Progress**: Real-time tracking of speed, size, percentage, and an approximate remaining time.
- **Cancel & Resume**: Cancel an outgoing file. If a connection drops, re-pair in the same open page and reselect the same file to continue from the received chunks held in memory.
- **Drag & Drop**: Easily send files by dragging and dropping them into the window.
- **Responsive and accessible controls**: Adapts to mobile, tablet, and desktop; supports visible keyboard focus and reduced motion.

## 🛠️ Tech Stack

- **HTML5**: Semantic structure.
- **CSS3**: CSS Variables, Flexbox, Animations (`@keyframes`), Glassmorphism effects.
- **JavaScript (Vanilla)**: WebRTC API, File API, Clipboard API, Web Crypto API (for SAS generation), and i18n management.
- **Signaling**: Uses the public `ntfy.sh` service by default for pairing messages, with a manual exchange mode.
- **Network**: Uses public STUN/TURN endpoints (Google and Open Relay) to traverse NATs. These are community services, not a reliability guarantee.
- **QR libraries**: Loaded from jsDelivr when the page opens. Pairing and transfer do not depend on QR scanning.

## 🚀 Installation & Usage

This project is a static HTML/CSS/JS page. Use GitHub Pages or serve it from `localhost` so secure-context browser APIs such as Web Crypto and camera access are available:

1. Clone the repository:
   git clone https://github.com/Bstudio136/TransfertP2P.git
2. Serve the folder locally (for example with `python -m http.server`) and open `http://localhost:8000`.
3. No build step is required. The QR libraries are fetched from jsDelivr at runtime.

### Current limitations

- Received file chunks are kept in browser memory until the page is closed. Very large files can exceed a phone or browser's available memory.
- Resume only works while the receiving page remains open. It is not persisted across reloads or browser restarts.
- Automatic signaling sends WebRTC connection metadata through the public `ntfy.sh` service. Use manual mode if you do not want to use that signaling service.

## 🎨 Customization

To adapt this page to your own needs:

1. **Colors**: Modify the CSS variables in `:root` to change the theme colors (e.g., `--accent: #f5b915;` for gold).
2. **Signaling Server**: If you want to use your own server instead of `ntfy.sh`, modify the `NTFY` constant in the JavaScript.
3. **TURN/STUN Servers**: Update the `ICE_CONFIG` object in the JavaScript to use your own TURN servers for better connection reliability.
4. **Languages**: Add or modify translations in the `I18N` object.

## 👨‍💻 Author

**Bstudio136**

- 🐙 GitHub : [@Bstudio136](https://github.com/Bstudio136)
- 🎵 TikTok : [@bstudio136](https://tiktok.com/@bstudio136)
- 🐦 Twitter / X : [@Bstudio136](https://x.com/Bstudio136)
- 📺 YouTube : [@Bstudio136](https://www.youtube.com/@Bstudio136)

## 📄 License

This project is under the MIT License. You are free to use and modify it for your own needs.

<a href="https://hiddenswap.com/pay/AgRPwfFe" target="_blank" rel="noopener"><img src="https://hiddenswap.com/pay/AgRPwfFe/button.svg" alt="Donate with any coin" width="247" height="44"></a>

---

<div id="francais"></div>
🇫🇷<br>
# 🌟 Transfert P2P | Bstudio136

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=for-the-badge&logo=webrtc&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-121013?style=for-the-badge&logo=github&logoColor=white)

Une application web légère pour transférer des fichiers entre téléphones et ordinateurs en pair-à-pair. Les données passent par un canal WebRTC chiffré avec DTLS et ne sont pas stockées par le service de signalisation. WebRTC peut utiliser un relais TURN si une connexion directe est impossible.

## 🔗 Démo en direct
👉 **[Visiter la page en ligne](https://bstudio136.github.io/TransfertP2P/)**

## ✨ Fonctionnalités

- **Transfert WebRTC** : Les fichiers passent par un canal WebRTC chiffré. Un relais TURN peut transporter le trafic chiffré si la connexion directe échoue ; le service de signalisation ne stocke pas les fichiers.
- **Appairage sécurisé** : Utilise un code aléatoire à 6 chiffres généré de manière cryptographiquement sûre. Le code expire après 5 minutes.
- **Vérification de l'appareil (SAS)** : Après la connexion, une chaîne d'authentification courte (SAS) est générée à partir des empreintes DTLS des deux appareils. Les utilisateurs doivent comparer visuellement ce code de sécurité à 6 chiffres affiché sur les deux écrans et confirmer qu'ils correspondent pour débloquer le transfert. Cela permet de prévenir les attaques de type homme du milieu (MITM).
- **Contrôle d'intégrité** : Les données sont contrôlées avec une empreinte SHA-256 par blocs pour s'assurer que le fichier arrive exactement tel qu'il a été envoyé.
- **Mode manuel** : Échange l'offre et la réponse WebRTC sans utiliser `ntfy.sh` pour la signalisation.
- **Appairage QR** : Scanne un lien temporaire avec la caméra de l'appareil.
- **Thème Sombre/Clair** : Basculez entre les modes avec un bouton dédié. Le choix est sauvegardé dans le `localStorage` du navigateur.
- **Multilingue** : Interface disponible en Français, Anglais, Italien et Turc.
- **Progression en temps réel** : Suivi de la vitesse, de la taille, du pourcentage et du temps restant approximatif.
- **Annulation & Reprise** : Annule un fichier en cours d'envoi. Après une coupure, refais l'appairage dans la même page ouverte et sélectionne le même fichier pour continuer depuis les blocs conservés en mémoire.
- **Glisser-Déposer** : Envoyez facilement des fichiers en les glissant-déposant dans la fenêtre.
- **Responsive et commandes accessibles** : S'adapte aux mobiles, tablettes et ordinateurs, avec focus clavier visible et réduction des animations.

## 🛠️ Technologies Utilisées

- **HTML5** : Structure sémantique.
- **CSS3** : Variables CSS, Flexbox, Animations (`@keyframes`), effets de verre (Glassmorphism).
- **JavaScript (Vanilla)** : API WebRTC, API File, API Clipboard, API Web Crypto (pour la génération du SAS) et gestion de l'i18n (multilingue).
- **Signalisation** : Utilise le service public `ntfy.sh` par défaut pour les messages d'appairage, et propose un échange manuel.
- **Réseau** : Utilise des serveurs STUN/TURN publics (Google et Open Relay), qui ne garantissent pas une disponibilité permanente.
- **Bibliothèques QR** : Chargées depuis jsDelivr. Le transfert et l'appairage manuel restent utilisables si le scan QR est indisponible.

## 🚀 Installation & Utilisation

Ce projet est une page statique HTML/CSS/JS. Utilise GitHub Pages ou un serveur local `localhost` afin que Web Crypto et l'accès caméra soient disponibles :

1. Clonez le dépôt :
   git clone https://github.com/Bstudio136/TransfertP2P.git
2. Lancez un serveur local (par exemple `python -m http.server`) et ouvrez `http://localhost:8000`.
3. Aucune compilation n'est nécessaire. Les bibliothèques QR sont chargées depuis jsDelivr à l'ouverture.

### Limites actuelles

- Les blocs reçus restent en mémoire dans le navigateur jusqu'à la fermeture de la page. Les fichiers très volumineux peuvent dépasser la mémoire disponible du téléphone ou du navigateur.
- La reprise fonctionne tant que la page de réception reste ouverte ; elle ne survit pas à un rechargement ou au redémarrage du navigateur.
- Le mode automatique transmet des métadonnées de connexion WebRTC au service public `ntfy.sh`. Utilise le mode manuel si tu ne veux pas utiliser ce service.

## 🎨 Personnalisation

Pour adapter cette page à vos propres besoins :

1. **Couleurs** : Modifiez les variables CSS dans `:root` pour changer les couleurs du thème (par exemple, `--accent: #f5b915;` pour l'or).
2. **Serveur de signalisation** : Si vous voulez utiliser votre propre serveur au lieu de `ntfy.sh`, modifiez la constante `NTFY` dans le JavaScript.
3. **Serveurs TURN/STUN** : Mettez à jour l'objet `ICE_CONFIG` dans le JavaScript pour utiliser vos propres serveurs TURN pour une meilleure fiabilité de connexion.
4. **Langues** : Ajoutez ou modifiez les traductions dans l'objet `I18N`.

## 👨‍💻 Auteur

**Bstudio136**

- 🐙 GitHub : [@Bstudio136](https://github.com/Bstudio136)
- 🎵 TikTok : [@bstudio136](https://tiktok.com/@bstudio136)
- 🐦 Twitter / X : [@Bstudio136](https://x.com/Bstudio136)
- 📺 YouTube : [@Bstudio136](https://www.youtube.com/@Bstudio136)

## 📄 Licence

Ce projet est sous licence MIT. Vous êtes libre de l'utiliser et de le modifier pour vos propres besoins.

<a href="https://hiddenswap.com/pay/AgRPwfFe" target="_blank" rel="noopener"><img src="https://hiddenswap.com/pay/AgRPwfFe/button.svg" alt="Donate with any coin" width="247" height="44"></a>
