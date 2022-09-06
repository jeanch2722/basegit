# -- Initialisation du client git

# creation de la branche par défaut
git config --global init.defaultBranch <branch_name>
# indique le nom de l'utilisateur pour signer les commits
git config --global user.name <first-name name>
# iniquer le mail de l'utilisateur pour signer les commits
git config --global user.email <email>
# vérification de la config de git
git config --list --show-origin
# ajout d'un proxy pour utilisation de dépôt de distant
git config --global http.proxy http://proxyUsername:proxyPassword@proxy.server.com:port

# -- les commandes de bases

# Création d'un projet 
git init
# Modification du nom d'une branche :
git branch -m <name>
# Donne l'état de la branche et si des modifications ont eu lieu sur les fichiers
git status
# Ajoute le fichier pour le prochain commit
git add README.MD
# Enregistre (commit) les fichiers comme étant les versions de référence
git commit -a -m "Mes commentaires"
# -- Vérifie la différence entre les fichiers actuels et la version de référence
git diff
# Retourner à la version du précédent commit si fichier non encore selectionné
git restore MonFichier
# Déselection d'un fichier : 
git restore --staged MonFichier

# -- Les commandes de branche

# Affichage des branches existantes
git branch
# Création d'une nouvelle branche
git checkout -b NomDeBranche

# -- Github

# Ajout d'alias pour un dépot github ou autre
git remote add origin https://github.com/Repo/NomProjet
#Pousser une branche dans le dépot distant
git push -u origin Branche

# -- SOURCES
- [Paramétrage à la première utilisation](https://git-scm.com/book/fr/v2/D%C3%A9marrage-rapide-Param%C3%A9trage-%C3%A0-la-premi%C3%A8re-utilisation-de-Git)
- [Une introduction pour les débutant pour git et github](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)
- 