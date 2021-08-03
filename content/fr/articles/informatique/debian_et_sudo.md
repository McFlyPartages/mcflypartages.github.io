+++
title = "Debian 10 et sudo"
subtitle = "Retrouver le sudo"
description = "Retrouver le sudo"
date = 2021-06-30
#images = ["images/articles_vierge_1.png"]
author = "McFly"

draft = true

series = ["Debian"]
categories = ["Debian"]
tags = ["Informatique" , "Serveur" , "Linux"]

featured = true
comment = false
toc = true
reward = false

+++
Depuis le passage a sa version 10, Debian a supprimer par défaut la commande 'sudo'.

Nous allons voir comment la réinstaller et ajouter votre utilisateur au groupe 'sudo'.


## installation de 'sudo'

Connectez vous en SSH, puis passer en root avec la commande suivante 'su -', entrer votre mot de passe 'root' puis taper la commande suivante :
'apt-get install sudo -y'

## Ajouter votre utilisateur

Nous allons maintenant ajouter votre utilisateur au groupe sudo avec cette commande 'usermod -aG sudo mon_utilisateur'.

Connectez vous a votre utilisateur avec la commande 'su mon_utilisateur' puis tester avec 'sudo date', si la date et l'heure s'affiche c'est tout bon.

## conclusion

Cet écrit est plus un mémo qu'un tutoriel.