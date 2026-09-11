# 🎨 KaïroOS Themes Store

Dépôt officiel des thèmes communautaires pour **KaïroOS** — le frontend d'arcade moderne et 100% personnalisable.

Ce dépôt alimente directement l'onglet **Store de Thèmes** dans KaïroOS via l'API GitHub. Tout thème soumis et mergé ici devient instantanément disponible en téléchargement en un clic pour tous les utilisateurs !

---

## 📦 Comment ça marche ?

### Thèmes Officiels

Les thèmes officiels sont développés par l'équipe KaïroOS et livrés avec l'application. Ils se trouvent dans le dépôt principal [`KairoOS-Official/KairoOS`](https://github.com/KairoOS-Official/KairoOS) dans le dossier `themes/` :

| Thème | Description | Layout |
|-------|-------------|--------|
| **kairo-default** | Style arcade classique années 80, palette claire | Sidebar + grille |
| **kairo-hub** | Interface plein écran catégories sans barre latérale | Rayonnages horizontaux |
| **kairo-console** | Style console TV / Steam Big Picture | Hero + carrousel |

### Thèmes Communautaires

Les thèmes de la communauté sont hébergés ici et accessibles directement depuis l'application via le **Community Store**.

---

## 🚀 Installer un Thème

### Depuis l'application (recommandé)

1. Ouvrez **Paramètres** → **Thèmes & Style**
2. Cliquez sur l'onglet **Store & En ligne**
3. Parcourez les thèmes disponibles et cliquez sur **Télécharger**
4. Le thème est installé automatiquement !

### Manuellement

Copiez le dossier du thème dans :
- **Mode portable** : `builds/portable/themes/`
- **Mode installé** : `%APPDATA%\kairo-os\themes/`

---

## 🎨 Créer un Thème

### Structure

```
mon-theme/
├── theme.json        ← Métadonnées, couleurs, polices (obligatoire)
├── preview.svg       ← Aperçu du thème (recommandé)
└── assets/           ← Images, sons (optionnel)
```

### Spécification `theme.json`

```json
{
  "id": "mon-theme",
  "name": "Mon Super Thème",
  "author": "VotrePseudo",
  "version": "1.0.0",
  "description": "Description pour le store.",
  "theme_type": "community",
  "colors": {
    "bg_primary": "#0b0f19",
    "bg_secondary": "#111827",
    "bg_card": "#1e293b",
    "accent_primary": "#f43f5e",
    "text_primary": "#f8fafc"
  },
  "fonts": {
    "primary": "Outfit, system-ui, sans-serif",
    "arcade": "Press Start 2P"
  }
}
```

> 📖 Consultez le guide complet dans [`THEME_GUIDE.md`](THEME_GUIDE.md) pour la spécification détaillée.

---

## 📤 Contribuer

### Via Pull Request (recommandé)

1. **Forkez** ce dépôt
2. Créez une branche : `git checkout -b theme/mon-nouveau-theme`
3. Ajoutez votre dossier de thème à la racine
4. Testez localement dans KaïroOS
5. Ouvrez une **Pull Request** avec une capture d'écran

### Soumettre sans GitHub

Envoyez votre `theme.json` et `preview.svg` via :
- **Discord** : canal #theme-submissions
- **Email** : themes@kairo-os.com

L'équipe ajoutera votre thème pour vous.

---

## ✅ Critères de Validation

Votre thème sera accepté si :

- [ ] `theme.json` est un JSON valide
- [ ] L'`id` est unique (pas de doublon avec un thème existant)
- [ ] Une image `preview.svg` ou `preview.png` est fournie
- [ ] La description est claire et concise
- [ ] Les couleurs sont lisibles (contraste suffisant)

---

## 📁 Structure du Dépôt

```
kairos-themes/
├── README.md              ← Ce fichier
├── THEME_GUIDE.md         ← Guide complet de création
└── <votre-theme>/         ← Votre contribution ici
```

> **Note** : Les thèmes officiels (`kairo-default`, `kairo-hub`, `kairo-console`) sont dans le dépôt principal [`KairoOS-Official/KairoOS`](https://github.com/KairoOS-Official/KairoOS), pas ici.

---

## 🔗 Liens Utiles

- [Site officiel](https://kairo-os.com)
- [Dépôt principal](https://github.com/KairoOS-Official/KairoOS)
- [Discord](https://discord.gg/kairo-os)
- [Guide des thèmes](THEME_GUIDE.md)

---

Fait avec ❤️ par la communauté KaïroOS.
