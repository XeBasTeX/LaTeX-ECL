# Paquet LaTeX de l'École centrale de Lyon

[![](https://img.shields.io/badge/donate-paypal-46AFE0.svg)](https://www.paypal.me/bastienlaville)
![](https://img.shields.io/github/release-pre/XeBasTeX/LaTeX-ECL.svg)
![](https://img.shields.io/github/last-commit/XeBasTeX/LaTeX-ECL.svg)
![](https://img.shields.io/github/license/XeBasTeX/LaTeX-ECL.svg)
![](https://img.shields.io/github/languages/code-size/XeBasTeX/LaTeX-ECL.svg)

<div align="center">
  <img src="https://www.ec-lyon.fr/sites/default/files/legacy-files/logo_quadri.jpg">
</div>

-----------------

## Installation

### Pour utiliser le rapport et le paquet

Télécharger le dossier, le placer dans le sous-dossier de votre choix et modifier uniquement le fichier ```rapport.tex```. Vous pouvez retirer le fichier ```README.md``` et le fichier de license.

### Pour utiliser seulement le paquet

Copier le fichier ```centrale.sty``` dans le répertoire de votre propre rapport et utiliser dans le code de votre propre rapport la commande suivante :
```latex
\usepackage{centrale}
```

## Commandes utiles

### Opérations basiques

- Pour insérer une image : utiliser la commande fournie en exemple dans le rapport :
```latex
\begin{figure}[ht!]
    \centering
    \includegraphics[width=1\textwidth]{example-image-a}
    \caption{Insérer ici le sous-titre.}
    \label{fig:id-de-la-figure}
\end{figure}
```

- Pour insérer du code : soit avec ```listing``` soit avec ```minted```

- Pour faire référence à une figure : utiliser ```\reff{fig:id-de-la-figure}```

- Pour faire référence à une référence bibliographique ```\citee{fig:id-de-la-ref}```

- Pour taper bêtement un nombre : vous pouvez le faire normalement ou utiliser la commande ```\num{nombre}``` comme ```\num{2e-6}```

- Pour taper des quantités physiques : utiliser la commande ```\SI{nombre}{unités}```, par exemple comme ``` e = \SI{1e-2}{m.kg^2/s}```

### Macros

```\subt{texte en dessous}``` permet d'écrire proprement un indice de notation (donc pas une variable). Par exemple T_c signifie << température chaude >>, c n'est pas une variable mais bien l'abréviation de chaud. Il faut donc noter ```T\sub{c}```

```\supt{texte au dessus}``` permet d'écrire de la même façon un indice supérieur : filtre non-causal ```W\sub{nc}```

```\ud``` permet d'écrire proprement une différentielle, par exemple dans une intégrale : ```\int f(x) \ud x```

```\derd{f}{x}``` permet de taper la dérivée droite de la fonction ```f``` par rapport à ```x```

```\derp{f}{x}``` permet de taper la dérivée partielle de la fonction ```f``` par rapport à ```x```

## Comment contribuer ?

- Contactez-moi pour devenir un contributeur du projet, notamment sur la branche *dev* ;
- Vous pouvez m'envoyer vos suggestions à mon adresse centralienne, en me cherchant depuis l'annuaire de Zimbra.

## Crédits

Je tiens à remercier en particulier, par ordre chornologique de contributions dans le projet :
- Nicolas Gameiro dont la première feuille de style a fourni une excellente base pour la suite ;
- Gauthier Fanucci dont le rapport de PAr a permis de tirer quelques *features* intéressantes ;
- l'équipe de la PAO mandat 2019 - 2020 et plus spécialement Yann Zerrouk, Olivia Jeanne et Blaise (chais-pas-ton-nom déso) pour ses chtites contributions
- les bêta-testeurs du code, à savoir personne.

## À propos des auteurs

Bastien Laville dit le Makzer (président de la PAO mandat 2018 - 2019) en 2A à l'ECL

## Distribution et license

Licence MIT © Bastien Laville
