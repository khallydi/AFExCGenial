# AFE x CGénial : L'apprentissage automatisé

Ce GitHub a été crée dans le cadre de l'initiative *Professeurs en Entreprise* avec la fondation CGénial. Ce notebook est destiné aux enseignants sur la thématique de l'apprentissage automatisé (en anglais **Machine Learning**). 

Nous utilisons la librairie AutoGluon qui permet d'automatiser les tâches de machine learning, de tester plusieurs algorithmes et d'avoir l'algorithme le plus performant : https://auto.gluon.ai/stable/index.html

Dans cet exemple, nous estimons si la personne va acheter ou non le produit présenté en publicité. Nous avons à disposition le dataset "Social_Network_Ads.csv".

## Comment utiliser ce répertoire ?

Il suffit de git clone le répertoire dans un outil IDE tel que Amazon Sagemaker Studio Lab. 
Sur Amazon Sagemaker Studio Lab, il suffit de créer un compte pour avoir accès à un environnement virtuel avec tout le nécessaire pour lancer le notebook.
Dès que vous avez accès à l'environement, vous pouvez ouvrir un terminal et lancer le clonage du projet.

```bash
git clone https://github.com/khallydi/AFExCGenial.git
```

## Installation

Certains packages doivent être installés avant l'utilisation de ce notebook. Vous pouvez directement le 
faire depuis le notebook : 

```bash
!pip install -U pip
!pip install -U setuptools wheel
!pip install -U "mxnet<2.0.0"
!pip3 install --pre autogluon
!pip3 install seaborn
```

## Comment réutiliser le code avec un autre dataset (ici tabulaire) ?

Il suffit d'importer la donnée tabulaire dans le même répertoire que le fichier AFExCgenial.ipynb et de ne pas lancer cette partie du notebook : 

```bash

url = 'https://raw.githubusercontent.com/khallydi/AFExCGenial/main/Social_Network_Ads.csv'
r = requests.get(url, allow_redirects=True)

open('Social_Network_Ads.csv', 'wb').write(r.content)
```

