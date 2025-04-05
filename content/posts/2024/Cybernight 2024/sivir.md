---

title: "Mon Champion Préféré"
author: "Onelots"
date: 2024-11-23T10:50:00+01:00
draft: false
tags: ['Web', 'Cybernight']
categories:

- 'Writeups'
- 'Cybernight'


---
{{< image src="/cybernight/sivir/cybn.png" caption="Cybernight 2024" title="Sujet" alt="Sujet" >}}

# Cybernight 2024 - Web - Intro

--- 

## Category :

> Osint 

## Description :

> Tu joues à league of legends ? Moi, je joue à league of legends.
> D'ailleurs, je main Sivir. C'est un champion que je trouve incroyable mais... ses stats ne lui rendent pas service, je trouve. Du coup, j'ai créé un site qui permet de patch son champion.
> Aide moi à patch Sivir pour qu'elle soit la meilleure du jeu !
> Note : dans un jeu, patch un champion signifie lui augmenter ou lui baisser ses stats.
> Auteur : Onelots
> 
>  {{< image src="/cybernight/sivir/img.png" caption="Preview du site" title="Sujet" alt="Sujet" >}}

## Difficulty :

**Intro**



## Write up :

On arrive donc sur un site qui nous permet de patch notre champion. On en fait très rapidement le tour, quelques boutons, et un gros bouton principal.

Directement, le premier réflexe est de jouer avec les possibilités, et surtout d'appuyer sur le bouton "patch".

Si on fait ça, on a une fenêtre qui nous informe que le champion a été "patché."

{{< image src="/cybernight/sivir/patched.png" caption="Le champion a été patché" title="Sujet" alt="Sujet" >}}

Mais rien de concret ne se passe.
Immédiatement, on pense à regarder le code source de la page et on peut aussi observer ce qu'en dit l'onglet réseau.  
On s'aperçoit que lorsque le bouton "patch" a été cliqué, une requête "post" est envoyée sur un endpoint "/patch-the-champ".

{{< image src="/cybernight/sivir/rezo.png" caption="Requête POST" title="Sujet" alt="Sujet" >}}

On voit aussi dans le code que, outre les scripts inutiles d'incrémentation des stats (boutons factices, de façon évidente), il y a un script très intéressant qui envoie la requête.

{{< image src="/cybernight/sivir/code.png" caption="Script" title="Sujet" alt="Sujet" >}}

Cela dit, on nous demande de "patch" le champion, mais on ne voit qu'une request POST.  
En HTTP, il y a un concept très intéressant qui est les [méthodes HTTP.](https://fr.wikipedia.org/wiki/Hypertext_Transfer_Protocol#:~:text=Dans%20le%20protocole%20HTTP%2C%20une,le%20nom%20de%20la%20m%C3%A9thode.)

On peut donc essayer de changer la méthode de la requête. En regardant la liste des méthodes, on s'aperçoit d'une méthode `PATCH`.
Intéressant, non ?

On peut essayer de refaire la request sur le même endpoint, mais en utilisant la méthode `PATCH`.

{{< image src="/cybernight/sivir/methode.png" caption="Requête PATCH" title="Sujet" alt="Sujet" >}}

Hop magnifique !!! le flag !

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `CYBN{J3_P4TCH_C0MM3_UN_D13U}`
{{< /admonition >}}
