# Paquet LaTeX de l'École centrale de Lyon

[![](https://img.shields.io/badge/donate-paypal-46AFE0.svg)](https://www.paypal.me/bastienlaville)
![](https://img.shields.io/github/release-pre/XeBasTeX/LaTeX-ECL.svg)
![](https://img.shields.io/github/license/XeBasTeX/LaTeX-ECL.svg)
![](https://img.shields.io/github/languages/code-size/XeBasTeX/LaTeX-ECL.svg)

Correctifs à apporter :
- terminer le setup du siunitx, clarifier l'usage ;
- faire un environnement pour les parties particulières du rapport (e.g. la page résumé) ;
- faire une documentation ;
- mettre en ordre le code par section (EN COURS).

## Installation

Télécharger le dossier, le placer dans le sous-dossier de votre choix et modifier uniquement le fichier ```rapport.tex```. Vous pouvez retirer le fichier ```README.md``` et le fichier de license.

## Commandes utiles

### Opérations basiques

- Pour insérer une image : utiliser la commande fournie en exemple dans le rapport :
```latex
\begin{figure}[ht!]
    \centering
    \includegraphics[width=0.3\textwidth]{example-image-a}
    \caption{Insérer ici le sous-titre.}
    \label{fig:id-de-la-figure}
\end{figure}
```

- Pour insérer du code : soit avec ```listing``` soit avec ```minted```

- Pour taper des quantités physiques : utiliser la commande ```\SI{nombre}{unités}```, par exemple comme ``` e = \SI{10}{m.kg^2/s}```

### Macros

```\ud``` permet d'écrire propement une différentielle dans une intégrale, par exemple ```\int f(x) \ud x```

```\derd{f}{x}``` permet de taper une dérivée droite de la fonction ```f```par rapport à ```x```

```\derp{f}{x}``` permet de taper une dérivée partielle de la fonction ```f```par rapport à ```x```

## Comment contribuer ?

Vous pouvez m'envoyer vos suggestions à mon adresse centralienne, en me cherchant depuis l'annuaire de Zimbra.

## Crédits

Je tiens à remercier en particulier :
- Hachtung, dont la première feuille de style a fourni une excellente base pour la suite ;
- Govi dont le rapport de PAr a permis de tirer quelques *features* intéressantes ;
- les bêta-testeurs du code, à savoir personne.

## À propos des auteurs

Bastien Laville dit le Makzer (président de la PAO mandat 2018 - 2019)

## Distribution et license

MIT © Bastien Laville
