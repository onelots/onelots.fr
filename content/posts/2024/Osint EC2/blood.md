---
title: "Blood - Law breaker"
date: 2024-03-31T00:51:00+01:00
draft: false
tags: ['Osint']
categories:

- 'Writeups'
- 'EC2 2024'

---

# Projet FOX • EC2 2024 • Blood

--- 

## Category :

> Osint 

## Description :

> A colleague remembers some information that seemed minor to him. He tells you that during the investigation, your colleague Zohra wanted to re-examine a piece of evidence, she handled one without protection and injured herself with it. After being treated in hospital, she has received the results of a blood test, which she has apparently saved on the work environment's common space.
> 
> Analyse it in depth to identify the illness she suffered from.
> 
> {{< pdfReader "/blood/blood.pdf" >}}

## Difficulty

**Easy**

## Write up :

Ce challenge était honnêtement extrêmement simple. Je sais que certaines personnes y ont passé un certain temps... Il suffisait de ne pas réfléchir.

Quelle maladie un peu crade peut s'attraper en manipulant des objets et en se blessant avec ? Personellement, seul le tétanos me vient à l'esprit... ça, c'était ma déduction.

Cela dit, j'ai donné le pdf à ChatGPT. voilà sa conclusion : 

> {{< image src="/blood/bloodgpt.png" caption="Rapport médical Zohra" title="rapport" alt="Rapport Zohra" >}}



Le résultat est sans appel 😂 le docteur chatGPT est de mon avis



La maladie est donc le tétanos, `tétanus` en anglais.



{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `FLAG{tetanus}` {{< /admonition >}}






