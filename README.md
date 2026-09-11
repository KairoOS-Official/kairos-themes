# 🎨 KaïroOS Themes Store

Dépôt officiel des thèmes pour **KaïroOS** — le frontend d'arcade moderne et 100% personnalisable.

---

## 📦 Système de Thèmes

### Vue d'ensemble

| Catégorie | Badge | Source | Installation | Validation |
|-----------|-------|--------|--------------|------------|
| **Officiels** | 🟢 OFFICIEL | `official/` | 1 clic | Équipe KaïroOS |
| **Communauté** | 🟡 COMMUNAUTÉ | `community/` | 1 clic | PR validée |
| **Non Vérifiés** | 🔴 NON VÉRIFIÉ | URL GitHub | Manuel | Aucune |

### Thèmes Officiels

Les thèmes officiels sont développés et maintenus par l'équipe KaïroOS.

| Thème | Description | Layout |
|-------|-------------|--------|
| **kairo-default** | Style arcade classique années 80 | Sidebar + grille |
| **kairo-hub** | Interface plein écran catégories | Rayonnages horizontaux |
| **kairo-console** | Style console TV / Steam Big Picture | Hero + carrousel |

### Thèmes Communauté Vérifiés

Les thèmes communautaires ont été validés par l'équipe via une Pull Request.

→ Consultez le dossier [`community/`](community/)

### Thèmes Non Vérifiés

Les thèmes non vérifiés sont des créations communautaires non validées. Ils sont installables via une URL GitHub.

→ Consultez le dossier [`unverified/`](unverified/)

---

## 🚀 Installer un Thème

### Depuis l'application (recommandé)

1. Ouvrez **Paramètres** → **Thèmes & Style**
2. Choisissez l'onglet correspondant :
   - **Thèmes** : thèmes installés
   - **Store** : thèmes officiels et communautaires
   - **Non Vérifiés** : thèmes par URL GitHub
3. Cliquez sur **Appliquer**

### Installer un thème non vérifié

1. Ouvrez l'onglet **Non Vérifiés**
2. Collez l'URL du dépôt GitHub
3. Vérifiez les couleurs et le layout affichés
4. Cliquez sur **Appliquer**

---

## 🎨 Créer un Thème

### Structure

```
mon-theme/
├── theme.json       ← obligatoire
├── preview.png      ← obligatoire (screenshot 16:9)
└── assets/          ← optionnel
```

### Spécification `theme.json`

```json
{
  "id": "mon-theme",
  "name": "Mon Super Thème",
  "author": "VotrePseudo",
  "version": "1.0.0",
  "description": "Description claire du thème.",
  "theme_type": "community",
  "colors": {
    "bg_primary": "#0b0f19",
    "bg_secondary": "#111827",
    "bg_card": "#1e293b",
    "sidebar_bg": "#0f172a",
    "accent_primary": "#f43f5e",
    "accent_secondary": "#38bdf8",
    "text_primary": "#f8fafc",
    "text_secondary": "#94a3b8",
    "text_muted": "#64748b",
    "border": "#334155",
    "success": "#10b981",
    "warning": "#f59e0b",
    "danger": "#ef4444"
  },
  "fonts": {
    "primary": "Outfit, system-ui, sans-serif",
    "arcade": "Press Start 2P",
    "size_base": "14px"
  },
  "layout": {
    "card_radius": "16px",
    "sidebar_width": "280px",
    "card_gap": "16px"
  }
}
```

> 📖 Consultez le guide complet dans [`THEME_GUIDE.md`](THEME_GUIDE.md)

### Variables CSS

| Variable | Description |
|----------|-------------|
| `--bg-primary` | Fond général |
| `--bg-secondary` | Fond alternatif |
| `--bg-card` | Fond des cartes |
| `--sidebar-bg` | Fond de la barre latérale |
| `--accent-primary` | Couleur d'accentuation principale |
| `--accent-secondary` | Couleur d'accentuation secondaire |
| `--text-primary` | Texte principal |
| `--text-secondary` | Texte secondaire |
| `--text-muted` | Texte discret |
| `--border-color` | Bordures |
| `--color-success` | Succès |
| `--color-warning` | Avertissement |
| `--color-danger` | Danger |

### Layouts

| `layout_type` | Description |
|---------------|-------------|
| `sidebar_grid` | Barre latérale + grille de cartes |
| `single_page_categories` | Plein écran rayonnages |
| `console_launcher` | Style console TV / Steam Big Picture |

---

## 📤 Contribuer

### Pour les thèmes vérifiés (recommandé)

1. **Forkez** ce dépôt
2. Ajoutez votre thème dans `community/{nom-theme}/`
3. Ouvrez une **Pull Request**
4. L'équipe valide et merge

### Pour les thèmes non vérifiés (rapide)

1. Créez un dépôt GitHub avec `theme.json` + `preview.png`
2. Ajoutez le topic `kairoos-theme` dans les settings
3. Partagez l'URL sur Discord ou GitHub Discussions
4. Les utilisateurs installent depuis l'app via l'URL

---

## ✅ Critères de Validation

Votre thème sera accepté si :

- [ ] `theme.json` est un JSON valide
- [ ] L'`id` est unique
- [ ] Une image `preview.png` ou `preview.svg` est fournie
- [ ] La description est claire
- [ ] Les couleurs sont lisibles (contraste suffisant)

---

## 🆘 Raccourci d'Urgence

Si un thème casse l'affichage :
- Appuyez sur la touche <kbd>Suppr</kbd> (ou <kbd>Del</kbd>)
- KaïroOS réapplique instantanément le thème officiel `kairo-default`

---

## 📁 Structure du Dépôt

```
kairos-themes/
├── README.md              ← Ce fichier
├── THEME_GUIDE.md         ← Guide complet
├── official/              ← Thèmes officiels KaïroOS
├── community/             ← Thèmes vérifiés (PR)
└── unverified/            ← Guide thèmes non vérifiés
```

---

## 🔗 Liens

- [Dépôt principal](https://github.com/KairoOS-Official/KairoOS)
- [Discord](https://discord.gg/kairo-os)
- [Guide des thèmes](THEME_GUIDE.md)
- [Thèmes non vérifiés](unverified/)

---

Fait avec ❤️ par la communauté KaïroOS.
