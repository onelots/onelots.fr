---
title: "Bravo - Journey beyond the horizon"
date: 2024-03-30T12:19:16+01:00
draft: false
tags: ['Osint', 'ImInt', 'GeoInt']
categories:

- 'Writeups'
- 'EC2 2024'

---

{{< image src="/bravo/banner-bravo.png" caption="Fox Project & Ec2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2024 • Bravo

--- 

## Category :

> Osint 

## Description :

> Heading west, it seems that he took off from the previous location to meet a manufacturer of a robot factory, whose director has already been convicted of conflict of interest. The individual leaked this photo over the coast of north-west Africa. Find the name of the main town visible.
> 
> {{< image src="/bravo/img.jpg" caption="Challenge" title="Challenge" alt="Challenge" >}}



## Difficulty :

**EASY**

## Write up :

On va commencer par télécharger la photo, puis l'ouvrir.

Tout de suite, on se dit "eh merde, je vais jamais y arriver c'est de nuit..."

Puis on relit l'énoncé, et il est dit que la ville se situe au nord de l'Afrique.

en observant attentivement l'image, on peut voir qu'en fait l'endroit ressemble à un golf, en tout cas la côte a l'air sacrément courbée donc on cherche un endroit en forme de demie lune.



Armé de notre fidèle ami google maps, on s'aperçoit assez vite qu'un coin entre l'espagne et le Maroc ressemble fortement, à cela près que l'image n'est pas tout à fait bien orientée. 

À regarder de plus près, la forme du port correspond, l'emplacement de la ville aussi, la "pointe" en bas à gauche de la photo correspond également.



Bravo, c'est trouvé : on est à Ceuta.



{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `FLAG{Ceuta}`
{{< /admonition >}}
