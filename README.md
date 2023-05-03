Quentin LAPARRE
Tom VAILLANT
Maxime BOUJU


# SAE-2.03                                                                                                           Groupe 15
------------------------------------------------------------------------------------------------------------------------------
## Service de vidéo à la demande
### Introduction

Notre projet consiste à créer un site de vidéo à la demande avec l'aide de jellyfin, qui est un open source.
Notre projet doit partir de la base officielle de debian, c’est-à-dire que la première ligne du Dockerfile devrait être ` FROM debian:latest `
Notre projet doit utiliser un Dockerfile.

### Installation du Docker  

* Pour vérifier que Docker soit bien installé, on effectue la commande suivante dans le terminal :  
` docker --version `  
  
  Nous devons alors voir la version du Docker que nous utilisons.  
  
### Lancer le site Web  

* Il faut dans un premier temps cloner le référentiel :  
` git clone git@github.com<nom_utilisateur>/docker-sae203.git `  
Avec comme <nom_utilisateur> le nom de votre utilisateur  
  
* Nous allons créer le docker avec la commande suivante :  
` docker build -t jellyfin-server C:\Users\<nom_utilisateur>\docker `  
Avec comme <nom_utilisateur> votre nom d'utilisateur  
  
* Ensuite il faut exécuter la commande pour lancer le docker  
` docker run -d --name SAEG15 -p 8096:8096 -v C:\Users\<nom_utilisateur>\docker\data:/var/lib/jellyfin -v C:\Users\<nom_utilisateur>\docker\cache:/var/cache/jellyfin -v C:\Users\<nom_utilisateur>\docker\bande_annonce:/bande_annonce jellyfin-server `  
  
* Enfin lancer une page web et insérer l'URL :   
  ` localhost:8096 `
  
* Il est important de rentrer "Groupe 15" dans le nom d'utilisateur lorsque le site est lancé.
