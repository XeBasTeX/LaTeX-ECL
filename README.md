# Paquet LaTeX de l'École centrale de Lyon

[![Faites-moi un don ici !](https://img.shields.io/badge/donate-paypal-46AFE0.svg)](https://www.paypal.me/bastienlaville)
![Numéro de la version](https://img.shields.io/github/release/XeBasTeX/LaTeX-ECL.svg)
![Dernière modification](https://img.shields.io/github/last-commit/XeBasTeX/LaTeX-ECL.svg)
![Licence MIT](https://img.shields.io/github/license/XeBasTeX/LaTeX-ECL.svg)
![Langage du projet](https://img.shields.io/github/languages/code-size/XeBasTeX/LaTeX-ECL.svg)

<div align="center">
  <img title="Logo du paquet centrale.sty" alt= "Logo du paquet LaTeX centrale.sty" src="eps/centrale_sty_logo.png">
</div>

-----------------

## Installation

### Pour utiliser le rapport et le paquet

Télécharger le dossier, le placer dans le sous-dossier de votre choix et modifier uniquement le fichier ```rapport.tex```. Vous pouvez retirer le fichier ```README.md``` et le fichier de licence.

### Pour utiliser seulement le paquet

Copier le fichier ```centrale.sty``` dans le répertoire de votre propre rapport et utiliser le dans le code de votre fichier ```tex``` avec la commande suivante, à insérer dans le préambule :
```latex
\usepackage{centrale}
```

## Commandes utiles

### Actions basiques

- Pour insérer une image : utiliser la commande fournie en exemple dans le rapport, modifier la taille de l'image avec *width = ...* soit par exemple *width=1\textwidth*
```latex
\begin{figure}[ht!]
    \centering
    \includegraphics[width=1\textwidth]{example-image-a}
    \caption{Insérer ici le sous-titre.}
    \label{fig:id-de-la-figure}
\end{figure}
```

- Pour insérer du code : soit avec ```listing``` soit avec ```minted```. Attention : pour utiliser ```minted``` il vous faudra soit utiliser *Overleaf* (qui est très permissif niveau compilation), soit compiler ```pdflatex``` avec l'option ```--shell-escape```. Reportez-vous à la doc de votre éditeur LaTeX pour plus d'informations ;

- Pour faire référence à une figure : utiliser ```\reff{fig:id-de-la-figure}```

- Pour faire référence à une référence bibliographique ```\citee{fig:id-de-la-ref}```

- Pour taper bêtement un nombre : vous pouvez le faire normalement comme 123, ou utiliser la commande ```\num{nombre}``` comme ```\num{2e-6}```

- Pour taper des quantités physiques : utiliser la commande ```\SI{nombre}{unités}```, par exemple comme ```e = \SI{1e-2}{m.kg^2/s}```

### Macros

- ```\subt{texte en dessous}``` permet d'écrire proprement un indice de notation (donc pas une variable). Par exemple T_c signifie << température chaude >>, c n'est pas une variable mais bien l'abréviation de chaud. Il faut donc noter ```T\sub{c}```

- ```\supt{texte au dessus}``` permet d'écrire de la même façon un indice supérieur : filtre non-causal ```W\sub{nc}```

- ```\ud``` permet d'écrire proprement une différentielle (avec une espace avant le d), par exemple dans une intégrale : ```\int f(x) \ud x```

- ```\derd{f}{x}``` permet de taper la dérivée droite de la fonction ```f``` par rapport à ```x```

- ```\derp{f}{x}``` permet de taper la dérivée partielle de la fonction ```f``` par rapport à ```x```

- les opérateurs différentiels tels que rot ou div sont disponibles. Notez que ces commandes sont compatibles avec le paquet ```physics```.

## Ressources utiles (et pour aller plus loin)

- un peu de typographie française ;
- 10 règles fondamentales en LaTeX disponible [ici](https://faculty.math.illinois.edu/~hildebr/tex/tips-topten.html)

## Comment contribuer ?

- contactez-moi pour devenir un collaborateur du projet, notamment sur la branche *dev* ;
- vous pouvez m'envoyer vos suggestions ou modifications à mon adresse mail, disponible sur [mon site Web](https://www-sop.inria.fr/members/Bastien.Laville/) ou par DM Facebook.

## Crédits

Le paquet a été réalisé au cours de l'année 2017 à partir de plusieurs paquets d'anciens élèves et des feuilles de style d'autres écoles.
Je tiens à remercier en particulier, par ordre chronologique de contributions dans le projet :
- Nicolas Gameiro (E2017) dont la première feuille de style a fourni une excellente base pour la suite ;
- Gauthier Fanucci (E2013) dont le rapport de PAr a permis de tirer quelques *features* intéressantes ;
- l'équipe de la PAO mandat 2019 - 2020 et plus spécialement Yann Zerrouk, Olivia Jeanne et Blaise Le Coquil (E2018) pour leurs chtites contributions ;
- les bêta-testeurs du code, à savoir personne.

## À propos de l'auteur

Bastien Laville, ancien étudiant à l'ECL (2017E, diplômé 2020). Je ne contribue plus au projet, vous pouvez cependant m'écrire un mail pour récupérer mon paquet Inria.

## Distribution et licence

Licence [MIT](https://choosealicense.com/licenses/mit/) - Bastien
