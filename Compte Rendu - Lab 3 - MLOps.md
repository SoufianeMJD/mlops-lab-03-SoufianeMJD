# Compte Rendu - Lab 3 - MLOps

Soufiane MAJDALANE

# **Versionnement des données et pipelines ML avec DVC**

### **Étape 1 : Initialisation de DVC dans le projet**

**initialisation de DVC**

![image.png](image.png)

![image.png](image%201.png)

### **Étape 2 : Versionner les données brutes avec DVC**

**Apres session deuppr data/ de votre .gitignore, on ajoute le dataset au suivi DVC**

![image.png](image%202.png)

**Ajoute au versionnement Git :**

![image.png](image%203.png)

### **Étape 3 : Configuration d’un remote DVC**

![image.png](image%204.png)

**Déclaration comme remote principal**

![image.png](image%205.png)

**Versionne la config :**

![image.png](image%206.png)

### **Étape 4 : Push des données dans le remote DVC**

![image.png](image%207.png)

### **Étape 5 : imulation d’une collaboration : supprimer localement et récupérer depuis DVC**

**Suppression du dataset local :**

![image.png](image%208.png)

**Récupèration du dataset via DVC :**

![image.png](image%209.png)

### **Étape 6 : Création d’un pipeline reproductible dvc.yaml**

On a versionné les données transformées et les statistiques d’entraînement avec DVC, en les liant à un commit Git précis.

![image.png](image%2010.png)

Remove the file from Git's index

![image.png](image%2011.png)

![image.png](image%2012.png)

![image.png](image%2013.png)

![image.png](image%2014.png)

**Création d’un pipeline :**

![image.png](image%2015.png)

**Ajoute l'étape d’entraînement :**

![image.png](image%2016.png)

**Evaluation du model :**

![image.png](image%2017.png)

![image.png](image%2018.png)

![image.png](image%2019.png)

### **Étape 7 : Reproduire automatiquement tout le pipeline**

![image.png](image%2020.png)