---
title: "Echo - Journey beyond the horizon"
author: "Onelots"
date: 2024-04-01T02:08:00+01:00
draft: false
tags: ['Osint', 'ImInt', 'GeoInt']
categories:

- 'Writeups'
- 'EC2 2024'

---

 {{< image src="/echo/echo-banner.png" caption="Projet Fox & EC2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2024 • Echo

--- 

## Category :

> Osint 

## Description :

> An operation has been set up in conjunction with the Moroccan authorities to arrest him, but the individual left the city a few hours before the police arrived at his home. Feeling that he was now wanted, the individual crossed the border on a camel and found himself stranded in a hut on the shore. Find out the location.
> 
>  {{< image src="/echo/chall.jpg" caption="Sujet" title="Sujet" alt="Sujet" >}}

## Difficulty :

**EASY**

## Write up :

Après avoir ouvert la photo, on s'aperçoit qu'il s'agit d'une vue satellite d'un lieu.

 Deux méthodes possibles.

## Méthode 1 : google lens

En utilisant google lens, on retrouve l'endroit assez vite :

> {{< image src="/echo/lens.png" caption="Google Lens" title="Sujet" alt="Sujet" >}}

## Méthode 2 : chercher à la mano

Un autre joueur m'a fait remarquer qu'il suffisait de chercher les points d'eau à la sortie du maroc à la main :

> {{< image src="/echo/maps.png" caption="Google Maps" title="Sujet" alt="Sujet" >}}

Effectivement, après un certain temps de recherche on tombe sur cet endroit :

> {{< image src="/echo/lieu.png" caption="Google Lens" title="Sujet" alt="Sujet" >}}



On a donc le flag.

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `FLAG{Djorf_Torba}`
{{< /admonition >}}



