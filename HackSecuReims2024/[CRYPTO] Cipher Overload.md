## Description :scroll:

Le stagiaire vient de découvrir le concept de chiffrement et vous lance un défi.

Retrouvez la chaîne originale qu'il a encodé.

## Principe 💭

Utilisation de multiples encodages sur une même chaîne de caractère.

## Write-up 📝

Le flag à été encodé une dixaine de fois, donc il va falloir passer par dix étapes pour le retrouver.

#### 1. La première partie du challenge porte sur le dernier encodage appliqué

```
00 0 0 000000 00 00 0 000 00 0 0 000 00 0 0 0000 00 00 0 0 00 0 0 0 00 00000000 0 00 00 0 0 0 00 0 0 0 00 0 0 00 00 0000 0 0 00 0 0 00 00 00 0 0 00 000 0 00 00 000000 0 00000 00 0000 0 0 00 0 0 0 00 0000 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 0000 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 000 0 000000 00 00 0 0000 00 0 0 0 00 0 0 00 00 000 0 0 00 000 0 00 00 0 0 0 00 0000 0 000000 00 0 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 0000 0 00 00 00 0 00 00 0 0 0 00 0000 0 0 00 0 0 0 00 00000 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 00000 0 0 00 00 0 0 00 0 0 0 00 0 0 00 00 0 0 00 00 0000 0 0 00 00 0 0000 00 0 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 0 0 00000 00 0000 0 0 00 00 0 0 00 0 0 0 00 00 0 0 00 000 0 00 00 0 0 0 00 0000 0 00 00 00 0 0 00 0 0 0 00 0 0 00 00 00 0 0 00 0 0 0 00 00 0 0 00 0 0 0000 00 00 0 0 00 0 0 0 00 00000000 0 0 00 0 0 0 00 0 0 00 00 00 0 00000 00 00 0 00 00 0 0 0 00 0000 0 0 00 000 0 000 00 0 0 00000 00 000 0 00 00 0000 0 0 00 00 0 0000 00 0 0 0 00 00 0 0000 00 0 0 0 00 00 0 0 00 0 0 0 00 0 0 00 00 00 0 000 00 0 0 00 00 00 0 000 00 00 0 0 00 00 0 0000 00 0000 0 00 00 0 0 0 00 0000 0 00000 00 00 0 00 00 00 0 000 00 0 0 0 00 00 0 0 00 0 0 00 00 0 0 00000 00 000 0 00 00 0000 0 0 00 0 0 0 00 00000 0 0 00 0 0 00 00 00 0 0 00 000 0 00000 00 0 0 0 00 00 0 0 00 0 0 0 00 00000 0 0 00 000 0 00 00 00 0 0000 00 0 0 0 00 00 0 00 00 00 0 00 00 0 0 00 00 0000 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 000 0 000 00 00 0 00 00 00 0 0 00 000 0 00000 00 000 0 0 00 00 0 00 00 00 0 0 00 0 0 00000 00 00 0 00 00 0 0 0 00 0 0 0 00 00 0 0 00 0 0 0 00 0000 0 00000 00 0 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 00 0 00 00 00 0 00 00 00 0 000000 00 00 0 0 00 00 0 000 00 00 0 000000 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 00 0 0 00 0 0 00 00 00 0 0 00 00 0 000 00 0 0 0 00 00 0 0 00 0 0 0 00 000 0 00 00 0 0 0 00 000 0 0 00 00 0 0 00 0 0 00 00 0 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 0 0 00000 00 00 0 00 00 0 0 00 00 000 0 000 00 0 0 00 00 00 0 000 00 00 0 0 00 00 0 000 00 0 0 0 00 000 0 00 00 00 0 0 00 000 0 000000 00 00 0 0 00 00 0 000 00 00 0 0000 00 0 0 0 00 00 0 00 00 0 0 0 00 000 0 000 00 0 0 00 00 00 0 00 00 000 0 00 00 0 0 00 00 000 0 00 00 00 0 00 00 00 0 0 00 000 0 00000 00 00 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 00000000 0 00 00 0 0 0 00 0 0 0 00 0 0 00 00 000 0 0 00 000 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 000 0 000 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 000 00 00 0 00 00 0 0 00000 00 0 0 0 00 00 0 0000 00 0 0 0 00 00 0 00 00 0 0 0 00 0000 0 000 00 0 0 00 00 00 0 0 00 000 0 00 00 00 0 00000 00 000 0 00 00 0 0 00 00 000 0 0 00 00 0 0 00 0 0 0 00 0 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 000 0 00 00 000 0 00 00 00 0 0 00 00 0 00 00 0000 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 00 00 00 0 0 00 0000 0 00 00 00 0 0 00 00 0 000 00 0 0 00 00 000 0 0 00 0 0 0 00 0 0 00 00 0 0 0 00 000 0 000 00 00 0 0 00 0 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 0 0 00 00 00 0 0 00 000 0 00 00 0 0 0 00 000 0 0 00 0 0 0 00 00 0 0 00 0 0 0 00 0 0 00 00 00 0 0 00 0 0 0 00 00 0 0 00 0 0 000 00 000 0 0 00 00 0 000000 00 00 0 00 00 00 0 0 00 000 0 0 00 0 0 0 00 00000 0 0 00 00 0 000 00 0 0 0 00 0 0 00000 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 000 00 00 0 00 00 0 0 00000 00 0 0 0 00 00 0 000000 00 00 0 00 00 00 0 0 00 000 0 0 00 0 0 0 00 0000 0 0000 00 00 0 0 00 00 0 0000 00 0000 0 0 00 0 0 0 00 0 0 00 00 00 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 000 0 00 00 0 0 0 00 0000 0 00 00 00 0 00 00 0 0 0 00 0000 0 0 00 0 0 0 00 00000 0 00 00 0 0 0 00 0 0 0 00 00 0 0000 00 0 0 0 00 0 0 00000 00 0 0 0 00 0 0 000 00 0 0 000 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 000 0 00 00 000 0 00 00 0 0 0 00 0 0 0 00 00 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 000 0 00 00 0 0 0 00 00 0 0 00 0 0 00 00 00 0 0 00 0 0 0 00 0 0 00 00 0 0 00 00 000 0 0 00 000 0 0 00 000 0 00 00 00 0 0000 00 0 0 0 00 00 0 00 00 0 0 0 00 0000 0 000000 00 00 0 00 00 0 0 0 00 000 0 0 00 00 0 0 00 00 0 0 00 0 0 00000 00 0000 0 0 00 0 0 0 00 0000 0 00 00 0 0 0 00 00000 0 000000 00 0 0 00000 00 000 0 0 00 00 0 0 00 0 0 00 00 00 0 000 00 00 0 0 00 00 0 0000 00 0000 0 00 00 0 0 0 00 0000 0 000 00 0 0 00 00 0 0 000 00 0 0 0 00 000 0 0 00 00 0 0 00 0 0 00 00 00 0 0 00 0 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0000 0 0 00 00000 0 0 00 0 0 0 00 00 0 0 00 00000 0 00 00 0 0 00 00 000 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 00 0 000 00 00 0 000000 00 00 0 00 00 0 0 0 00 0000 0 0 00 0 0 0 00 0000 0 0 00 0000000 0 0 00 00 0 0 00 0 0 00 00 00 0 0 00 0 0 0 00 0 0 00 00 0 0 00 00 000 0 0 00 00 0 000 00 000 0 0 00 00 0 000000 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 00 0 0 00 0 0 00 00 00 0 0 00 000 0 0 00 00 0 0 00 00 0 0 00 00 0 0 00 0 0 00000 00 0000 0 0 00 0 0 0 00 0000 0 0000 00 00 0 0 00 0 0 0 00 0000 0 00 00 00 0 00 00 00 0 0 00 000 0 000000 00 00 0 0000 00 0 0 0 00 0 0 00 00 000 0 0 00 000 0 00 00 00 0 0 00 00 0 000 00 0 0 00 00 00 0 00 00 0 0 0 00 0000 0 0 00 0000 0 0 00 000 0 00 00 0 0 0 00 0 0 0 00 0 0 00 00 0000 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 0000 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 000 0 000000 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 00 00 000 0 0 00 000 0 00 00 00 0 00 00 0 0 00 00 0000 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 000 0 00 00 00 0 000000 00 00 0 000 00 0 0 00 00 000 0 0 00 0 0 0 00 0 0 00 00 00 0 000 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 00 00 0 0 000 00 0 0 00 00 00 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 000 0 000 00 00 0 00 00 00 0 0 00 00 0 00 00 0000 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 0000 0 00 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 000 00 0 0 00 00 00 0 00 00 00 0 0 00 0000 0 0000 00 0000 0 00 00 00 0 00 00 0 0 00 00 000 0 0 00 000 0 0 00 000 0 00 00 00 0 000 00 0 0 0 00 000 0 00 00 0 0 00 00 000 0 00000 00 000 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 0 0 00000 00 00 0 00 00 00 0 00 00 00 0 0 00 0 0 0 00 00 0 0 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 00 00 000 0 0 00 00 0 00000 00 0000 0 0 00 00 0 0 00 0 0 0 00 0 0 000 00 0 0 0 00 0 0 0 00 00 0 00000 00 00 0 000000 00 00 0 000 00 0 0 00 00 00 0 0000 00 0000 0 00 00 000 0 00 00 00 0 0 00 0 0 0 00 0 0 00 00 0 0 000 00 0 0 000 00 0 0 0000 00 00 0 0 00 0 0 00 00 0000000 0 00 00 0 0 0 00 0 0 0 00 0 0 000 00 0 0 00 00 00 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 0000 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 000 0 0 00 00 0 0 00 0 0 0 00 0 0 00000 00 0 0 0 00 0 0 0 00 00 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 00 00 0 0 00 00 000 0 0 00 00 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 0000 0 0 00 00 0 00000 00 000 0 00 00 0000 0 0 00 00 0 00 00 0 0 0 00 0 0 0 00 00 0 000 00 0 0 00 00 0 0 00000 00 000 0 00 00 000 0 0 00 000 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 000 0 00 00 00 0 00000 00 0000 0 0 00 0 0 0 00 0000 0 0000 00 0000 0 0 00 00 0 0 00 0 0 00 00 00 0 00 00 00 0 0 00 000 0 00000 00 00 0 0 00 00000 0 0 00 0 0 00 00 00 0 0 00 0000 0 00 00 00 0 0 00 000 0 0 00 0 0 0 00 00000 0 00 00 0 0 0 00 0 0 0 00 00 0 000 00 0 0 00 00 00 0 00 00 00 0 0 00 00 0 00 00 000 0 0 00 00 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 0000 0 0 00 000 0 00 00 00 0 0 00 000 0 0 00 0 0 0 00 00000 0 0 00 0 0 0 00 0 0 00 00 0 0 0 00 00000 0 0 00 00 0 0 00 0 0 0 00 0 0 00 00 0 0 00 00 000 0 0 00 000 0 0 00 00 0 000 00 0 0 0 00 0 0 00000 00 0 0 00000 00 000 0 00 00 0000 0 0 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 00 0 0 00 0 0 0 00 00 0 00000 00 0 0 0 00 0 0 000 00 0 0 00 00 000 0 0 00 000 0 00 00 0 0 0 00 0000 0 00 00 00 0 00 00 00 0 00 00 0 0 00 00 0000 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 00 0 0 00 0 0 0 00 0 0 00 00 00 0 0 00 0 0 0 00 00000 0 0 00 0 0 0 00 0 0 00 00 0 0 00 00 00 0 0 00 0000 0 00 00 0 0 0 00 0 0 0 00 0 0 00 00 0000 0 0 00 0 0 00 00 00 0 0 00 000 0 0 00 00 0 0 00 00 0 0 00 00 0 00 00 00 0 0 00 000 0 00000 00 000 0 0000 00 0 0 0 00 0 0 0 00 0000 0 0 00 000 0 00 00 00 0 0 00 000 0 0 00 0 0 0 00 0000 0 0000 00 00 0 0 00 0 0 00 00 000 0 0 00 000 0 00 00 00 0 0 00 00 0 000 00 00 0 00 00 0 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 0 0 00000 00 00 0 00 00 0 0 0 00 000 0 00 00 0000 0 0 00 00 0 0 00 00 0 000 00 00 0 00000 00 000 0 00 00 00 0 00 00 00 0 00000 00 000 0 0 00 000 0 00 00 00 0 000 00 0 0 00 00 00 0 00 00 0 0 0 00 0 0 0 00 00 0 0 00 0 0 0 00 0000 0 0 00 00000 0 0 00 0 0 0 00 00 0 0 00 0 0 00 00 00 0 00 00 00 0 0 00 000 0 000000 00 0 0 000 00 000 0 0 00 0 0 0 00 0000 0 00 00 00 0 00 00 0 0 0 00 0000 0 00000 00 00 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 00 0 00 00 00 0 0 00 00 0 00 00 000 0 0 00 000 0 0 00 00 0 000 00 00 0 000000 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 000 00 00 0 00 00 00 0 000 00 00 0 0 00 0 0 0 00 00 0 0 00 0 0 0 00 000 0 00 00 0 0 0 00 0000 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 00 0 00 00 00 0 0 00 00 0 0 00 00 0 0 00 00 0 0 00 0 0 0 00 0 0 0 00 000 0 00000 00 00 0 0 00 00000 0 0 00 0 0 0 00 00000 0 0 00 00 0 00 00 0 0 00 00 000 0 0 00 0 0 0 00 00 0 0 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 0 00 000 0 000 00 00 0 00 00 0 0 0 00 000 0 000 00 0 0 00 00 00 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 00 0 0 00 00000 0 00 00 00 0 0 00 00 0 00 00 0000 0 0 00 0 0 0000 00 0000 0 00 00 000 0 00 00 00 0 00 00 0 0 0 00 0000 0 00000 00 00 0 00 00 00 0 0 00 000 0 00 00 000 0 0 00 00 0 00000 00 000 0 00 00 0000 0 0 00 0 0 000 00 0 0 0 00 0 0 0 00 0 0 0 00 0000 0 0 00 000 0 00 00 00 0 0 00 000 0 0 00 0 0 0 00 0000 0 0 00 000 0 0 00 0 0 0 00 00 0 0000 00 0000 0 00 00 00 0 0 00 00 0 00 00 000 0 0 00 00 0 000 00 000 0 0 00 0 0 0 00 000 0 00 00 000 0 00 00 00 0 0 00 00 0 00 00 0000 0 0 00 0 0 0 00 000 0 0 00 0 0 0 00 0 0 0 00 0 0 00000 00 00 0 00 00 0 0 00 00 000 0 0 00 0 0 0 00 00 0 0 00 00 0 0 00 00 0 000 00 0 0 0 00 000 0 000 00 00 0 00 00 0 0 0 00 000 0 00 00 0000 0 0 00 0 0 0000 00 00 0 0 00 0 0 00 00 00 0 0 00 0 0 0 00 00 0 0 00 0 0 0 00 0 0 00 00 0 0 00 00 000 0 0 00 000 0 0 00 000 0 00 00 00 0 0000 00 0000 0 00 00 0 0 0 00 0 0 0 00 0 0 00 00 0000 0 0 00 0 0 00 00 00 0 000 00 0 0 0 00 00 0 0 00 00 0 0 00 00 0 00 00 0 0 0 00 0 0 0 00 0 0 000 00 00 0 00 00 0 0 00000 00 0 0 0 00 00 0 0000 00 0 0 0 00 00 0 0 00 0 0 0 00 0 0 00 00 00 0 000 00 0 0 00 00 00 0 000 00 00 0 0 00 00 0 0000 00 0000 0 00 00 00 0 0 00 00 0 00 00 000 0 0 00 00 0 000 00 000 0 0 00 0 0 0 00 0000 0 0 00 000 0 00 00 0 0 0 00 000 0 0 00 00 0 0 00 0000 0 00 00 0 0 00 00 000 0 00 00 0 0 00 00 00
```

