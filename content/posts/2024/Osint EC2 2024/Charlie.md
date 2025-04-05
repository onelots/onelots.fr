---
title: "Charlie - Journey beyond the horizon"
author: "Onelots"
date: 2024-03-30T12:19:00+01:00
draft: false
tags: ['Osint', 'ImInt', 'GeoInt']
categories:

- 'Writeups'
- 'EC2 2024'

---

{{< image src="/Charlie/banner-charlie.png" caption="Fox Project & Ec2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2024 • Charlie

--- 

## Category :

> Osint 

## Description :

> The individual headed for an archipelago and was spotted on the edge of a puddle with a robot at his side, the same type used by the police. Find out his name.
> 
> {{< image src="/Charlie/Charlie.jpg" caption="Charlie" title="Charlie" alt="Charlie" >}}

## Difficulty

**Medium**

## Write up :

Comme à chaque fois, nous allons commencer par télécharger la photo, puis l'ouvrir.

en voyant la photo, il peut y avoir un petit instant de panique. C'est normal.

Nous avons donc une photo, de nuit, de ce qui semble être un lac ou peut-être un bord de mer. On va donc creuser par là.

>  ⚠️ On voit que l'eau est extrêmement calme donc soit c'est un lac soit c'est un port ⚠️

N'oublions pas qu'il s'agit d'un <u>_archipel_</u>, comme mentionné dans l'énoncé. 

> On a vu dans [Bravo](https://onelots.fr/posts/2024/bravo/bravo/) que l'homme était passé au dessus de Ceuta, et qu'il venait de Genève. On peut donc supposer qu'il ne sera pas dans les baléares, qui sont entre les deux. 

Descendons un petit peu donc.

On peut éliminer les Baléares et réstreindre le champ de recherches

| Archipel | Probabilité |
|:--------:|:-----------:|
| Baléares | ❌           |
| Açores   | ✅           |
| Canaries | ✅           |
| Cap vert | ✅           |

C'est là que ça devient intéressant. 

Dans l'énoncé il est écrit "Puddle", soit flaque en français

....

C'est bizarre, nan ? même en anglais, qui appelle un bord de lac/mer "une flaque ?"

Je ne me suis rendu compte de ça qu'après un petit bout de temps à chercher, et c'est là toute la subtilité de ce challenge.

💡 • En **espagnol**, flaque se dit "<u>charco</u>"

Je me suis rendu compte de ce détail un peu au hasard, je n'ai pas d'explication sur le pourquoi du comment, c'est un "éclair de génie" que j'ai eu après un certain temps passé à ne rien trouver.

les *Açores* sont portugaises, donc on peut également les enlever.

Il ne nous reste que les Canaries et le Cap Vert.
À savoir que bien qu'ispanophone, le Cap Vert est tout de même très loin de Genève donc je l'avais ignoré. Il me semblait vraiment éloigné du champ de recherches, donc j'ai préféré éviter de m'éparpiller et l'ai mis de côté quelques instants.


À partir de là, en tapant "Charco" dans google maps, on voyait apparaître un certain nombre de résultats :

> {{< image src="/Charlie/charco.png" caption="Charco maps" title="Charco" alt="Charco" >}}



J'ai donc commencé à regarder les photos de chaque résultat, jusqu'à voir un intriguant "El Charco" avec 2 photos. 

En cliquant, je suis tombé sur quelquechose très intéressant :

> {{< image src="/Charlie/beatriz.png" caption="Beatriz" title="Beatriz" alt="Beatriz" >}}

Eh oui ! en zoomant... Le bâtiment au fond correspond, la forme du port aussi, les palmiers à gauche... ça semble être là !

> {{< image src="/Charlie/zoom.png" caption="Zoom" title="Zoomed" alt="Zoomzs" >}}

Bien, mais malheureusement, l'image ne correspond pas au lieu exact.

Un coup de google lens sur cette image :

> {{< image src="/Charlie/lens.png" caption="Lens" title="Lens" alt="Lens" >}}



Les premiers résultats sont les bons !

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `FLAG{Charco_de_san_gines}`
{{< /admonition >}}


