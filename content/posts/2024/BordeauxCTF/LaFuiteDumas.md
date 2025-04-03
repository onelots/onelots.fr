---
title: "La fuite Dumas"
date: 2024-04-10T00:54:25+01:00
draft: false
tags: ['Osint', 'ImInt']
categories:

- 'Writeups'
- 'Bordeaux CTF by CTFREI'
---

{{< image src="/BordeauxCTF/LaFuiteDumas/LaFuiteDumas.png" caption="BordeauxCTF " title="Sujet" alt="Sujet" >}}

# Bordeaux CTF by CTFREI

---

## Category :

> Osint

## Description :

> Vous avez découvert qu'Alexis Dumas a menti. Mais Pourquoi ? En attendant, un informateur vous apprend qu'il a fui en Espagne et qu'il cherche à rejoindre l'Algérie par bateau. De plus, l'informateur en question a réussi à obtenir une photo satellite de l'endroit dont compte partir Alexis Dumas.
> 
> Retrouver la ville de départ : CTFREI{ville}
> 
> Par : Onelots.
> 
> {{< image src="/BordeauxCTF/LaFuiteDumas/img.png" caption="Sujet" title="Sujet" alt="Sujet" >}}

## Difficulty :

**EASY**

## Write up :

Après ouverture du document, on voit une simple image satellite d'un port. Rien de bien intéressant.

D'ailleurs, google lens/yandex/bing images etc ne nous donnent aucun information

C'est là qu'intervient une notion que j'ai personnellement peu vue en osint : __les routes maritimes.__

De fait, lorsqu'on regarde google maps au dessus de la mer méditérannée, on remarque ces lignes bleues sur l'eau :

> {{< image src="/BordeauxCTF/LaFuiteDumas/lignes.png" caption="Lignes bleues dans l'eau" title="Sujet" alt="Sujet" >}}

En partant de là, on voit qu'il ne reste que 3 ports possibles : 

- Motril

- Almeria

- Alicante

En zoomant sur chacun, et en comparant, on obtient rapidement le flag.

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `CTFREI{Almeria}`
{{< /admonition >}}
