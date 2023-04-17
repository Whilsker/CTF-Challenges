## Flag 🚩 

HSR{43b043013fb800bb747d1ca2393e90ce}

## Description :scroll:

Reims est une ville magnifique sur Nord Est de la France. 
Elle est la capitale officieuse de la région productrice de champagne, un produit qui en a fait sa renommée.
Son architecture également attire l'attention. On pense notamment à l'Ange au sourire, emblème de la ville de Reims. Et donc vient naturellement la cathédrale, avec une longueur de 149,17 mètres, pour une hauteur de 87 mètres au clocher, elle est bâtie sur le plan d'une croix latine. C'est un chef-d'œuvre de l'architecture gothique.

Les deux images montrent ces deux fiertés de la ville de Reims. Maintenant à vous de trouver le point commun fondamental entre les deux.

## Principe 💭 

MD5 collision

## Write-up 📝 

Il fallait se rendre compte que les images étaient parfaitement identiques... du moins leurs métadonnées... (on devrait se rendre compte assez directement qu'ils font exactement la même taille, etc.)
En passant par Apéri'solve on pouvait aussi remarquer qu'il interprétait les deux fichiers comme étant les mêmes.

Inutile ensuite de perdre du temps à chercher la différence de caractères entre les deux fichiers, mais il fallait plutôt penser au concept de checksum qui permet de s'assurer de son intégrité.

Donc pour le challenge il fallait calculer les checksums des deux fichiers avec la commande $ md5sum Cathedrale.jpg Champagne.jpeg 

Et on se rend compte que c'était le même hash MD5.

## Contact 📲

Whilsker#7942 sur discord
