# 📖 Carnet de Cuisine — Livre de recettes HTML

Un carnet de recettes de cuisine présenté comme un **livre relié**, entièrement en HTML/CSS statique. Aucune dépendance, aucun framework — juste un fichier à ouvrir dans un navigateur.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Licence MIT](https://img.shields.io/badge/licence-MIT-green?style=flat)

---

## ✨ Aperçu

> Une présentation élégante, style éditorial, inspirée des livres de cuisine imprimés.

- 📚 **Couverture** sombre avec titre calligraphié et ornements dorés
- 🗂️ **Sommaire interactif** avec navigation par clic
- 🍽️ **Fiches recettes** structurées : ingrédients, étapes numérotées, astuces du chef
- 🖨️ Pensé pour l'impression et la lecture en ligne

---

## 📁 Structure du projet

```
carnet-de-cuisine/
├── livre_recettes.html   # Fichier principal — tout-en-un
├── README.md
└── LICENSE
```

Le projet est volontairement **mono-fichier** : HTML, CSS et JavaScript sont regroupés dans `livre_recettes.html` pour une portabilité maximale.

---

## 🚀 Utilisation

### Ouvrir localement

```bash
# Cloner le dépôt
git clone https://github.com/votre-utilisateur/carnet-de-cuisine.git

# Ouvrir dans le navigateur
open livre_recettes.html
# ou double-cliquer sur le fichier
```

Aucune installation requise.

### Publier sur GitHub Pages

1. Aller dans **Settings → Pages** du dépôt
2. Sélectionner la branche `main` et le dossier racine `/`
3. Renommer `livre_recettes.html` en `index.html`
4. Le livre est accessible à `https://votre-utilisateur.github.io/carnet-de-cuisine/`

---

## 🍴 Recettes incluses

| # | Recette | Catégorie | Durée |
|---|---------|-----------|-------|
| 1 | Lentilles au saumon, sauce moutarde aux herbes | Salade | 40 min |
| 2 | Soupe de légumes d'hiver au gingembre | Soupe | 50 min |
| 3 | Poulet rôti aux herbes, citron confit & ail doux | Plat | 1h30 |
| 4 | Tarte aux pommes rustique, cannelle & beurre salé | Dessert | 1h |

---

## ➕ Ajouter une recette

Copier le bloc suivant dans `livre_recettes.html`, après la dernière `<div class="recipe-page">`, et adapter le contenu :

```html
<div class="recipe-page" id="recetteN">
  <div class="recipe-header">
    <div class="recipe-header-left">
      <div class="recipe-num">0N</div>
      <div class="recipe-category">Catégorie</div>
      <h2 class="recipe-title">Titre de la recette</h2>
      <p class="recipe-subtitle">Sous-titre ou variante</p>
    </div>
  </div>
  <div class="recipe-meta">
    <div class="meta-item"><span class="meta-label">Préparation</span><span class="meta-value">XX min</span></div>
    <div class="meta-item"><span class="meta-label">Cuisson</span><span class="meta-value">XX min</span></div>
    <div class="meta-item"><span class="meta-label">Personnes</span><span class="meta-value">X</span></div>
    <div class="meta-item"><span class="meta-label">Difficulté</span><span class="meta-value">Facile</span></div>
  </div>
  <div class="recipe-divider"></div>
  <div class="columns">
    <!-- ingrédients et étapes ici -->
  </div>
</div>
```

Penser aussi à ajouter l'entrée correspondante dans le **sommaire** (`<ul class="toc-list">`).

---

## 🎨 Personnalisation

Les couleurs principales sont définies en variables CSS au début du fichier :

```css
:root {
  --cream: #f5f0e8;       /* fond des pages */
  --warm-brown: #3d2b1a;  /* couverture & titres */
  --olive: #5c6b3a;       /* accents verts */
  --rust: #9b4521;        /* labels & catégories */
  --gold: #c9a84c;        /* ornements dorés */
}
```

Les polices utilisées proviennent de **Google Fonts** :
- `Playfair Display` — titres
- `Cormorant Garamond` — corps de texte
- `Libre Baskerville` — labels & métadonnées

---

## 🤝 Contribuer

Les contributions sont les bienvenues ! Pour proposer une recette ou une amélioration :

1. Forker le dépôt
2. Créer une branche (`git checkout -b ajout/ma-recette`)
3. Committer les modifications (`git commit -m "Ajout : tarte tatin"`)
4. Ouvrir une Pull Request

---

## 📄 Licence

Ce projet est distribué sous licence **MIT**. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
