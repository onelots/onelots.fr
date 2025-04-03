---
title: "Foxtrot - Journey beyond the horizon"
date: 2024-04-05T00:26:00+01:00
draft: false
tags: ['Osint', 'ImInt']
categories:

- 'Writeups'
- 'EC2 2024'

---

{{< image src="/foxtrot/Foxtrot.png" caption="Projet Fox & EC2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2024 • Foxtrot

--- 

## Category :

> Osint 

## Description :

> The individual found on his way an antiques dealer in a pick-up truck . He published a photo of a well-guarded site. Find out his name.
> 
> {{< image src="/foxtrot/img.jpg" caption="Sujet" title="Sujet" alt="Sujet" >}}

## Difficulty :

**EASY**

## Write up :

En ouvrant l'image, j'ai tout d'abord cru avoir affaire à une archive datant de la guerre d'Algérie, étant donné qu'elle était en noir et blanc.
Puis la BMW en fond m'a convaincu que non.

Examinons donc l'image.
En fond, nous voyons une sorte d'arche de triomphe miniature, en tout cas on dirait une ruine. (romaine ?)

On voit aussi qu'elle est en contrebas par rapport à la route, et qu'il y a un parlmier devant le pilier gauche.



Faisons une recherche google images :



{{< image src="/foxtrot/lens.png" caption="Google Lens" title="Sujet" alt="Sujet" >}}



Dès les premiers résultats, on se rend compte que l'image tombe directement :



{{< image src="/foxtrot/lensentoure.png" caption="Google Lens 2" title="Sujet" alt="Sujet" >}}



On en déduit donc que l'individu se trouve près de l'arche de Marc Aurèle.

On a donc le flag :



{{< admonition type=success title="Flag" open=false >}}

:triangular_flag_on_post: `FLAG{Archus_of_marcus_aurelius}`

{{< /admonition >}}





