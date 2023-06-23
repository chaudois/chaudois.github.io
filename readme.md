# Site Racine des membres de la famille chaudois



Ce site static permet la redirection vers les site personnels des membres de la familles Chaudois si  ceux-ci en ont.

![](./documentation/ressources/images/image_accueil.png)

## Lien utiles

- Mail Damien : damien.chaudois@gmail.com
- Domaine : https://domains.google.com/registrar/chaudois.com
- serveur de fichiers statique : https://dashboard.render.com/
- GitHub : https://github.com/chaudois/chaudois.com
- noip : https://www.noip.com/members/dns/

## Domaine

le DNS est [Google Domains](https://domains.google.com/registrar/chaudois.com). Les login sont détenues par Damien Chaudois (damien.chaudois@gmail.com). le domaine est enregistré à son nom



## Host

les fichiers sont host sur [render.com](https://dashboard.render.com/static/srv-cagimosobjd12th5oojg) gratuitement. La contrepartie à la gratuité est une URL au format chaudois.render.net. Pour contourner ce problème, le domaine redirige l'URL chaudois.com directement sur l'IP de l'hôte.

Les fichiers sources sont versionné sur [github](https://github.com/chaudois/chaudois.com) sur un repository public. le propriétaire est Damien Chaudois. une autorisation est requise pour pousser des Pull Request.



## Déploiement / Mise à jour du site

Le seul moyen de mettre à jour le site est de passer par GitHub. Render est hook sur la branche master et déclenche un déploiement sur chaque nouveau commit sur cette branche. Les fichiers sources ne sont pas à la racine sur repository, mais dans ./src



## damien.chaudois.com

Cette section concerne le site personnel de Damien mais est placé là d'ici à sa création et celle du repository correspondant.



### Hôte

l'application est pour le moment hébergé sur la machine PC-BOISCO sur un serveur IIS local. Pour contourner l'IP dynamique de Orange, le domaine redirige sur un service VPN qui sert de DNS et va régulièrement mettre à jour la nouvel IP pour la mapper avec le nom de domaine public custom. Le nom de domaine est chaudois.ddns.net. Pour que l'IP soit régulièrement mise à jour, un agent tourne en tâche de fond sur la machine hôte pour aller pousser la nouvelle IP sur noip.com