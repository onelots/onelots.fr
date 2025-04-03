---
title: "Alexis Dumas"
date: 2024-04-10T00:54:27+01:00
draft: false
tags: ['Osint', 'MediaInt']
categories:

- 'Writeups'
- 'Bordeaux CTF by CTFREI'

---

{{< image src="/BordeauxCTF/AlexisDumas/AlexisDumas.png" caption="BordeauxCTF " title="Sujet" alt="Sujet" >}}

# Bordeaux CTF by CTFREI

---

## Category :

> Osint

## Description :

> One of your informants calls you for help, saying he's working on a suspect suspected of trafficking in robots. The individual has been seen at various locations. Find out where this person passed through.
> 
>  {{< rawhtml >}} 
> 
> <video width=100% controls autoplay>
>     <source src="/BordeauxCTF/AlexisDumas/video.mp4" type="video/mp4">
>     Your browser does not support the video tag.  
> </video>
> 
> {{< /rawhtml >}}

## Difficulty :

**EASY**

## Write up :

On télécharge donc la vidéo.

Assez vite, après plusieurs visionnages, on peut se rendre compte qu'il va être très difficile de localiser l'endroit par géoint.

On va donc vérifier les metadata.

L'outil exiftool nous donne des informations intéressantes : 

> {{< image src="/BordeauxCTF/AlexisDumas/exiftool.png" caption="Exiftool" title="Sujet" alt="Sujet" >}}

nous avons donc des coordonnées GPS, au format HMS (heures/minutes/secondes)

On peut donc les convertir dans un format lisible par google maps : 

44 deg 31' 12.72" N, 1 deg 10' 51.60" W => 44.5202, -1.1810

> {{< image src="/BordeauxCTF/AlexisDumas/maps.png" caption="Exiftool" title="Sujet" alt="Sujet" >}}

On a donc le flag :

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `CTFREI{La_Teste_de_buch}`
{{< /admonition >}}
