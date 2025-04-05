---

title: "Quien Es ?"
author: "Onelots"
date: 2025-04-04T12:20:00+01:00
draft: false
tags: ['Osint', 'Socmint']
categories:

- 'Writeups'
- 'EC2 2025'
- 'Bravo 2025'


---

{{< image src="/FIC2025/quienes/quienes.png" caption="Fox & Ec2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2025 • Quien Es ?

--- 

## Category :

> Osint 

## Description :

> Uthen Chaithiang, un expert en blockchain indien, est réputé pour ses compétences exceptionnelles dans le domaine des technologies décentralisées. Cependant, il semblerait qu'il soit impliqué dans des activités notamment sur la blockchain. Ses transactions et ses interactions en ligne ont attiré l'attention de nombreux observateurs, mais ses intentions restent floues.
> Il faut percer le mystère entourant Uthen Chaithiang. Retrouvez le pseudonyme ou l'adresse liée à la création du projet. Cette information pourrait être la clé pour comprendre ses véritables motivations et ses activités sur la blockchain.

> Format du Flag : pseudonyme ou adresse crypto

## Difficulty :

**EASY**

## Write up :

La première chose à faire était bien évidemment d'effectuer une rapide recherche sur internet de `Uthen Chaithiang`. Une recherche simple comme celle-ci ne nous donnait rien, il fallait donc aller sur différents réseaux sociaux et chercher à la main.  
Assez vite, on se dirigeait sur twitter et, en cherchant `Uthen Chaithiang`, on tombait sur un profil plutôt convainquant.

{{< image src="/FIC2025/quienes/twitter.png" caption="Profil Twitter" title="Sujet" alt="Sujet" >}}

`https://x.com/U_Chaithiang339`.  
Cela dit, mis à part ce compte twitter, rien de plus. Rien associé à ce pseudo (`U_Chaithiang339`) ou rien d'autre sur Uthen sur internet.

Cela dit, il restait une dernière solution : faire une recherche inversée de la photo de profil (plutôt particulière) d'Uthen.  
Et là, bingo, on était relancé : 

{{< image src="/FIC2025/quienes/gimage.png" caption="Google Image" title="Sujet" alt="Sujet" >}}

On apprenait donc que cette image semblait liée aux cryptos.  
En fouillant un peu sur le site, et en cherchant un peu dans les cryptod liées à la page qu'on avait trouvée (on était tombés sur la page d'une autre crypto, différente de celle qu'on cherchait), on finissait enfin par découvrir une crypto dont le logo était exactement le même que la photo de profil d'Uthen.

{{< image src="/FIC2025/quienes/crypto.png" caption="Bharat" title="Sujet" alt="Sujet" >}}

Avec cette information en main, il ne nous restait donc plus qu'à aller sur le site "livre blanc" de Solana (Solscan) et de regarder les infos en rapport avec la crypto qu'on avait trouvé : le **$BHARAT**

Sur la page des infos, on avait notemment l'adresse du créateur : 

{{< image src="/FIC2025/quienes/solscan.png" caption="Solscan" title="Sujet" alt="Sujet" >}}

On n'avait plus qu'à copier l'adresse du créateur, et c'était flag.

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `J3jCRYi3UMEUuXK8QNVSFdpVPWXffZfTwnCv3iYFktMo`
{{< /admonition >}}
