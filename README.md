# TD-Final-part1-APi-AA-2023_24
# Introduction aux web-services (API)
# TD FINAL (PART 1 sur 2) : Spécification Open API

## Nous voulons spécifier le web-service d’une gestion des matchs d’une compétition de football. En effet, le web-service existant permet d’effectuer les fonctionnalités suivantes :

1. Créer et obtenir une liste de compétitions, dont les caractéristiques sont :
- Nom de la compétition, exemple : LIGA
- Pays ou Continent où se déroule la compétition, exemple : ESPAGNE ou
EUROPE
1. Créer et obtenir une liste d’équipes, dont les caractéristiques sont :
- Nom de l’équipe
- Slogan de l’équipe
- La liste des compétitions auxquelles elle joue
- La liste des joueurs
.
En particulier, notez qu’une équipe peut jouer dans plusieurs compétitions,
par exemple, l’équipe intitulée Real Madrid peut à la fois jouer dans la
compétition intitulée LIGA et dans la compétition intitulée UEFA CHAMPIONS
LEAGUE.
Un autre exemple, l’équipe FC Barcelona peut uniquement jouer dans la
compétition intitulée LIGA mais pas dans la compétition intitulée UEFA
CHAMPIONS LEAGUE.
Aussi, notez que dans la fonctionnalité d’ajout d’équipe ne comprend pas
l’attribution des compétitions ou encore l’attribution des joueurs à l’équipe.
Autrement dit, durant la création d’équipes, on ne peut fournir que le nom et
le slogan, mais c’est durant l’obtention que nous avons la liste des
compétitions auxquelles elle participe ainsi que la liste des joueurs qui la
composent.
Le fait d’associer une équipe à une liste de compétitions est donc un autre
point d’entrée, de même, l’association (dit également “transfert” dans le
jargon) d’une liste de joueurs à une équipe est un autre point d’entrée.
1. Créer, modifier ou obtenir une liste de joueurs d’une équipe donnée, dont les
caractéristiques sont :
- Nom du joueur
- Numéro du joueur
- Pied fort du joueur (Gauche ou Droite sont les seules valeurs possibles)
Notez que durant la création, les seules informations à fournir sont le nom du
joueur, le numéro du joueur et le pied fort du joueur.
Lorsqu’on va associer un joueur à une équipe, notez qu’il faut passer par un
autre point d’entrée, où nous associons directement une liste de joueurs à
une équipe spécifique.
4. Enfin, spécifier les paramètres de requêtes nécessaires, pour filtrer les données
suivantes :
- Paramètre de requête, intitulée “teamName” de type string, dans la requête
qui permet d’obtenir la liste des équipes. Celui-ci a pour objectif de filtrer la
liste des équipes obtenues en fonction de la valeur du “teamName” fournie,
préciser cela dans la spécifications à travers la description.
- Paramètre de requête, intitulée “playerName” de type string, dans la requête
qui permet d’obtenir la liste des joueurs d’une équipe. Celui-ci a pour objectif
de filtrer la liste des joueurs obtenues en fonction de la valeur du
“playerName” fournie, préciser cela dans la spécifications à travers la
description.
NB :
- La spécification doit se faire intégralement en Anglais, si vous employez du français,
la note attribuée sera automatiquement la note minimum.
- Chaque liste en réponse d’une requête HTTP GET doit être paginée, donc avoir un
paramètre de requêtes page et pageSize, qui sont des champs obligatoires. Notez
que la liste dont on mentionne ici c’est la liste principale, par exemple la liste
- Si vous n’utilisez pas les components object (que ce soit pour les schema ou pour
tout autre object), votre note va être significativement diminuée (12 sur 20 maximum)
