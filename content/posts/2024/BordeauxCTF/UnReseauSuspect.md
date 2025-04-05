---
title: "Un réseau suspect"
author: "Onelots"
date: 2024-04-10T00:54:23+01:00
draft: false
tags: ['Osint']
categories:

- 'Writeups'
- 'Bordeaux CTF by CTFREI'
---

{{< image src="/BordeauxCTF/UnReseauSuspect/UnReseauSuspect.png" caption="BordeauxCTF " title="Sujet" alt="Sujet" >}}

# Bordeaux CTF by CTFREI

---

## Category :

> Osint

## Description :

> Vous l'avez retrouvé, mais trop tard... il a réussi à fuir en Algérie.
> 
> Cependant, vous ne lâchez rien. En faisant une perquisition chez lui, vous retrouvez un smartphone miraculeusement dévérouillé. Après une analyse Forensic par Mr Quenthein Vinsang, il ressort qu'il est absolument vide... Mais qu'il a été connecté à 1 seul réseau, appelé DJAWEB_1D80; il semblerait que ce soit le réseau de la résidence secondaire d'Alexis.
> 
> Retrouvez le nom de la rue dans laquelle habite Alexis Dumas.  
> Format de flag : CTFREI{nom_de_la_rue}
> 
> Par : Onelots.

## Difficulty :

**Medium**

## Write up :

Pour celui-ci, pas de secret.

Il fallait connaître ou trouver le bon outil.

De fait, le site [Wigle](https://wigle.net/) est vraiment utile lorsque l'on fait de l'osint; il permet de rechercher des lieux avec des adresses MAC, des SSID etc.

On va donc importer notre SSID dans le site, et faire une recherche.

> {{< image src="/BordeauxCTF/UnReseauSuspect/wigle.png" caption="Wigle" title="Sujet" alt="Sujet" >}}

On voit donc qu'en Algérie, il existe 2 endroits avec ce SSID : à Algers et à Oran (ça se voit pas sur l'image mais croyez moi :) )

De là, on sait de part le précédent challenge (La fuite Dumas) qu'il est parti d'Almeria; il est donc forcément à Oran donc on regarde à Oran.

On a donc la rue : 

> {{< image src="/BordeauxCTF/UnReseauSuspect/rue.png" caption="Rue" title="Sujet" alt="Sujet" >}}

Et par la même, le flag (qui, je le reconnais, était vraiment immonde) :

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `CTFREI{Shari'_al'arabi_Bin_Muhaydi}`
{{< /admonition >}}
