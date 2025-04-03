---
title: "Dr Octopus"
date: 2024-04-10T00:54:20+01:00
draft: false
tags: ['Osint', 'SocialInt']
categories:

- 'Writeups'
- 'Bordeaux CTF by CTFREI'
---

{{< image src="/BordeauxCTF/DrOctopus/DrOctopus.png" caption="BordeauxCTF " title="Sujet" alt="Sujet" >}}

# Bordeaux CTF by CTFREI

---

## Category :

> Osint

## Description :

> Arrivé sur place avec Interpol, l'oiseau s'était déjà envolé. Encore.  
> Cependant, le téléphone dans votre poche vibre. Ce n'est pas le votre, c'est celui d'Alexis !!!   
> Vous recevez une notification : "Alexis, Dependabot updates for march"
> 
> Trouvez le flag  
> format : CTFREI{}
> 
> Par : Onelots.

## Difficulty :

**EASY**

## Write up :

Directement, sans même vous poser de question, vous avez lu le mot Dependabot : direction github.

Pour ceux qui auraient la chance de ne pas se faire spam par les mails github dependabot, il s'agit d'un outil automatisé qui vous avertit régulièrement si votre code possède des vulnérabilités ou pas.

De plus, le nom __docteur octopus__ (en référence à la pieuvre, symbole de GitHub) était également un indice.

On se dirige donc vers Github.

Dans la barre de recherche, on tape Alexis Dumas

Rien n'apparaît au premier abord mais, oh surprise ! dans la catégorie "users" à gauche, deux résultats :

> {{< image src="/BordeauxCTF/DrOctopus/githubusers.png" caption="Utilisateurs github" title="Sujet" alt="Sujet" >}}

En cliquant sur un des utilisateurs, on tombe sur cette page, où un repo flag est clairement indiqué :

> {{< image src="/BordeauxCTF/DrOctopus/dumasgit.png" caption="Git Alexis Dumas" title="Sujet" alt="Sujet" >}}

Dans le repo, un flag et des phrases mystérieuses apparaissent :

> {{< image src="/BordeauxCTF/DrOctopus/bizarre.png" caption="Repo du flag" title="Sujet" alt="Sujet" >}}

On voit donc que c'est... bizarre... Alexis parle en anglais et semble devenir fou...

Mais au moins, on a le flag :

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `CTFREI{PL34S3_F1ND_M3_1_C4NT_ST0P_MYS3LF}`
{{< /admonition >}}
