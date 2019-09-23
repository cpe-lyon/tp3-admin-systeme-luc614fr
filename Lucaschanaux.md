# Exercice 1. Commandes de base

Commencez par mettre à jour votre système avec les commandes vues dans le cours.

j'ai fait `apt full-upgrade` pour mettre a jour la distribution 

1- <b>_.1. Quels sont les 5 derniers paquets installés sur votre machine ?_</b>

J'ai fait `grep installed /var/log/dpkg.log`
Les 5 derniers paquets sont :  libc-bin:amd64 2.29-0Ubuntu2
man-db:amd64 2.8.5-2
rsyslog:amd64 8.32.0-1Ubuntu7
apt-utils:amd64
sosreport:amd64


2- <b>_2. Utiliser dpkg et apt pour compter le nombre de paquets installés (ne pas hésiter à consulter le manuel !).
Comment explique-t-on la (petite) différence de comptage ?_</b>

il y'a 519 paquet installé 
j'ai fait `dpkg -l` et j'ai vu qu'il y'avait 519 lignes de paquet

3- <b>_Combien de paquets sont disponibles en téléchargement ?_</b>



4- <b>_Créer un alias “maj” qui met à jour le système_</b>

alias maj='apt update && apt upgrade' 

5- <b>_. A quoi sert le paquet fortunes ? Installez-le._</b>
