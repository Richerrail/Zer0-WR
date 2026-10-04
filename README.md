# Zer0-WR

Lecteur de web-radio cyber-futuriste, simple et léger, conçu pour lire des flux audio directement dans le navigateur.

## 🎯 Fonctionnalités

- **Interface Cyber/Futuriste** : Design moderne avec thème sombre par défaut
- **Sélection intuitive** : Playlist de stations avec navigation clavier et souris
- **Lecteur Audio HTML5** : Lecture fluide de flux audio en direct
- **Gestion personnalisée** : Ajout, modification et suppression de radios
- **Visualiseur animé** : Barres EQ dynamiques lors de la lecture
- **Contrôle de volume** : Slider interactif avec ajustement au clavier
- **Stockage persistant** : Vos stations sont sauvegardées automatiquement
- **Import/Export** : Sauvegardez et restaurez vos playlists en JSON
- **30+ stations RADIOBOB!** : Collection de radios Metal et Rock préconfigurées
- **Accessibilité** : Support complet du clavier et des lecteurs d'écran
- **Mode clair/sombre** : Suit les préférences du système
- **Aucune dépendance externe** : Pur HTML/CSS/JavaScript

## ⌨️ Raccourcis Clavier

| Touche | Action |
|--------|--------|
| **Espace** | Lecture/Pause |
| **Flèches Haut/Bas** | Navigation stations |
| **Flèches Gauche/Droite** | Navigation stations |
| **M** | Sourdine/Volume |
| **E** | Ajouter une station |

## 🚀 Prérequis

- Un navigateur web moderne (Chrome, Firefox, Safari, Edge)
- Accès à des flux audio (URL de type MP3, AAC, Ogg, etc.)

## 📦 Installation et Utilisation

### Option 1 : Clonage local
```bash
git clone https://github.com/Richerrail/Zer0-WR.git
cd Zer0-WR
# Ouvrez index.html dans votre navigateur
```

### Option 2 : Utilisation directe en ligne
Consultez la version hébergée et ouvrez le fichier directement.

## 🎮 Guide d'Utilisation

### Lire une radio
1. Sélectionnez une station dans la liste **PLAYLIST**
2. Cliquez sur le **gros bouton rond** ou appuyez sur **Espace**
3. Ajustez le volume avec le slider ou les flèches clavier

### Ajouter une station
1. Cliquez sur le bouton **+ (plus)** dans l'interface
2. Entrez :
   - **NOM** : Nom de la radio
   - **URL** : Lien du flux audio (ex: `https://stream.example.com/live.mp3`)
   - **GENRE** : Catégorie (optionnel)
3. Cliquez **AJOUTER**

### Gérer votre playlist
- **Modifier** : Cliquez l'icône ✏️ sur une station
- **Supprimer** : Cliquez l'icône 🗑️ sur une station
- **Importer** : Importez une playlist en JSON depuis Firefox DevTools
- **Exporter** : Copiez votre playlist en JSON ou téléchargez-la
- **Réinitialiser** : Supprimez toutes les stations et revenez aux defaults

## 💾 Import/Export

### Exporter vos stations
1. Cliquez **EXPORT** dans le footer
2. La playlist est copiée en JSON ou téléchargée

### Importer une playlist
1. Récupérez le JSON des stations (depuis Firefox ou un export antérieur)
2. Cliquez **IMPORT** et collez le JSON
3. Validez avec **IMPORTER**

## 📁 Structure du projet

```
Zer0-WR/
├── index.html       # Fichier principal (HTML + CSS + JS intégré)
├── README.md        # Documentation
└── LICENSE          # Licence MIT
```

## 🎨 Personnalisation

### Stations par défaut
Les 30 stations RADIOBOB! sont intégrées et se chargent automatiquement au premier lancement. Modifiez la constante `DEFAULT_STATIONS` (ligne ~320) pour ajouter vos propres stations par défaut.

### Thème
Modifiez les variables CSS `:root` (lignes 11-16) pour personnaliser les couleurs :
- `--bg` : Couleur de fond
- `--accent` : Couleur primaire
- `--danger`, `--warn` : Couleurs secondaires

## 🔧 Maintenance Console

Pour debug, accédez depuis la console :
```javascript
ZER0WR.stations()   // Voir la liste des stations
ZER0WR.export()     // Exporter les stations
ZER0WR.import(json) // Importer des stations
ZER0WR.play()       // Lancer la lecture
ZER0WR.pause()      // Pause la lecture
```

## 📝 Version

**ZERØ WR v2.0**
- Design cyber-futuriste complet
- Accessibilité renforcée
- Support stockage local
- Import/Export JSON
- Visualiseur animé

## 📄 Licence

Ce projet est distribué sous la licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

**Crédits**  
Données radio : [RADIOBOB!](https://www.radiobob.de/)
