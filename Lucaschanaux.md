# Exercice 1. Commandes de base

Commencez par mettre à jour votre système avec les commandes vues dans le cours.

j'ai fait `apt full-upgrade` pour mettre a jour la distribution 

1- <b>_.1. Quels sont les 5 derniers paquets installés sur votre machine ?_</b>

J'ai fait `grep installed /var/log/dpkg.log` <br>
Les 5 derniers paquets sont :  libc-bin:amd64 2.29-0Ubuntu2 <br>
man-db:amd64 2.8.5-2 <br> 
rsyslog:amd64 8.32.0-1Ubuntu7 <br> 
apt-utils:amd64 <br> 
sosreport:amd64 <br> 


2- <b>_2. Utiliser dpkg et apt pour compter le nombre de paquets installés (ne pas hésiter à consulter le manuel !).
Comment explique-t-on la (petite) différence de comptage ?_</b>

j'ai fait `dpkg -l | grep"^ii" | wc -l` et j'ai vu qu'il y'avait 519 lignes de paquet
j'ai fait `apt list --installed | wc -l` et j'ai vu 524 


3- <b>_Combien de paquets sont disponibles en téléchargement ?_</b>



4- <b>_Créer un alias “maj” qui met à jour le système_</b>

J'ai fait ```alias maj='apt update && apt upgrade'```  


5- <b>_ A quoi sert le paquet fortunes ? Installez-le._</b>

j'ai fait `apt show fortunes` pour savoir a quoi sert le paquet fortunes <br>
j'ai ensuite `apt-get install fortunes` pour l'installer 

6- <b>_Quels paquets proposent de jouer au sudoku ?_</b>

j'ai fait `apt-cache search sudoku` il y'a plusieurs résultats possible (ksudoku, gnome-sudoku, fltk1.3-games,nudoku etc..)

7- <b>_Lister les derniers paquets installés explicitement avec la commande apt install_</b>

j'ai fait `cat /var/log/dpkg.log` et je vois qu'il y'a eu fortunes en paquet installlé récemment 

# Exercice 2



