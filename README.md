# Cours intensif Handicap, autonomie et travail social — 8 séances

Livre académique Quarto avec slides reveal.js. 3 ECTS · 16h présentiel + 60h travail personnel.

## Formats disponibles

- HTML book (navigation web)
- PDF (impression)
- EPUB (liseuse)
- Slides reveal.js (un jeu par séance)

## Construire localement

```bash
./quarto render          # HTML + PDF + EPUB
for n in 01 02 03 04 05 06 07 08; do
  ./quarto render slides/${n}-slides.qmd --to revealjs
done
mkdir -p _site/slides && cp slides/*.html _site/slides/
```

## Publier

```bash
git push   # CI Actions déploie sur GitHub Pages
```

## Licence

CC BY-NC-SA 4.0
