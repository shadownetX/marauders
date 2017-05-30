# Configuration Server

Création d'un dossier sous windows qui hébergera les infos du serveur de dev dans :
```
C:\server\marauders.dev
```

Ajouter les 4 éléments de **vagrant_config** à l'intérieur de marauders.dev\
```
https://github.com/shadownetX/marauders/tree/master/vagrant_config
```

Ensuite c'est très simple (enfin pense à installer vagrant sur ta machine)

Ouvre ton invite de commandes puis :
```
cd c:/server/marauders.dev
vagrant up
```

Laisse faire vagrant +- 10 minutes.

# Projet Marauders


Un nouveau dossier **html** a été généré dans ton projet c'est à cet endroit qu'il faudra 
cloner le dépôt git : https://github.com/shadownetX/marauders.git

Maintenant que tout est au poil tu peux lancer un ``composer install`` (je t'ai laissé
le fichier **.json** pour que tout soit automatisé).

# VHOST

Dernière étape, ajouter la redirection en local pour atteindre le back-office depuis le fichier **hosts** dans :
```
C:\Windows\System32\drivers\etc
```
Une nouvelle ligne :
```
192.168.56.147 marauders.dev
```
Direct tu as accès à http://marauders.dev en local

# Infos Russe

Tu peux ensuite te connecter en ssh dans marauders.dev en tapant : ``vagrant ssh`` ou kill 
la session avec un ``vagrant halt`` quand tu auras besoin de créer ton projet angular ;)

PS : **Node.js (CLI)** est déjà installer 
