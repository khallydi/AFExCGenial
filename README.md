# AFE x CGénial : L'apprentissage automatisé
Ce Github a été crée dans le cadre de la présentation chez Cgénial destinée aux enseignants sur la thématique de 
l'apprentissage automatisé (en anglais Machine Learning). 


Nous utilisons la librairie AutoGluon qui permet 
d'automatiser les tâches de machine learning, de tester plusieurs algorithmes et d'avoir l'algorithme le plus 
performant : https://auto.gluon.ai/stable/index.html

Dans cet exemple, nous estimons si la personne va acheter ou non le produit présenté en publicité. Nous avons à disposition le dataset "Social_Network_Ads.csv".

## Installation
Certains packages doivent être installés avant l'utilisation de la librairie AutoGluon. Vous pouvez directement le 
faire depuis le notebook. 

```bash
!pip install -U pip
!pip install -U setuptools wheel
!pip install -U "mxnet<2.0.0"
!pip3 install --pre autogluon
!pip3 install seaborn
```
    
