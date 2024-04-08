## Description :scroll:

Un ami fan de GeoGuessr a fait une liste de lieux qu'il trouve insolites ou intéressants et il vous demande de répondre à ces questions :

1. Quel message peux-tu lire ?
2. En quelle police est-il écrit ?
3. Qui en est le(s) créateur(s) ?
4. En quelle année ?

## Principe 💭

Utilisation de google map en vue satellite pour interpréter les bâtiments et leurs formes comme étant des lettres.
Puis faire des recherches sur cette police d'écriture.

## Write-up 📝

#### 1. La première partie du challenge consiste à faire du GEOINT en utilisant des coordonnées gps données

Ces coordonnées étaient données sous forme de GeoHashs.

Ici le but était de distinguer des lettres dans les formes des bâtiments en vue satellite sur Google Map.

```
u3bv18fu8c3; => 55°43'39.2"N 12°22'27.9"E  => E
u3busu37wcz; => 55°39'31.4"N 12°30'55.6"E  => F
u281xymc68d; => 48°06'38.6"N 11°35'54.9"E  => I
dpz86jwxhtd; => 43°40'08.9"N 79°21'22.0"W  => O
spc01y5zw88; => 43°37'40.8"N 1°29'18.9"E   => R
9q8yy4srmv1; => 37°45'50.5"N 122°25'32.0"W => L
spc01q2tn29; => 43°37'44.2"N 1°27'43.7"E   => N
u283bbmq1wx; => 48°07'21.2"N 11°38'30.5"E  => S
u281yrhe4kz; => 48°09'32.8"N 11°31'51.4"E  => I
u0yjh2pjyh2; => 50°05'55.2"N 8°38'02.9"E   => O
9q5bgpr9fpj; => 33°55'19.2"N 118°20'03.6"W => T
u2fkb4z3v7u; => 50°04'08.9"N 14°25'27.3"E  => F
```

Le message a retrouver est en trois mots. Il s'agit de trouver ***OSINT FOR LIFE***.

#### 2. La suite s'enchaîne assez rapidement

En cherchant sur google quelque chose d'aussi basique que ***bâtiment en forme de lettre***, on pouvait trouver un article du figaro immobilier qui parlait de la création d'une police de caractère utilisant des photos aériennes de bâtiments.

![OSINT Partie 2](https://github.com/Whilsker/CTF-Challenges/assets/17589828/564b3ce6-dd14-4c58-9fcb-641139d67661)

Cet article explique le pourquoi du comment et donne même les noms des créateurs et le nom de la police.

Il faut ici garder ***Aerial Bold***, ***Benedikt Groß*** et ***Joey Lee*** comme réponses aux questions 2 et 3.

En cherchant le nom de la police dans google on peut tomber sur le [site](https://benedikt-gross.de/projects/the-aerial-bold-project/) d'un des créateurs qui explique le projet plus en détail et il donne accès au [kickstarter](https://www.kickstarter.com/projects/357538735/aerial-bold-kickstart-the-planetary-search-for-let) du projet.

Ici on voit que la période de financement à durée du 14 oct. 2014 au 13 nov. 2014.

C'est donc l'année 2014 qui va répondre à la question 4.

## Flag 🚩

HSR{osintforlife-aerialbold-benediktgroßjoeylee-2014}

## Contact 📲

whilsker sur discord
