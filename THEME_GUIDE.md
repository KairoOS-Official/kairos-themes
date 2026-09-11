# Theme Guide — KairoOS

## Structure obligatoire

```
yourname-themename/
  theme.json    ← obligatoire
  preview.png   ← obligatoire (min 800x450px, screenshot de l'interface)
  README.md     ← obligatoire
  assets/       ← optionnel (fonts, images de fond, sons)
```

## theme.json minimum

```json
{
  "id": "yourname-themename",
  "name": "My Theme",
  "version": "1.0.0",
  "author": "yourname",
  "type": "community",
  "description": "What it looks like",
  "colors": {
    "bg_primary": "#ffffff",
    "bg_secondary": "#f5f5f5",
    "bg_card": "#ffffff",
    "sidebar_bg": "#eeeeee",
    "accent_primary": "#e63950",
    "accent_secondary": "#f5a623",
    "text_primary": "#1a1a2e",
    "text_secondary": "#666666",
    "text_muted": "#999999",
    "border": "#dddddd",
    "success": "#28a745",
    "warning": "#ffc107",
    "danger": "#dc3545"
  },
  "fonts": {
    "primary": "Inter",
    "arcade": "Press Start 2P",
    "size_base": "14px"
  },
  "layout": {
    "card_radius": "12px",
    "sidebar_width": "260px",
    "card_gap": "16px"
  },
  "assets": {
    "background_image": null,
    "logo_override": null,
    "startup_sound": null
  }
}
```

## Règles

- Préfixe obligatoire : `pseudo-nom`
- preview.png obligatoire — screenshot réel de KairoOS avec le thème appliqué
- Zéro asset protégé par copyright (fonts, images)

## Publier

Dépose dans `community/` et push directement.

## Signaler un thème

Ouvre une issue avec le template "Report a theme".
