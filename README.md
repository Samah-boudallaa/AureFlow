<div align="center">

<img src="assets/banner.svg" alt="AureFlow, par Samah Boudallaa" width="100%">

**Un espace d'étude pensé pour apprendre vite, retenir longtemps et arriver prêt le jour J.**

![Statut](https://img.shields.io/badge/statut-actif-4f46e5?style=flat-square)
![Stack](https://img.shields.io/badge/stack-HTML%20%7C%20CSS%20%7C%20JavaScript-0891b2?style=flat-square)
![Dépendances](https://img.shields.io/badge/d%C3%A9pendances-aucune-0f9d58?style=flat-square)
![Licence](https://img.shields.io/badge/licence-MIT-lightgrey?style=flat-square)

[Démo en ligne](https://samah-boudallaa.github.io/AureFlow/) · [Signaler un problème](../../issues) · [Proposer une idée](../../issues/new)

</div>

---

## Présentation

AureFlow rassemble, module par module, tout ce qu'il faut pour préparer une évaluation : synthèse de cours, fiches de mémorisation, exercices corrigés, outils interactifs et examens blancs chronométrés.

Chaque module est une application autonome : un seul fichier, sans installation, sans serveur, sans compte. On l'ouvre dans le navigateur et on travaille.

## Aperçu

**Tableau de bord**

![Tableau de bord](assets/tableau-de-bord.png)

**Entraînement avec correction immédiate**

![Entraînement](assets/entrainement.png)

**Examen blanc**

![Examen blanc](assets/examen-blanc.png)

## Modules

| Module | Contenu | Statut |
|---|---|---|
| Cloud & IoT | Cours, fiches, labo interactif, TD corrigés, banque de 64 questions, examens blancs | Disponible |

### Programme couvert

| Chapitre | Titre |
|---|---|
| Ch0 | Vue d’ensemble de l’IoT |
| Ch1 | Systèmes embarqués |
| Ch2 | Plateforme Arduino |
| Ch3 | Capteurs et actionneurs |
| Ch4 | ATmega328 et interruptions |

## Fonctionnalités

**Apprendre**
- Synthèse structurée par chapitre, avec recherche instantanée
- 22 fiches de mémorisation à retourner et un mémo des valeurs à connaître
- Laboratoire interactif : manipulation de bits, convertisseurs, calculs électriques

**S'entraîner**
- Banque de 64 questions classées en trois niveaux : facile, moyen, difficile
- Filtrage par chapitre et par niveau
- Correction immédiate avec explication
- Mode « Revoir mes erreurs » : les questions ratées reviennent jusqu'à être maîtrisées
- 10 exercices de travaux dirigés avec énoncé puis correction à ouvrir

**Se tester**
- Examens blancs en 5 formats, dont un examen complet de 20 questions en 20 minutes
- Chronomètre, aucune correction pendant l'épreuve, note sur 20
- Bilan par chapitre et liste des questions à revoir

**Suivre sa progression**
- Indice de préparation global
- Maîtrise par chapitre et recommandation du point faible à travailler
- Historique des notes d'examen

**Confort d'utilisation**
- Thème clair et sombre, qui suit par défaut le réglage de l’appareil
- Raccourcis clavier : `1` à `4` pour répondre, `Entrée` pour continuer
- Interface adaptée au téléphone, à la tablette et à l'ordinateur

## Démarrage rapide

```bash
git clone https://github.com/Samah-boudallaa/AureFlow.git
cd AureFlow
```

Ouvre ensuite `index.html` dans ton navigateur. C'est tout.

### Publier sur GitHub Pages

1. Va dans **Settings** puis **Pages**.
2. Choisis la branche `main` et le dossier `/ (root)`.
3. Enregistre. Le site est accessible à l'adresse `https://samah-boudallaa.github.io/AureFlow/`.

## Structure du dépôt

```text
AureFlow/
├── assets/
│   ├── banner.svg
│   ├── signature.svg
│   ├── tableau-de-bord.png
│   ├── entrainement.png
│   └── examen-blanc.png
├── index.html
├── README.md
└── LICENSE
```

## Respect de la vie privée

Aucune donnée n'est envoyée nulle part. La progression (réponses, scores, erreurs à revoir) est stockée uniquement dans le navigateur de l'utilisateur et peut être effacée en vidant les données du site.

## Ajouter ou modifier des questions

Les questions sont rangées dans un tableau JavaScript au début du fichier, une ligne par question :

```js
[niveau, chapitre, "Énoncé", ["A", "B", "C", "D"], indexBonneReponse, "Explication"]
```

- `niveau` : `0` facile, `1` moyen, `2` difficile
- `chapitre` : numéro du chapitre, de `0` à `4`
- `indexBonneReponse` : position de la bonne réponse, en partant de `0`

Ajoute toujours les nouvelles questions **à la fin** du tableau pour ne pas casser l'historique des erreurs enregistré.

## Feuille de route

- [x] Cours, fiches et mémo
- [x] Labo interactif
- [x] TD corrigés
- [x] Examens blancs chronométrés
- [ ] Mode sombre automatique selon l'heure
- [ ] Export de la progression
- [ ] Questions à réponses multiples
- [ ] Nouveaux modules

## Contribuer

Les suggestions sont bienvenues.

1. Fais un fork du dépôt.
2. Crée une branche : `git checkout -b ajout-questions`
3. Valide tes changements : `git commit -m "Ajout de questions sur le chapitre 4"`
4. Envoie la branche : `git push origin ajout-questions`
5. Ouvre une Pull Request.

## Auteure

**Samah Boudallaa** · [Profil GitHub](https://github.com/Samah-boudallaa)

## Licence

Distribué sous licence MIT. Voir le fichier `LICENSE`.

<div align="center">

Fait avec soin pour réussir ses évaluations.

<img src="assets/signature.svg" alt="Samah Boudallaa" width="420">

</div>
