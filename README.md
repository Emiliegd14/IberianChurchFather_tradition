# IberianChurchFather_tradition

Ce projet vise à utiliser des méthodes computationnelles pour estimer modéliser le processus de transmission textuelle des textes des Pères de l'Eglise du IIIe au Ve siècles en péninsule Ibérique. 
Ces analyses sont menées dans le cadre d'un Master en "Humanités Numériques" à l'École Nationale des Chartes-PSL.

## Ouvrage de Référence

**CORPUS CHRISTIANORUM, Traditio Patrum : scriptores hispanae, tome I, Turnhout, 2015.**

## Méthodes Employées

- Applications de modèles d'espèces invisibles : estimateurs de richesse et indicateurs de diversité.
- Modèles stochastiques de naissance-mort : modèles de Poisson, modèle de Yule, inférence bayésienne.
- 
### Description des données

- **wits_table_tot.csv**  
  Ce fichier est un jeu de données complet qui rassemble l’ensemble des témoins et manuscrits recensés pour chaque texte. Il contient également plusieurs métadonnées importantes, telles que la datation, la foliation, les informations sur le manuscrit, la date de l’auteur, etc. Ce tableau permet d’avoir une vue d’ensemble structurée sur les différentes sources textuelles et leurs caractéristiques.

- **corpus_stemmata**  
  Ce dossier contient deux sous-dossiers principaux :  
  - **stemmata_modified**  
  - **stemmata_nomodified**  
  
  Chacun de ces sous-dossiers regroupe des dossiers dédiés à chaque auteur. Ces dossiers comprennent plusieurs fichiers relatifs aux stemmata :  
  - Des métadonnées au format `.txt` décrivant les stemmata  
  - Les stemmata représentés au format `.gv` (Graphviz), permettant de visualiser la structure des arbres de transmission  
  - Les stemmata sous format `.png`, images des graphes pour une consultation rapide et visuelle  


## Premières analyses exploratoires des données

Cette analyse est structurée autour de trois notebooks Jupyter :

- `loi_puissance.ipynb`
- `stemmata_analysis.ipynb`
- `traitement_doublons.ipynb` 

Chaque notebook s'appuie sur des bibliothèques Python spécifiques, listées dans deux fichiers `requirements`.

### Dépendances

- Pour le notebook `stemmata_analysis.ipynb` :  
  → Utiliser les dépendances listées dans `requirements_stemmata.txt`.

- Pour les notebooks `loi_puissance.ipynb` et `traitement_doublons.ipynb` :  
  → Utiliser les dépendances listées dans `requirements_donnees.txt`.

### Installation et étapes

Il est recommandé d’utiliser un environnement virtuel (`venv` ou `conda`) pour isoler les dépendances.

```bash
# Pour exécuter le notebook stemmata_analysis.ipynb
pip install -r requirements_stemmata.txt

# Pour exécuter les notebooks loi_puissance.ipynb et traitement_doublons.ipynb
pip install -r requirements_donnees.txt
```


## Modélisation probabiliste avec le modèle des espèces non-vues

Cette méthode s’appuie sur l’article de référence :  
*"Forgotten Books: The Application of Unseen Species Models to the Survival of Culture"* (2021)  
par Mike Kestemont, Folgert Karsdorp, Elisabeth de Bruijn, Matthew Driscoll, Katarzyna A. Kapitan, Pádraig Ó Macháin, Daniel Sawyer, Remco Sleiderink & Anne Chao.

### Dépôts GitHub associés :  
- [forgotten-books](https://github.com/mikekestemont/forgotten-books)  
- [copia](https://github.com/mikekestemont/copia)

## Installation et étapes

**Copia** est un logiciel distribué sous forme de module Python.  
Pour l’installer, il suffit d’exécuter la commande `pip install` et d’installer les dépendances listées dans le fichier `requirements_copia.txt`, situé dans le dossier `unseen_species` de ce dépôt.


```bash
pip install copia
pip install -r unseen_species/requirements_copia.txt
```

## Modélisation stochastique de processus de naissance et de mort

Cette méthode s’appuie sur l'article de référence :  
CAMPS (Jean-Baptiste), CHRISTENSEN (Kelly), GODREAU (Ulysse) et MOINS (Théo), « One Tree
to Yule Them All ? reflexions on intertextuality and text transmission », École nationale
des chartes, Université PSL (, 2024), Preprint or working paper.

### Dépôt GitHub associé :  
- https://github.com/LostMa-ERC/simMAtree

## Installation et étapes

Certains prérequis sont nécessaires :
- Python 3.8+
- `git`
- Un environnement virtuel (optionnel mais vivement recommandé!)


```bash
# Cloner le dépôt
git clone https://github.com/LostMa-ERC/simMAtree.git

# Aller dans le dossier du projet
cd simMAtree

# Installer le package localement
pip install .



