# DEMO CICD

## Les principes de base

Pour déployer les applications, on utilise les GitHub actions.

Les GitHub actions sont des workflows qui permettent d'effectuer des actions en automatique sur un repository.

Tous les workflows doivent être définis dans le répertoire .github/workflows

Chaque workflow est représenté par un fichier *.yml. 
Chaque workflow est constitué de JOB qui sont eux même constitués de STEP

![cicd_1.png](docs/pictures/cicd_1.png)

Les workflows vont être déclanchés par des actions pré-définies.
Par défaut, tous les job d'un workflow vont être lancés en parallèle. 
Et dans un job, tous les steps vont être lancés sussessivement.
Dans un même workflow, il sera possible d'attendre la fin d'un job pour en déclencher un autre. 
Mais cela devra être précisé dans la déclaration.

## Mon 1er workflow
Le workflow ci-dessous possède de 2 types de déclencheurs
Il possède 1 job et utilise dans son 1er step une action pré-définie.

![cicd_2.png](docs/pictures/cicd_2.png)

## Travailler avec des variabes

![cicd_3.png](docs/pictures/cicd_3.png)

## Creer des workflow réutilisables

![cicd_4.png](docs/pictures/cicd_4.png)



