---

title: "Cuanto ?"
author: "Onelots"
date: 2025-04-04T12:22:00+01:00
draft: false
tags: ['Osint', 'Socmint']
categories:

- 'Writeups'
- 'EC2 2025'
- 'Bravo 2025'


---

{{< image src="/FIC2025/cuanto/cuanto.png" caption="Fox & Ec2" title="Sujet" alt="Sujet" >}}

# Projet FOX • EC2 2025 • Cuanto ?

--- 

## Category :

> Osint 

## Description :

> Uthen a malheureusement commis une erreur de "trading" qui lui a coûté sa place de top trader. Dans un moment de frustration, il a avoué qu'il avait un petit FOMO et a perdu une partie de ses gains. Ainsi il se pourrait qu'il eu une deuxième adresse, est-il possible de retrouver le montant du premier gain ?

> Format du Flag : $XXX,XXX.XX

## Difficulty :

**EASY**

## Write up :

On a vu dans la partie précédente ([Cliquez ici pour la lire](https://onelots.fr/posts/2025/osint-ec2-2025/quien_es/)) que notre homme était très étroitement lié au `$BHARAT`.  
On va donc partir d'ici pour remonter son deuxième compte.  

Sur Solscan, on n'obtient aucune info intéressante, mais on s'aperçoit que sur d'autre sites tels que [Birdeye](https://www.birdeye.so/), [dextools](https://www.dextools.io/app/en/solana/pair-explorer/3ZWMcogvgmzVcEo6DPMYuCZCfvDSJYsFpgygKpyba51E?t=1743870623425) ou encore [Photons AI](https://photon-sol.tinyastro.io/en/lp/3ZWMcogvgmzVcEo6DPMYuCZCfvDSJYsFpgygKpyba51E) on pouvait récupérer ce qu'on appelle les **TOP TRADERS**.

Ce qui est extrêmement intéressant pour notre cas, étant donné que la consigne dit clairement : "__Uthen a malheureusement commis une erreur de "trading" qui lui a coûté sa place de top trader__"

Ce qui veut dire qu'il n'est plus premier, par définition.

# [UNDER WORK...]

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `J3jCRYi3UMEUuXK8QNVSFdpVPWXffZfTwnCv3iYFktMo`
{{< /admonition >}}
