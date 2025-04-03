---
title: "Back to the bureau"
date: 2024-04-10T00:54:17+01:00
draft: false
tags: ['Osint', 'Steganography']
categories:

- 'Writeups'
- 'Bordeaux CTF by CTFREI'
---

{{< image src="/BordeauxCTF/BackToTheBureau/BackToTheBureau.png" caption="BordeauxCTF " title="Sujet" alt="Sujet" >}}

# Bordeaux CTF by CTFREI

---

## Category :

> Osint

## Description :

> One of your informants calls you for help, saying he's working on a suspect suspected of trafficking in robots. The individual has been seen at various locations. Find out where this person passed through.
> 
> {{< pdfReader "/BordeauxCTF/BackToTheBureau/sujet.pdf" >}}

## Difficulty :

**EASY**

## Write up :

Il y a plusieurs méthodes pour résoudre ce challenge.

### Méthode 1 - bourrin.

Un simple ctrl a + ctrl c copiait le flag dans notre clipboard vu qu'il ne s'agissait que de texte blanc sur fond blanc.

### Méthode 2 - bourrin aussi.

En passant le pdf dans un site, on pouvait en extraire les objets (et donc le texte contenu dedans.)

### Méthode 3 - Un peu moins bourrin.

Un simple `strings chall.pdf | grep CTFREI` nous donnait directement la réponse :

> {{< image src="/BordeauxCTF/BackToTheBureau/strings.png" caption="Strings | grep" title="Sujet" alt="Sujet" >}}

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `CTFREI{L3T'5_C0NTR0L_TH3_W0RLD}`
{{< /admonition >}}
