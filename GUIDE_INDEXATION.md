# 📋 GUIDE D'INDEXATION SEO
## Portfolio — Aurras Charnel KOUGBE ZOGAN
---

## 📁 Fichiers livrés

| Fichier | Rôle |
|---|---|
| `portfolio.html` | Site principal (déjà optimisé) |
| `robots.txt` | Instructions pour les crawlers |
| `sitemap.xml` | Plan du site pour Google/Bing |
| `manifest.json` | PWA + identité du site |
| `seo_head_block.html` | Bloc `<head>` SEO complet à intégrer |

---

## ✅ ÉTAPE 1 — Mettre en ligne

Déploie sur un hébergeur avec un **domaine propre** :
- GitHub Pages : `charnscode.github.io` (gratuit)
- Netlify / Vercel (gratuit, HTTPS automatique)
- Hostinger / Infomaniak (payant, domaine `.dev` ou `.com`)

> ⚠️ **Remplace `https://charnscode.dev/`** dans `robots.txt`, `sitemap.xml` et
> `seo_head_block.html` par ton vrai domaine avant de déployer.

Structure de dossier attendue :
```
/
├── portfolio.html   (renommer en index.html)
├── robots.txt
├── sitemap.xml
├── manifest.json
├── M.jpeg
├── 1.jpeg … 8.jpeg
├── projet1a.jpg … projet6b.jpg
├── CV_Aurras_Charnel.pdf
└── icons/
    ├── icon-72.png
    ├── icon-96.png
    ├── icon-128.png
    ├── icon-192.png
    └── icon-512.png
```

> 📌 Renomme `portfolio.html` → **`index.html`** pour qu'il soit la page d'accueil.

---

## ✅ ÉTAPE 2 — Intégrer le bloc SEO dans index.html

Ouvre `index.html`, **remplace** l'ancien `<head>...</head>` par le contenu
de `seo_head_block.html`.

Assure-toi que ces 3 lignes sont présentes juste avant `</head>` :
```html
<link rel="stylesheet" href="style.css">
<script src="https://kit.fontawesome.com/a2e0f6ad4c.js" crossorigin="anonymous"></script>
<link rel="manifest" href="manifest.json">
```

---

## ✅ ÉTAPE 3 — Créer les icônes PWA

Va sur **https://realfavicongenerator.net** ou **https://favicon.io** :
1. Upload ta photo `M.jpeg`
2. Génère le pack d'icônes
3. Place les fichiers dans le dossier `icons/`

---

## ✅ ÉTAPE 4 — Soumettre à Google Search Console

1. Va sur https://search.google.com/search-console
2. Clique **"Ajouter une propriété"** → colle ton URL
3. Vérifie la propriété (méthode HTML tag ou DNS)
4. Va dans **Sitemaps** → colle `https://ton-domaine.com/sitemap.xml`
5. Clique **Soumettre**

> Google indexe généralement en 24–72h.

---

## ✅ ÉTAPE 5 — Soumettre à Bing Webmaster

1. Va sur https://www.bing.com/webmasters
2. Importe depuis Google Search Console (1 clic)
3. Ou ajoute manuellement et soumets le sitemap

---

## ✅ ÉTAPE 6 — Vérifications finales

Lance ces outils de validation avant soumission :

| Outil | URL | Vérifie |
|---|---|---|
| Rich Results Test | https://search.google.com/test/rich-results | JSON-LD Schema |
| Open Graph Debugger | https://developers.facebook.com/tools/debug/ | Partages réseaux sociaux |
| Twitter Card Validator | https://cards-dev.twitter.com/validator | Preview Twitter |
| PageSpeed Insights | https://pagespeed.web.dev | Performance (viser 90+) |
| Mobile Friendly Test | https://search.google.com/test/mobile-friendly | Responsive |

---

## 🔑 Mots-clés ciblés

```
Aurras Charnel KOUGBE ZOGAN
développeur web Bénin
cybersécurité Bénin
portfolio développeur Cotonou
full-stack developer Benin
Google Cybersecurity Certificate
INE Bénin hydrogéologie
Django React developer Africa
```

---

## 📌 Notes importantes

- **HTTPS obligatoire** pour le PWA manifest et l'indexation optimale
- Les **ancres** (`#about`, `#projects`…) sont dans le sitemap pour aider Google
  à comprendre la structure single-page
- Le **JSON-LD** (`@type: Person`) permet d'apparaître dans les **Knowledge Panels** Google
- Le **hreflang** FR/EN indique à Google les deux versions linguistiques
- Mets à jour `lastmod` dans `sitemap.xml` à chaque modification du portfolio

---

*Généré le 2025-06-07 — charnokgb@gmail.com*
