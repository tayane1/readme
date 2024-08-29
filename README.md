Pour créer un projet django il faut suivre les étapes suivantes 👍

créer un dossier puis l'ouvrir dans un éditeur, puis une fois à l'interieur
il faut créer un environnement virtuel avec les commandes qui suit : 
Créer un environnement virtuel : python3 -m venv nom de l'environnement,
Activer l'environnement virtuel
Sous macOS et Linux : source myenv/bin/activate 
Sous Windows : myenv\Scripts\activate
Installer des dépendances : pip install requests
Figer les dépendances : pip freeze > requirements.txt

ensuite créé le projet django : 
Installation de Django : pip install django
Création d'un nouveau projet Django : django-admin startproject nom du projet

après Installation et création du projet Django, il faut crée les differentes applications
pour cela il faut se deplacer dans le dossier racine du projet Django
avec la commande cd nom du dossier, une fois a1 l'interieur faire la commande
django-admin startapp nom de l'application
se rendre dans le settings du projet Django precisement au niveau de installed apps
ajouter chaque nom des apps créees
il faut configurer les views de chaque application en créant nos differentes fonctions dont nous aurons besoins
dans chaque application créer un ficher urls.py qui nous aidera pour les chemins des differents templates de notre application en important nos fonctions créees dans les views
inclure les chemins des urls des applications dans l'urls du projet Django
créer un dossier templates à la racine du projet django pour tous les fichers html de nos applications
integrer le dossier templates au settings au niveau de templates avec la commande [BASE_DIR / 'templates']
créer un dossier static à la racine du projet Django pour tous les fichiers non html c'est à dire css, js, images fonts etc
integrer le dossier static au settings au niveau de static avec la commande STATICFILES_DIR = [BASE_DIR / 'static']
faire les migrations avec la commande python manage.py makemigrations
après faire la commande python manage.py migrate
on crée un super user avec la commande python manage.py createsuperuser
puis on lance le projet avec la commande python manage.py runserver