# MIZEN SUITE — Site Web

**L'ERP qui équilibre votre production.**

Site web vitrine pour MIZEN SUITE, organisé autour du principe d'équilibre entre charge d'atelier, coût de revient et délai client.

## Structure

```
mizen-suite-website/
├── index.html       # Page unique (HTML + CSS + JS inline)
└── img/             # Toutes les images du site
    ├── transparent-MIZEN-logo.png
    ├── sofem-logo.png
    ├── login_logo.jpg
    ├── background_login_image.avif
    ├── clipper-pieces-cyclees-decolletage_jpg.webp
    ├── abas-erp-kennzahlen-laptop-dashboard-management_png.webp
    ├── proconcept_accompagnement_projet_jpg.webp
    ├── ow-book-a-demo-new_png.webp
    ├── 1782666633908_image.png
    ├── 1782666649478_image.png
    └── 1782666681277_image.png
```

## Lancer le site

Aucune installation requise. Ouvrez simplement `index.html` dans un navigateur :

- **Double-clic** sur `index.html`, ou
- **Serveur local** (recommandé) : `python3 -m http.server 8000` puis ouvrir `http://localhost:8000`

## Sections incluses

1. **Navigation** sticky avec logo et CTA "Demander une démo"
2. **Hero** avec balance animée en SVG (signature visuelle)
3. **Strip clients** avec SOFEM
4. **L'équilibre Mizen** — 3 piliers (Capacité / Coût / Délai)
5. **Fiche pièce cyclée** — showcase atelier
6. **Tableau de bord / Pilotage** — showcase KPI
7. **Modules** — 8 modules de la suite
8. **Portail de connexion** — preview du login
9. **Témoignage SOFEM**
10. **Galerie terrain**
11. **CTA démo**
12. **Footer**

## Technologies

- HTML5 / CSS3 (variables CSS, Grid, Flexbox)
- JavaScript vanilla (IntersectionObserver pour animations au scroll)
- Google Fonts : Fraunces (display) + Manrope (body)
- SVG animé pour la balance du hero
- 100% responsive (mobile / tablette / desktop)
- Respect de `prefers-reduced-motion`

## Personnalisation rapide

Toutes les couleurs sont définies en haut de `<style>` dans `index.html` :

```css
:root {
  --cream: #F7F3EC;
  --navy: #1C2330;
  --tan: #C99A66;
  --tan-dark: #9C6E3F;
  --sage: #3E6F61;
  ...
}
```

Changez ces variables pour ajuster la palette globale.

---

© 2026 MIZEN SUITE
