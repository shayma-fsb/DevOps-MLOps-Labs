Tache: Exécution Locale de l'Application

creation de environnement virtuel et sa preparation pour isolation des dependances du projet a fin d'eviter tous conflis

la cmd a executer dans le meme dossier ou se trouve le script a executer( dans mon cas c'est train.py) : python -m venv .venv

puis active le venv:

.\\.venv\\Scripts\\Activate.ps1    (puisque je travaille depuis powershell)

l'affichage de .venv dans powershell montre que le virtual enviorment est active

Puis 2eme etape: installation des dependances:

toutes les dependances necessaires se trouvent dans requirements.txt

pip install -r requirements.txt

Puis 3eme etape :

execution et verification:

python src/train.py



Le script s'est exécuté sans erreur. Il a affiché des métriques d'entraînement/validation à la console et a généré un fichier de modèle sérialisé

