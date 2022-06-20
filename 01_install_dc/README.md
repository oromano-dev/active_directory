# 01 Installation du controleur de domaine (DC)

1. Utiliser `scconfig` pour:
    - Changer le nom de l'ordinateur
    - Définir une adresse IP statitque
    - Changer le serveur DNS et mettre l'adresse du serveur 

2. Installer les fonctionnalités Active Directory

```` Shell
Install-windowsfeature AD-Domain-Services -IncludemanagementTools 
````

3. Installer la forêt Active Directory

```` Shell
Import-Module ADDSDeployment
Install-ADDSForest
````