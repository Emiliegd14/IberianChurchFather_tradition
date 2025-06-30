# IberianChurchFather_tradition

Ce projet vise à utiliser des méthodes computationnelles pour estimer les taux de perte et de survie des œuvres et des manuscrits des Pères de l'Église de la péninsule ibérique, couvrant la période du IVe au VIe siècle.

## Ouvrage de Référence

**CORPUS CHRISTIANORUM, Traditio Patrum : scriptores hispanae, tome I, Turnhout, 2015.**

## Méthodes Employées

- Applications de modèles d'espèces invisibles : estimateurs de richesse (Chao1, Jackknife, ACE)
- 
## Contexte de l'Étude

Ces analyses sont menées dans le cadre d'un Master en "Humanités Numériques" à l'École Nationale des Chartes-PSL.

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
```bash ... ```


## Premières analyses exploratoires des donnéesModélisation probabiliste avec le modèle des espèces non-vues

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
```bash ... ```


