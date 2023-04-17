## Flag 🚩 

HSR{cathedralenotredamedereims}

## Description :scroll:

Deux utilisateurs récurrents du discord OSINT-FR (Laura et Sam) se sont mis à sympathiser au fur et à mesure de leurs interactions, pour des tips, des participations à des challenges, etc...

Ils se rapprochent au point de vouloir se rencontrer et un événement va favoriser cette rencontre: le Hack Secu Reims.

Laura habites Reims et proposes à Sam de venir à l'événement pour profiter des conférences, du CTF et de la ville qu'il n'a encore jamais visité.

Mais au moment de convenir des détails de l'évènement et de la rencontre, Sam va recevoir un email intrigant ainsi qu'une archive verrouillée.

## Principe 💭 

De la dissimulation d'informations dans un texte et des images. Utilisations de différents outils, accompagné de recherches de positions géographiques.

## Write-up 📝 

La première partie du challenge porte sur le message de Laura qui est rempli de lettres en italique à noter et mettre de côté pour former des mots. Les points ont aussi leur importance. Voilà ce que cela donne:

![Message](https://user-images.githubusercontent.com/17589828/227071348-34d6918d-7034-4b64-9c05-0d408856d15e.PNG)

La chaine de caractères finale à obtenir doit être rentrée sur le site https://what3words.com////airports.necklace.ledge

C'est un site qui permet l'identification de lieux dans le monde en se basant sur 3 mots aléatoires.

Voilà ce qu'il faut obtenir dans le cas présent:

![3words](https://user-images.githubusercontent.com/17589828/227071869-29d3d305-c074-45b7-b5ca-bd263a98ca5e.PNG)

Le lieu dont parle Laura est la Porte Mars et c'est donc le mot de passe de l'archive Secret.zip -> portemars

Ensuite, une fois que l'archive est ouverte, il faut se pencher sur le seul fichier qu'elle contient:

![portemars](https://user-images.githubusercontent.com/17589828/227072509-d8e90b77-6007-47bd-8de1-d53fc7bae02b.PNG)

Cette image possède volontairement un grand nombre de métadonnées pour embrouiller les joueurs. Alors que la solution se trouve littéralement dans l'image elle-même:

![binwalk](https://user-images.githubusercontent.com/17589828/227072902-1f00f993-4ed6-43d6-9882-e5b0fef9db94.PNG)

Une autre archive zip qui contient des fichiers supplémentaires est cachée à l'intérieur.

Il faut donc faire une extraction de l'archive et on obtient un nouveau dossier "Lieux":

![Lieux](https://user-images.githubusercontent.com/17589828/227073245-08025a27-0bca-4530-945c-edee19ea927a.PNG)

Il y a 6 images de grandes villes en France, et deux fichiers txt avec des informations dedans.
Le fichier "Localisation" contient un indice pour aiguiller les joueurs.
Le fichiers "Liens" contient des liens google maps et d'autres pour le coup raccourcis pour qu'ils ne soient pas reconnaissables. Les liens maps sont là pour la confusion en donnant des repères inutiles. Et les liens raccourcis pour troller sauf un, le dernier. Le premier redirige vers un blog de phylosophie, le deuxième est un Rick Roll et le dernier est un article d'IBM sur les GeoHashs. 

Ces liens ont pour but de tromper et d'envoyer les joueurs dans de mauvaises directions.

Il va donc falloir se concentrer sur les images. L'information que l'on cherche se trouve dans les métadonnées:

![Coordonnées](https://user-images.githubusercontent.com/17589828/227074837-835f391f-a21e-4576-81d6-030e50c24e6b.PNG)

Il s'agit de coordonnées GPS coupées en plusieurs parties et mises dans les métadonnées de chaque images pour les cacher.

Une fois que l'on récupère toutes les parties, il faut aussi réussi à les assembler correctement (indication Localisation.txt) sinon on a pas le bon endroit.

On est censé avoir: 49°15'13.8931"N 4°02'2.5508"E -> Cathédrale Notre-Dame de Reims

On a donc trouvé le lieu de rencontre le Laura et Sam. 

## Contact 📲

Whilsker#7942 sur discord
