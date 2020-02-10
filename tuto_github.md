# TUTO: CRÉER UN NOUVEAU PROJET SUR GITHUB




- [1. Création du projet](#1-création-du-projet)
- [2. Création de l'environnement virtuel](#2-création-de-lenvironnement-virtuel)
- [3. Ouvrir son environnement virtuel](#3-ouvrir-son-environnement-virtuel)
- [4. Commiter](#4-commiter)
- [5. Autres commandes Bash](#5-autres-commandes-bash)


## 1. Création du projet
 **Etape 1** : Se rendre sur GitHub

 [Lien vers GitHub](https://github.com/)

 **Etape 2** : New Project

 * Dans le coin en haut à droite, appuyez sur le symbole "+"
 * Sélectionnez "New Repository"
 * Créer un dossier dans C: que nous noterons *project* ici
 * Dans ce dossier faire clique-droit puis *GitBash Here*
 * Un terminal de commande va alors s'ouvrir
 * Tapez les commandes suivantes, **en appuyant sur *Entrée* à chaque retour à la ligne pour exécuter celle-ci** :
 ```bash
 git init

 touch README.md #créer fichier vierge

 git add READ.md

 git commit -m "Desc" #"Desc" étant la description notre action 

 git remote add origin https://github.com/moncompte/myproject.gitgit #ce lien est celui qu'on trouve dans GitHub lorsque on à créer le new Repository

 git push -u origin master
 ```
 **Votre projet est maintenant crée sur GitHub, passons maintenant à la création de notre environnement virtuel**

 ---------

## 2. Création de l'environnement virtuel 

**Étape 1** : Ouvrir GitBash

* Se rendre dans C:/.../project
* Clic-Droit
* GitBash Here

**Étape 2** : Tapez les commandes suivantes (**Appuyez sur *Entrée* à chaque retour à la ligne pour l'exécuter**)

```bash
python -m venv nom_venv #création env virtuel nommé mon_venv

source nom_venv/Scripts/activate

pip install jupyterlab 

option pip install -r requirement.txt #OPTIONNEL
```

**Tout est prêt, il ne reste plus qu'à lancer l'environnement virtuel**

-------
 
## 3. Ouvrir son environnement virtuel


Comme dans l'étape 1 de la partie 2, il vous faut d'abord ouvrir GitBash.  

Une fois cette étape réalisée, tapez les lignes de commandes suivantes (***Entrée* à chaque retour à la ligne**) : 
```bash
source mon_venv/Scripts/activate

jupyter lab
 ```
**Un page Jupyter va alors s'ouvrir, dans laquelle vous pourrez taper votre code. Dernière étape, commiter!**

---

## 4. Commiter 

Afin d'enregistrer votre travail, il est essentiel d'apprendre à commiter, c'est à dire de sauvegarder sur GitHub avec une description.   

D'abord, il faut se rendre sur GitBash de la même manière que dans les deux parties précedentes.    

Notons *data_tc* les données que nous voulons commiter.  

Dans GitBash, tapons les commandes suivantes (***Entrée* à chaque retour à la ligne**) :

```bash
git add data_tc

git commit -m "Data added in the project "  #-m = pour écrire la description de ce qu'on vient de commiter

git push
```

**Voilà tout est prêt!**

---

## 5. Autres commandes Bash 

```bash
git status #voir les changements avant commit

git clone #pour cloner le projet

cd #descendre d'un étage dans l'arborescence

cd .. #remonter d'un étage dans l'arborescence 

ls #lister les éléments

ll #comme ls mais en mieux 

mkdir nom_directory #créer un directory nom_directory

rm nom_fichier #détruire un fichier nom_fichier

rm -rf nom_directory #détruire un directory nom_directory
```














