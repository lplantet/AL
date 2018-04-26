# AL
TP Projet d'Architecture Logicielle

# Pour lancer le serveur tomcat il faut lancer le script catalina, qui se trouve dans le dossier AL-TP/apache-tomcat-9.0.6/bin :
"./catalina.sh run"
# Note : il faut compter quelques minutes avant que le serveur se mette en marche

# Les composants recipes-rss sont lancés avec les commandes suivantes en se plaçant dans le dossier AL-TP/recipes-rss:
java -jar rss-middletier/build/libs/rss-middletier-*SNAPSHOT.jar
java -jar rss-edge/build/libs/rss-edge-*SNAPSHOT.jar

# Pour build les Dockerfile, utiliser la commande :
docker build -t NomImage .
# Le nom de l'image peut être "imagecatalina" par exemple

# Pour lancer le serveur apache-tomcat en passant par le docker, se placer dans le répertoire AL-TP/apache-tomcat-9.0.6 :
docker run tomcat catalina.sh run
# Après cette commande, un message disant que le serveur est ouvert s'affiche, mais celui-ci n'est pas accessible





