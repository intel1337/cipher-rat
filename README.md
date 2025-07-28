# Cipher-RAT

**Cipher-RAT** est un projet de Remote Access Tool (RAT) éducatif et multi-modules développé avec Python, JavaScript (Electron/React), et des outils de visualisation modernes. Il comprend une interface graphique, une interface web et des fonctions d'interaction temps réel avec des clients infectés.

---

## 📁 Structure du projet

```
cipher-rat/
├── cipher/                 # Code principal du RAT (backend Python)
│   ├── App.py              # Point d'entrée principal
│   ├── server.py           # Serveur de gestion des clients
│   ├── zombie.py           # Gestion des clients ("zombies")
│   ├── tkmsg.py            # Interface tkinter pour les messages
│   ├── utils.py            # Fonctions utilitaires
│   ├── password.py         # Extraction/gestion de mots de passe
│   ├── config.py           # Configuration statique
│   └── assets/             # Ressources : screamer audio, screenshot
│
├── electron_overlay/       # Overlay Electron déclenchant des actions (ex: screamer)
│   ├── main.js             # Processus principal Electron
│   ├── index.html          # Interface visuelle
│
├── web-dashboard/          # Dashboard web (React / Next.js)
│   └── src/app/            # Structure React typique avec plusieurs pages
│       ├── dashboard/
│       ├── devices/
│       ├── monitor/
│       └── realtime/
│
├── setup.bat               # Script de configuration rapide Windows
├── requirements.txt        # Dépendances Python
├── commandes.txt           # Liste de commandes RAT
└── README.md               # Ce fichier
```

---

## ⚙️ Fonctionnalités

- 📡 Command & Control (serveur Python)
- 🪟 Interface tkinter pour interaction manuelle
- 🧠 Dashboard React pour surveillance centralisée
- 💀 Screamer audio + overlay visuel (Electron)
- 🧪 Extraction de mots de passe
- 🖥️ Capture d’écran
- 💬 Envoi de messages en direct
- 🔐 Obfuscation partielle du code

---

## 🚀 Installation

### Python backend

```bash
cd cipher
pip install -r requirements.txt
python App.py
```

### Dashboard Web (React)

```bash
cd web-dashboard
npm install
npm run dev
```

### Overlay Electron

```bash
cd electron_overlay
npm install
npm start
```

---

## ⚠️ Avertissement

> Ce projet est destiné à des fins **éducatives uniquement**. Toute utilisation abusive, malveillante ou sans le consentement explicite des parties concernées est strictement interdite.

---

## 📄 Licence

Aucune licence déclarée (assumez usage restreint et privé). Ajoutez une licence open source si vous souhaitez le distribuer.

---

## 👨‍💻 Auteur

Projet par **intel1337**  
GitHub : [intel1337/cipher-rat](https://github.com/intel1337/cipher-rat)