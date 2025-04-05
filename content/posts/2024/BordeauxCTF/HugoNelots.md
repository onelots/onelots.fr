---
title: "Hugo Nelots - Prélude"
author: "Onelots"
date: 2024-04-10T00:54:30+01:00
draft: false
tags: ['Osint', 'SocialInt']
categories:

- 'Writeups'
- 'Bordeaux CTF by CTFREI'

---

{{< image src="/BordeauxCTF/HugoNelots/HugoNelots.png" caption="BordeauxCTF " title="Sujet" alt="Sujet" >}}

# Bordeaux CTF by CTFREI

--- 

## Category :

> Osint 

## Description :

> 31/02 2024. Vous êtes dépêché au 83 Rue Lucien Faure. En effet, au 3eme étage de l'entreprise Effraye, gisant dans son sang, vous trouvez l'éminent chercheur en cyber et bio. Sur le sol, tracé en lettres de sang, vous pouvez lire le symbole "X". Vous décidez donc de vous lancer sur la piste du meurtrier... 
> 
> Trouvez les dernières paroles publiques de Hugo Nelots.
> 
> Format : CTFREI{dernières_paroles}
> 
> Par : Onelots.

## Difficulty :

**EASY**

## Write up :

À partir de l'énoncé, on sait que l'on doit chercher un certain Hugo Nelots.
Dans l'énoncé également, il est dit qu'il a tracé par terre un symbole : X

on va donc logiquement commencer par chercher sur X (twitter)

on tombe sur ce compte :

> {{< image src="/BordeauxCTF/HugoNelots/twitter.png" caption="Twitter (X)" title="Sujet" alt="Sujet" >}}

On a donc directement le flag : 

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `CTFREI{J3_n3_su1s_p4s_3n_s3cur1t3_1c1}`
{{< /admonition >}}
