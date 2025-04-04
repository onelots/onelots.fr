---

title: "RonRon"
date: 2025-04-03T12:19:00+01:00
draft: false
tags: ['Osint']
categories:

- 'Writeups'
- 'EC2 2025'


---
{{< image src="/FIC2025/ronron/ronron.png" caption="Fox & Ec2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2024 • Alpha

--- 

## Category :

> Osint 

## Description :

> Lors d'une soirée dans un café prisé, vous tendez l'oreille pour écouter une conversation derrière vous. Une femme se vante d'être parvenue à prendre le contrôle à distance de la puissance moteur d'avions de tourisme, avec un complice dans une entreprise de maintenance aéronautique. Mais elle a arrêté après que l'un des avions piraté se soit écrasé. Cela semble être un bon tuyau, pour cibler les avions ou pour faire chanter son complice, ça sera suivant votre hummeur...

Debut de votre enquête. Vous vous intéressez à l'avion le plus produit au monde. Quel est le numéro d'article du moteur qui équipe l'appareil lors de la révision, en français, de 2006 ?

Format du flag : 01-02-A

## Difficulty :

**EASY**

## Write up :

Le challenge n'était pas SI compliqué que ça, il était même carrément facile par certains aspects.
Il s'agissait de savoir lire.

Pour commencer, il fallait trouver **quel avion** a été le plus produit au monde.  
On imagine que l'on parle des avions de tourisme, donc une recherche rapide nous apprend qu'ils s'agit du `CESSNA 172` (dans toutes ses déclinaisons, de `172A` à `172S`)

Une fois cette information en notre possession, nous n'avions plus qu'à faire une recherche pour trouver le manuel de l'avion (le 172S en l'occurence, vu qu'on est en 2006...)

Assez vite on tombait sur [ce manuel-ci](https://www.casgac.com/fichiers/data/club/manuels/Manuel_Cessna172S.pdf)

En effet, il a l'air de correspondre ! on nous parle de **La révision, en français, de 2006**

Contrairement à ce que nous avons cru, lorsque l'énoncé parlait de révision, il ne s'agissait pas de la révision mécanique, mais de la version du manuel !

Nous avons donc ce manuel : 

{{< image src="/FIC2025/ronron/manuel.png" caption="Fox & Ec2" title="Manuel d'utilisation" alt=""Manuel d'utilisation" >}}

Ce pdf n'étant qu'un scan de pages, il n'est donc pas possible de ctrl + f.
On se dirige donc vers la table des matières, puis à la page 202 pour consulter la liste des équipements.

Et page 203, on trouve une ligne particulièrement intéressante : 

{{< image src="/FIC2025/ronron/moteur.png" caption="Fox & Ec2" title="Info moteur" alt="Info moteur" >}}

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `FLAG{72-03-R}`
{{< /admonition >}}






