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

1. **Navigation** sticky avec logo, lien Connexion, CTA "Demander une démo" et **menu mobile (hamburger)**
2. **Hero** avec balance animée en SVG (signature visuelle) et **compteurs animés**
3. **Strip clients** avec SOFEM
4. **L'équilibre Mizen** — 3 piliers (Capacité / Coût / Délai)
5. **Atelier connecté (MES)** — suivi machine, OEE en direct, ordonnancement, traçabilité, terminal, qualité, alertes, GMAO
6. **Fiche pièce cyclée** — showcase atelier
7. **Tableau de bord / Pilotage** — showcase KPI
8. **Modules** — 12 modules de la suite (ERP + MES)
9. **Intégrations** — comptabilité, CAO/FAO, machines CN, Power BI, API REST…
10. **Portail de connexion** — preview du login
11. **Tarifs / Éditions** — Atelier / Suite / Entreprise
12. **Témoignage SOFEM**
13. **FAQ** — accordéon (6 questions)
14. **Galerie terrain**
15. **CTA + formulaire de démo** (validation côté client)
16. **Footer** étendu (liens, réseaux sociaux)
17. **Bouton retour en haut**

## Améliorations techniques

- **SEO** : meta description, Open Graph, Twitter Cards, canonical, favicon, données structurées JSON-LD (`SoftwareApplication`)
- **Accessibilité** : skip link, `aria-*` sur menu/FAQ, focus visible, `role="img"` sur le SVG
- **Navigation active** au scroll (IntersectionObserver)
- **Animations** respectant `prefers-reduced-motion`

> Le formulaire de démo valide les champs côté client et affiche une confirmation.
> Il n'est pas encore relié à un backend — brancher l'envoi (e-mail / CRM / API) dans `index.html` (`#demoForm`).

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
