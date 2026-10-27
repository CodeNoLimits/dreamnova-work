# Portfolio DreamNova — travaux et prototypes

Page publique (noindex) : https://codenolimits.github.io/dreamnova-work/

- `index.html` : la page (aucune donnée en dur, tout vient de `works.json`).
- `works.json` : UNE entrée par prototype ou travail (`id`, `date`, `type`, `title`, `sector`, `region`, `link`, `media`, `poster`, `note`).
- `assets/media/` : vidéos ré-encodées (720p) et images.

## Ajouter une entrée (une ligne, publie et vérifie en ligne)

```bash
dn-portfolio-add --type reel --title "Launch reel (EN)" --sector "Dental clinic" --region "Austin, TX" --media ~/chemin/reel.mp4
```

Types : `voice`, `reel`, `video`, `demo`, `case`. `dn-portfolio-add --sync-war` ajoute les prototypes vocaux envoyés par la war-machine. `--dry-run` pour tester, `--list` pour lister.

## Règles

- Le dépôt est PUBLIC : jamais de nom de client ou de prospect, jamais de lien `/d/<slug>` nominatif, jamais de prix. Le script refuse ces cas.
- Texte de la page en anglais (prospects US/CA).
