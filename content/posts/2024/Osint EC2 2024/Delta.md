---
title: "Delta - Journey beyond the horizon"
author: "Onelots"
date: 2024-03-30T12:19:00+01:00
draft: false
tags: ['Osint', 'GeoInt']
categories:

- 'Writeups'
- 'EC2 2024'

---

{{< image src="/delta/banner-delta.png" caption="Fox & Ec2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2024 • Delta

--- 

## Category :

> Osint 

## Description :

> According to your informant, the individual has returned to the continent. He is preparing to build a warehouse to store hijacked robots, and has posted an aerial shot of the place where he plans to set up shop.
> 
> Find out in which city he is located.
> 
> {{< rawhtml >}} 

<video width=100% controls autoplay>
    <source src="/delta/video.mp4" type="video/mp4">
    Your browser does not support the video tag.  
</video>

{{< /rawhtml >}}
## Difficulty

**Medium**

## Write up :

En théorie, ce challenge ne devait pas être très long, certaines personnes l'ont flag en 5 minutes. J'y aurai passé <u>un total de 14h.</u>
J'ai passé tout ce temps car j'ai choisi de me focus sur ce qu'on voyait au sol (le yin/yang, le terrain vague et le rond point).
Fort de ces informations, j'ai passé mon temps sur maps au lieu de chercher d'autres détails; C'est cela qui m'a fait passer 14h sur ce challenge.

Après avoir téléchargé la vidéo, on l'ouvre; Nous voyons un certain nombre d'éléments, lesquels étaient plus ou moins utile.

Récapitulons (J'imagine que vous avez visionné la vidéo) :

- Une ville qui a l'air d'être au maghreb, du moins en Afrique.

- Des montagnes en fond

- Une grue

- Un terrain un peu étrange (type parking) avec un Yin/Yang 

- Un terrain de foot

- Un terrain vague avec un manège, terrain vague qui aboutit sur un grand rond-point

- Un certain nombre de voitures

- Une séparation nette entre des bâtiments +- délabrés et des immeubles

Bien, à partir de ça on devrait pouvoir s'en sortir.

À savoir également que l'énoncé précise que la personne est revenue sur __le continent__, ce qui était vague. Après en avoir discuté avec les admins, il s'agissait bien du continent africain comme je le pensais.

> 👉 Vous avez lu [Charlie](https://onelots.fr/posts/2024/charlie/charlie/) ? si non, allez le lire. Si oui, vous savez que l'archipel était les Canaries, j'ai donc supposé qu'il était revenu au plus proche donc au __Maroc__ (c'est important !)

Après avoir discuté avec les créateurs du challenge et les joueurs, il y a eu deux techniques similaires utilisées. Je vous donnerai les deux.

### Technique 1 : Les grands bâtiments en fond.

Je n'aurais honnêtement jamais pensé à commencer comme ça mais... pourquoi pas. J'ai refait le challenge après coup en faisant comme ça et ça a fonctionné.

Cette technique consistait à se baser sur les <u>grands bâtiments blancs que l'on pouvait voir en fond</u> :

> {{< image src="/delta/zoomed.png" caption="Fond" title="Bâtiments" alt="Bâtiments" >}}

Ce type de bâtiment se voit très bien depuis le ciel (donc google maps). J'ai donc cherché les villes marocains avec des bâtiments similaires. 

J'ai fait par ordre de taille, suivant cette liste wikipedia : [Liste des grandes villes du Maroc par population — Wikipédia](https://fr.wikipedia.org/wiki/Liste_des_grandes_villes_du_Maroc_par_population)

Au bout d'un certain temps de recherche sur google maps, je suis tombé sur cet endroit :

> {{< image src="/delta/maps.png" caption="Maps" title="Maps" alt="Maps" >}}

Il s'avère que c'était l'endroit exact.

> {{< image src="/delta/ciel.png" caption="Vue ciel" title="Vue ciel" alt="vue ciel" >}}

*(Le flag sera donné après la 2eme méthode)*

### Technique 2 : Les taxis !

Cette technique est celle qui m'a fait perdre un temps fou pour pas grand chose.

Sur la vidéo, on voit un certain nombre de voitures de la même couleur, j'ai donc supposé qu'il s'agissait de taxis. Je sais qu'au Maroc, il existe un certain nombre de taxis de couleur différente en fonction de la ville qu'ils desservent (il y a une liste ici, dont je me suis servi : [Taxi au Maroc — Wikipédia](https://fr.wikipedia.org/wiki/Taxi_au_Maroc))

Sur la vidéo, je voyais des taxis **rouges**, j'ai donc parcouru toutes les villes possédant des taxis rouges.

> Ne trouvant pas, je me suis arrêté là et j'ai fait la première méthode.

Le problème est que les taxis n'étaient pas rouges, mais **oranges**; Cette toute petite différence faisait passer la liste des villes potentielles de 11 à 2 : Berkane ou Agadir.

On se dirigeait donc sur google maps et on trouvait le rond-point et le terrain vague... donc la ville.

> {{< image src="/delta/ciel.png" caption="Vue ciel" title="Vue ciel" alt="Vue ciel" >}}

### Edit : Technique 3 : Bing images...

Après avoir discuté avec d'autres joueurs, ils m'ont confié que Bing images fonctionnait très bien également...

> {{< image src="/delta/aled.png" caption="Solve frauduleux..." title="Solve frauduleux" alt="Solve frauduleux" >}}

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `FLAG{Agadir}`

{{< /admonition >}}



