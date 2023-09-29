Namesake : [[Hierophant Green]], Stand de [[Noriaki Kakyoin]], qui peut se déplacer beaucoup plus loin que la plupart des Stands

# But du projet

Le projet a pour but de créer un ensemble de services pour permettre de travailler à distance, centraliser nos données, créer des processus de traitement / validation / déploiement automatisés, etc.

# Composants

Chaque composant du projet correspond à un besoin, auquel on aura donc trouvé une (ou plusieurs) solution(s).

## git

Aujourd'hui les services `git`, c'est globalement [[Github]] et [[Gitlab (site)]]. Problèmes : le premier ne respecte pas d'éthique de base concernant la propriété du code qu'il héberge, et le deuxième reste le site d'une entreprise.

La solution serait donc de créer et [[self-host]] un [[Gitlab (serveur)]] puisque techniquement, le serveur est un [[FOSS]].

On pourrait techniquement utiliser [[Gitea]] à la place pour un projet maintenu par une entité à but non lucratif, mais le serveur est encore un peu en retard sur certain points (notamment la possibilité de build des releases, qui serait nécessaire pour OH)
## PC Game Streaming

Des fois, c'est sympa de se poser tranquillement dans le lit pour jouer. Mais le petit souci c'est qu'un petit raspberry pi 4 comme c'est le standard actuellement n'est pas capable de faire tourner grand chose au-delà de la PSP. Et des fois c'est sympa de jouer à des jeux un peu plus modernes.

Une bonne solution pour ça est [[Moonlight]], un serveur de streaming de jeu PC ([[FOSS]], en plus) qui est une implémentation du protocole [[NVIDIA GameStream]]. Donc, on pourrait installer un serveur Moonlight sur une machine de jeu (HermitePurple ou Deathputer typiquement) et stream un jeu depuis cette machine vers un raspberry branché à une TV.

## PS3 Game Streaming

Pour les backups de jeux [[PS3]], on peut utiliser [[ps3netsrv]] sur une machine modeste, pour une console équipée d'un [[CFW]].

## PS2 Game Streaming

Pour les backups de jeux [[PS2]], on peut utiliser un [[SMB]] ou autre Samba-like, sur une machine modeste encore une fois, pour aller sur n'importe quelle PS2 disposant de [[FreeMcBoot]] et ayant [[OpenPS2Loader]].

Pour gérer la bibliothèque, il y a une application Windows [[OPLManager]]. Elle est graphique, mais avec un ou deux jours je pourrais peut-être construire un outil en [[CLI]] en Python ou autre.

## PSX Game Streaming

Pour les backups de jeux PSX, on peut tout simplement utiliser la méthode de [[#PS2 Game Streaming]] en installant et configurant [[POPStarter]] pour OPL.

## XBox, Wii, etc. Game Streaming

Pour les jeux d'autres consoles, une idée serait d'installer des Emus et de les configurer pour le [[#PC Game Streaming]].

Typiquement, [[Retroarch]] pourrait être utile ici

## Web Server