Cet encodage est un encodage un peu troll et se nomme le [Code Unaire Chuck Norris](https://www.dcode.fr/code-chuck-norris)

Car Chuck Norris n'a besoin que deux touches pour encoder ses messages, le 0 et la barre espace.

Le codage ASCII est sur 8-Bit.

#### 2. Une fois décodé on se retrouve avec cette nouvelle chaîne

```
~wy@5ad`|(EB*?=b4?uC4(5A+a=I|%#C+)y@+>hG|a==+;9<4>gK|aAd}(#=3aEG2>&_5(}I3?'?5K'J4Ku_6;9:2?'=4vcc2>u@5b5G5s}=4;#>6%uF2aEd2v+G*K#E+)q?2('_5s}?2(y<+)#C4(5=}w5F5)#K+b#=4?4I|(h?|K9<4;tK*(AH6)'?4(@K+bq?5K"I|(yC2?=b2vhB5aEB*?5b3aEF~v+:+vEG2aEC5vd<3b#:6>5_3)5b|%u>~vxc+wy`5vuB*%}J+buB|a5;|b5F|(xK2>Ad2(5;2buB2(+A+b'_|a5J}v#C3aEI+(+d5adI2>=B2(yb2su_4a'>3>#;5(AK2?qC4>EI2b'?5s9J4)&I*>AA6)5G4vEH2axc4>db|auB2(E<2bqF2aE_6)'G4aye+b#<5agI5s}=+;9<2bqB4Hll
```

Il s'agit ici d'un chiffrement [ROT-47](https://www.dcode.fr/chiffre-rot-47)

Ce code utilise un « alphabet » de 94 caractères (les caractères 33 à 126 du code ASCII) constitué de lettres minuscules, de lettres majuscules, des chiffres 0 à 9, et de divers signes et symboles.

Il était donc reconnaissable à la présence de certains caractères spécifiques.

#### 3. Maintenant il y a un air de déjà vu sur la suivante

```
OHJod251MWtqYnl3cnFrcWdpZ2lxMTRrZXJoZm9vM2llZjhkcm8zM2p5NWRlb2tvamU0dWNxbnVndzVyczF0ejhianVlcG44amFod3dvdDNlcjRmeTFua2t5aGZvYzRtZXBnaWV0dDNnaWJkZXRrcWdlNHdudXRzZ3RlcncxMW9nMzhkcjEzYWpweXVncWozZ3BndzQxMWJranl3aG9qd2tqYnd3b2tuOGZiZGtva2trdG5kb3Riemd0bXd3MTFmOGI4ZHJ1dGFqYTNyZ3FqM2djM3duMWIzamp5aWdja3FqaWZpZ3V0M2dyNGRrb2txZWZ5d25xamlqaWJ3aDF0c2VmbmRjdWpzanBrcmtxa3VndDhycXUxYmppeXdvcGtwa2I4cm53M2FqaWtka3Bua2t0eXVvc2J6Z3Rkd28xdDNlZjhka3Bqcw==
```

Avec le double égal a la fin, il s'agit bien du [Base64](https://www.dcode.fr/code-base-64)

Ce code se reconnaît au fait que le message codé est constitué d’un mélange de lettres majuscules et de lettres minuscules, avec également quelques chiffres, et de rares signes : + / =

Il est l'un des encodages les plus courants.

#### 4. On reste dans le Base quelque chose mais cette fois-ci avec un petit twist

```
8rhwnu1kjbywrqkqgigiq14kerhfoo3ief8dro33jy5deokoje4ucqnugw5rs1tz8bjuepn8jahwwot3er4fy1nkkyhfoc4mepgiett3gibdetkqge4wnutsgterw11og38dr13ajpyugqj3gpgw411bkjywhojwkjbwwokn8fbdkokkktndotbzgtmww11f8b8drutaja3rgqj3gc3wn1b3jjyigckqjifigut3gr4dkokqefywnqjijibwh1tsefndcujsjpkrkqkugt8rqu1bjiywopkpkb8rnw3ajikdkpnkktyuosbzgtdwo1t3ef8dkpjs
```

Il s'agit ici du [Z-Base-32](https://www.dcode.fr/code-z-base-32)

Le codage z-base-32 est une variante de la base 32 (norme RFC 3548) proposée par Zooko O'Whielacronx et censée optimiser l'écriture et la lecture par les humains. Le code z-base-32 utilise 32 caractères ybndrfg8ejkmcpqxot1uwisza345h769 soit les 36 caractères alphanumériques excluant 4 caractères pouvant être confondus avec d'autres : 0,l,v,2.

#### 5. Encore une ?

```
99ANJHAB9N5MWKJA8XC5AN2C9H64APJ568S56KJ78S44GN9JB9A4PHJP8X3KCMTF95B4EN25AN64PJJP6N2K8KA3993MMJARANA4RCJAB9B5AJTD8D74WJJE8N2N8N2C9933AH9JAS1NMKSN9145ANAAA95MCNJ6AD6M6KTE9S4NGNAMAH5MPNAS8MT54JTA8X74GHJ9AN556
```

Encore une version du Base-32 qui cette fois-ci se nomme [Base-32 Crockford](https://www.dcode.fr/code-base-32-crockford)

La base-32 imaginée par Douglas Crockford est une variante de la base 32 voulant optimiser l'écriture et la lecture par l'homme et y ajoutant une somme de controle. La Crockford base-32 utilise 32 caractères 0123456789ABCDEFGHJKMNPQRSTVWXYZ soit les 36 caractères alphanumériques excluant I,L,O pour ne pas les confondre des chiffres et la lettre U ce qui permet d'éviter des jeux de mots (U=You).

#### 6. And another one ? Non

```
JUYEKMKNNJGXUTLLLEZE22SNGFHHU2ZTKFVGG6SOIVGTEULKJV5E4MCJGJIXUTL2JZVUKMCNNJNEETTLJF5E2VCZO5HHUUJRKFVFSMCONNIXUTTKKUYE4RKJGNHFIUJS
```

Cette fois-ci il s'agit bien du [Base32](https://www.dcode.fr/code-base-32) originiel et pas d'une variante.

Le code Base32 est une norme d'encodage pour faciliter la transmission de chaines binaires via 32 caractères de la table ASCII.

#### 7. Une variante du Base64

```
M0E1MjMzMkY2MjM1Nzk3QjczNEM2QjMzN0I2QzMzNkE0MjZBNkIzMTYwNzQ1QjY0NkQzNjU0NEI3NTQ2
```

Il s'aggit ici d'une variante du Base64 qui se nomme Base64URL. C'est une modification de la norme principale Base64, dont le but est la possibilité d'utiliser le résultat de l'encodage comme nom de fichier ou adresse URL.

#### 8. Plus on se rapproche du début, plus c'est simple

```
3A52332F6235797B734C6B337B6C336A426A6B3160745B646D36544B7546
```

Il s'agit ici du [Base-16 ou Hexadécimal](https://www.dcode.fr/systeme-hexadecimal)

L'hexadécimal est un système d'écriture de nombres en base 16, avec les symboles 0,1,2,3,4,5,6,7,8,9,a,b,c,d,e,f.

#### 9. Pas commun mais pas compliqué

```
:R3/b5y{sLk3{l3jBjk1`t[dm6TKuF
```

Il s'agit ici du [Base-91](https://www.dcode.fr/code-base-91)

Le code Base91 (ou BasE91) est une alternative à base64 mais avec un alphabet élargi à 91 caractères : les 94 caractères ASCII imprimables (de 0x21 à 0x7E) en omettant - : tiret (0x2D), \ : backslash (0x5C) et ' : apostrophe (0x27). Elle permet d'encoder n'importe quelle donnée binaire en une chaîne de caractères composée uniquement de caractères imprimables (et donc transmissible via les messageries texte, etc.)

#### 10. And the last one

```
UFE{Qb_Abg_Cerl_RAPELCG}
```

Là le format du flag apparait mais ce ne sont pas les bonnes lettres.

Il s'agit ici d'un chiffrement [ROT-13](https://www.dcode.fr/chiffre-rot-13)

Dans la même ligné que le ROT-47 vu précédement, ROT-13 combine l'alphabet français/latin de 26 lettres et un décalage de 13, il remplace une lettre par une autre située treize rangs plus loin dans l'alphabet.

## Flag 🚩

HSR{Do_Not_Prey_ENCRYPT}

## Contact 📲

whilsker sur discord
