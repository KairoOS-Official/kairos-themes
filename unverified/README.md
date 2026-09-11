# 🔴 Thèmes Non Vérifiés (Unverified)

> ⚠️ **Attention** : Ces thèmes n'ont PAS été validés par l'équipe KaïroOS. Installez-les à vos propres risques.

---

## 📦 Comment ça marche ?

Les thèmes non vérifiés sont des créations communautaires qui n'ont pas passé le processus de validation officiel. Ils sont accessibles directement depuis KaïroOS via **l'installation par URL GitHub**.

### Sécurité

- Les thèmes ne contiennent que du CSS et des images
- Aucun code JavaScript ne s'exécute
- Les fichiers `theme.json` sont vérifiés avant injection CSS
- Possibilité de réinitialiser le thème avec la touche <kbd>Suppr</kbd>

---

## 🔍 Trouver des Thèmes Non Vérifiés

### Sources recommandées

1. **GitHub** : Cherchez des repos avec le topic `kairoos-theme`
2. **Discord** : Canal #community-themes
3. **GitHub Discussions** : [kairos-community](https://github.com/KairoOS-Official/kairos-community/discussions)

### Vérifier un thème avant installation

1. Consultez le `theme.json` : vérifiez les couleurs et le layout
2. Regardez la `preview.png` ou `preview.svg`
3. Vérifiez la réputation de l'auteur

---

## 🚀 Installer un Thème Non Vérifié

### Depuis KaïroOS

1. Ouvrez **Paramètres** → **Thèmes & Style**
2. Cliquez sur l'onglet **Non Vérifiés**
3. Collez l'URL du dépôt GitHub : `https://github.com/utilisateur/mon-theme`
4. Cliquez sur **Analyser**
5. Vérifiez les couleurs et le layout affichés
6. Cliquez sur **Installer**

### Structure du dépôt requis

```
mon-theme/
├── theme.json       ← obligatoire
├── preview.png      ← obligatoire (screenshot 16:9, ~600x340px)
└── assets/          ← optionnel
    ├── background.jpg
    └── logo.png
```

### Exemple de `theme.json`

```json
{
  "id": "mon-theme",
  "name": "Mon Super Thème",
  "author": "MonPseudo",
  "version": "1.0.0",
  "description": "Description claire",
  "theme_type": "unverified",
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

---

## 📤 Publier votre Thème

### Prérequis

1. Un dépôt GitHub public
2. Un fichier `theme.json` valide
3. Une image `preview.png` ou `preview.svg`

### Étapes

1. Créez votre dépôt GitHub
2. Ajoutez le topic `kairoos-theme` dans les settings du repo
3. Partagez l'URL :
   - **Discord** : canal #community-themes
   - **GitHub** : Discussion dans [kairos-community](https://github.com/KairoOS-Official/kairos-community/discussions)

### Faire valider votre thème

Si vous souhaitez que votre thème soit promu en **Community Vérifié** :

1. Fork `kairos-themes`
2. Ajoutez votre thème dans `community/{nom-theme}/`
3. Ouvrez une Pull Request
4. L'équipe valide et merge → votre thème devient officiellement communautaire

---

## 🎨 Créer un Thème

### Variables CSS disponibles

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

### Layouts disponibles

| `layout_type` | Description |
|---------------|-------------|
| `sidebar_grid` | Barre latérale + grille de cartes |
| `single_page_categories` | Plein écran rayonnages |
| `console_launcher` | Style console TV / Steam Big Picture |

> 📖 Consultez le guide complet dans [`THEME_GUIDE.md`](../THEME_GUIDE.md)

---

## ⚠️ Avertissements

- Les thèmes non vérifiés ne sont **pas supportés** par l'équipe KaïroOS
- En cas de problème, utilisez la touche <kbd>Suppr</kbd> pour réinitialiser
- Vérifiez toujours les couleurs avant installation
- Utilisez les thèmes non vérifiés uniquement à des fins d'évaluation

---

## 🔗 Liens

- [Guide officiel des thèmes](../THEME_GUIDE.md)
- [Thèmes officiels](../official/)
- [Thèmes communautaires vérifiés](../community/)
- [Discord](https://discord.gg/kairo-os)
