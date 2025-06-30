# IberianChurchFather_tradition

Ce projet vise à utiliser des méthodes computationnelles pour estimer les taux de perte et de survie des œuvres et des manuscrits des Pères de l'Église de la péninsule ibérique, couvrant la période du IVe au VIe siècle.

## Ouvrage de Référence

**CORPUS CHRISTIANORUM, Traditio Patrum : scriptores hispanae, tome I, Turnhout, 2015.**

## Méthodes Employées

- Applications de modèles d'espèces invisibles : estimateurs de richesse (Chao1, Jackknife, ACE)
- 
## Contexte de l'Étude

Ces analyses sont menées dans le cadre d'un Master en "Humanités Numériques" à l'École Nationale des Chartes-PSL.

## Méthode 1 : Modélisation probabiliste avec le modèle des espèces non-vues

Cette méthode s’appuie sur l’article de référence :  
*"Forgotten Books: The Application of Unseen Species Models to the Survival of Culture"* (2021)  
par Mike Kestemont, Folgert Karsdorp, Elisabeth de Bruijn, Matthew Driscoll, Katarzyna A. Kapitan, Pádraig Ó Macháin, Daniel Sawyer, Remco Sleiderink & Anne Chao.

### Dépôts GitHub associés :  
- [forgotten-books](https://github.com/mikekestemont/forgotten-books)  
- [copia](https://github.com/mikekestemont/copia)

## Installation

**Copia** est un logiciel distribué sous forme de module Python.  
Pour l’installer, il suffit d’exécuter la commande `pip install` et d’installer les dépendances listées dans le fichier `requirements_copia.txt`, situé dans le dossier `unseen_species` de ce dépôt.

### Étapes :

```bash
pip install copia
pip install -r unseen_species/requirements_copia.txt



