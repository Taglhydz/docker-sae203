# SAE-2.03                                                                                                           Groupe 15
------------------------------------------------------------------------------------------------------------------------------
## Service de vidéo à la demande
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
` docker run -d --name SAEG15 -p 8096:8096 -v C:\Users\<nom_utilisateur>\docker\bande_annonce:\bande_annonce jellyfin-server `  
  
* Enfin lancer une page web et insérer l'URL :   
  ` localhost:8096 `  
