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

A lightweight, secure, and interactive web application for peer-to-peer (P2P) file transfers between phones and computers. Built with a modern UI, smooth animations, and a dark/light theme. No files are stored on a server.

## 🔗 Live Demo
👉 **[Visit the page](https://bstudio136.github.io/TransfertP2P/)** *(Update this link once GitHub Pages is active)*

## ✨ Features

- **100% Peer-to-Peer**: Files travel directly from one device to another using WebRTC. No server storage.
- **Secure**: The communication channel is encrypted with DTLS, and files are verified using SHA-256 hashes.
- **Manual Mode**: Exchange pairing codes manually (via SMS, messaging apps, etc.) without using a signaling server.
- **Dark/Light Theme**: Toggle between modes with a dedicated button. The choice is saved in the browser's `localStorage`.
- **Multi-language**: Interface available in French, English, Italian, and Turkish.
- **Transfer Progress**: Real-time tracking of speed, size, percentage, and estimated time remaining.
- **Cancel & Resume**: Cancel a transfer in progress, or resume a transfer if the connection drops.
- **Drag & Drop**: Easily send files by dragging and dropping them into the window.
- **100% Responsive**: Adapts perfectly to mobile, tablet, and desktop screens.

## 🛠️ Tech Stack

- **HTML5**: Semantic structure.
- **CSS3**: CSS Variables, Flexbox, CSS Grid, Animations (`@keyframes`), Glassmorphism effects.
- **JavaScript (Vanilla)**: WebRTC API, File API, Clipboard API, and i18n management.
- **Signaling**: Uses `ntfy.sh` by default for pairing, with a fallback to manual code exchange.
- **Network**: STUN/TURN servers (Google, openrelay.metered.ca) to traverse NATs.

## 🚀 Installation & Usage

This project is a simple static file (HTML/CSS/JS). To run it locally:

1. Clone the repository:
   git clone https://github.com/Bstudio136/TransfertP2P.git
2. Open the `index.html` file in your browser.
3. That's it! No dependencies or build necessary.

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

Une application web légère, sécurisée et interactive pour transférer des fichiers directement d'un appareil à un autre (Peer-to-Peer) entre téléphones et ordinateurs. Conçue avec une interface moderne, des animations fluides et un thème sombre/clair. Aucun fichier n'est stocké sur un serveur.

## 🔗 Démo en direct
👉 **[Visiter la page](https://bstudio136.github.io/TransfertP2P/)** *(À mettre à jour une fois GitHub Pages activé)*

## ✨ Fonctionnalités

- **100% Pair-à-Pair** : Les fichiers voyagent directement entre les appareils via WebRTC. Aucun stockage sur serveur.
- **Sécurisé** : Le canal de communication est chiffré avec DTLS, et les fichiers sont vérifiés par empreinte SHA-256.
- **Mode Manuel** : Possibilité d'échanger les codes d'appairage à la main (via SMS, messagerie, etc.) sans utiliser de serveur de signalisation.
- **Thème Sombre/Clair** : Basculez entre les modes avec un bouton dédié. Le choix est sauvegardé dans le `localStorage` du navigateur.
- **Multilingue** : Interface disponible en Français, Anglais, Italien et Turc.
- **Progression en temps réel** : Suivi de la vitesse, de la taille, du pourcentage et du temps restant estimé.
- **Annulation & Reprise** : Annulez un transfert en cours, ou reprenez un transfert si la connexion a été coupée.
- **Glisser-Déposer** : Envoyez facilement des fichiers en les glissant-déposant dans la fenêtre.
- **100% Responsive** : S'adapte parfaitement aux mobiles, tablettes et ordinateurs.

## 🛠️ Technologies Utilisées

- **HTML5** : Structure sémantique.
- **CSS3** : Variables CSS, Flexbox, CSS Grid, Animations (`@keyframes`), effets de verre (Glassmorphism).
- **JavaScript (Vanilla)** : API WebRTC, API File, API Clipboard, et gestion de l'i18n (multilingue).
- **Signalisation** : Utilise `ntfy.sh` par défaut pour l'appairage, avec un mode de secours par échange manuel de codes.
- **Réseau** : Serveurs STUN/TURN (Google, openrelay.metered.ca) pour traverser les NAT.

## 🚀 Installation & Utilisation

Ce projet est un simple fichier statique (HTML/CSS/JS). Pour le faire fonctionner localement :

1. Clonez le dépôt :
   git clone https://github.com/Bstudio136/TransfertP2P.git
2. Ouvrez le fichier `index.html` dans votre navigateur.
3. C'est tout ! Aucune dépendance ou build n'est nécessaire.

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
