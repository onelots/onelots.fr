---

title: "SideQuest - Echos discordants"
author: "Onelots"
date: 2025-04-03T12:19:05+01:00
draft: false
tags: ['Osint']
categories:

- 'Writeups'
- 'EC2 2025'


---

{{< image src="/FIC2025/sidequest/sidequest.png" caption="Fox & Ec2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2025 • SideQuest - Echos Discordants

--- 

## Category :

> Osint 

## Description :

> Les notes dansent, les idées s'organisent... Notre homme laisse des traces dans sa vie numérique. Un message se cache là où mélodie et méthode se rencontrent. Parfois, l'ordre fait toute la différence. Qu'essaie-t-il de nous dire?

> Format du flag : deux mélodies - - - - - - deux mélodies

## Difficulty :

**GUESSY / EASY**

## Write up :

Ce challenge s'est démarqué particulièrement pour son caractère guessy et étrange dans la formulation de l'énoncée, raison pour laquelle les équipes ont préféré ne pas forcément s'attarder dessus ni donner de points pour avoir des hints.

Pour le résoudre, il fallait partir des challenges précédents et se souvenir que [Rajesh Devi possède un Notion](https://mahogany-shallot-cde.notion.site/Rajesh-Devi-s-personal-Notion-174e23272dd68036a383f4a04fdc7691). 

Arrivés sur ce Notion, on s'apercevait assez vite que Rajesh possède une [page complète dédiée à la musique](https://mahogany-shallot-cde.notion.site/My-music-page-1b2e23272dd68089b8bef3dc1b317e83)  
En même temps, l'énoncé disait "les notes dansent, les idées s'organisent". On part bien.

Le premier lien nous menait [vers une playlist spotify](https://open.spotify.com/user/31ldsfcs4zxgjeuumktp7dhfmpg4)

{{< image src="/FIC2025/sidequest/spoti-notion.png" caption="Spotify Notion" title="Notion" alt="Notion" >}}

C'est là que la partie guessy commence.  
Car oui, avoir une playlist spotify c'est chouette... Mais j'en fait quoi, moi ?

En descendant, on voit cette musique :

{{< image src="/FIC2025/sidequest/musique-chelou.png" caption="Musique spotify rajesh" title="MSC" alt="MSC" >}}

Si on se souvient bien, le flag est dans un format `deux mélodies - - - - - - deux mélodies`

On est donc aiguillés quant à ce qu'il faut faire : utiliser les musiques pour construire le flag.  
Mais là... il y a 75 chansons dans la playlist. Je ne vais pas faire toutes les combinaisons.

En relisant l'énoncé, cette phrase m'interpelle : **Parfois, l'ordre fait toute la différence.**

Essayons.

En jouant avec le tri des musiques, on finit par tomber sur un semblant de phrase : 

{{< image src="/FIC2025/sidequest/spotify.png" caption="Ordre des musiques spotify" title="ordre" alt="ordre" >}}

Mouais... Pas convaincu. Mais en essayant ça fonctionne.  
Voilà pourquoi je dis que ce challenge était un brin guessy... C'est vraiment bizarre de devoir jouer avec spotify comme ça, d'autant plus qu'on ne peut modifier l'ordre que sur l'application de bureau... Enfin bref

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `FLAG{Here's to You The Flag - - - - - - - Breach Security}`
{{< /admonition >}}
