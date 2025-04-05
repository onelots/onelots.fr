---
title: "Retour aux sources"
author: "Onelots"
date: 2024-04-28T23:39:16+01:00
draft: false
tags: ['Crypto', 'RSA']
categories:

- 'Writeups'
- 'MidnightCTF'

---

# MidnightCTF • 2024 •

--- 

## Category :

> Crypto 

## Description :

> Voilà les fichiers qui étaient fournis :
> 
> Source.py et Outpout.txt.
> 
> Il faut se baser sur ces deux fichiers pour résoudre le challenge.

## Source.py :

```py
from Crypto.Util.number import getPrime, bytes_to_long
import math
from super_secret import flag

m = bytes_to_long(flag)

z = []
for hey in range(1024**(0)):
    z.append(getPrime(1024))

n = math.prod(z)

e = 0x100001

with open('output.txt', 'w') as f:
    f.write(f'{n = }\n')
    f.write(f'{e = }\n')
    f.write("c =" + str(int(pow(m, e, n))))
```

## Output.txt:

```py
n = 120154269905138192411391191398976535526719518763614629012467119791158898243636581028193617198308072414473675597119386635758833912767888946461927038930309978578151909912247022109956454047808157443912106603576628133516080238431851987309829049482974245755557890602608533798942465700524674017649586964749795503907
e = 1048577
c =112131769061863157582206902794706307787376441536475925637794499610352216277884266668233852165255435484902059092228094627632502452075609345890718955546331647782141352807558391026039060334176952276306678953561089609897886575688921388228876952827334853010664153370817811056441329533096065098137670506655501321060
```

## Difficulty :

**EASY**

## Write up :

Dès l'ouverture du fichier .py, on se rend compte qu'il s'agit d'un challenge tout simple de RSA.

On écrit un programme python tout simple et rapide pour déchiffrer ce qui a été déchiffré :

```py
from Crypto.Util.number import inverse, long_to_bytes

# Valeurs fournies
n = ...  # valeur de n
e = 0x100001
c = ...  # valeur de c

# Calcul de l'exposant de déchiffrement (d)
phi_n = n - 1  # As the prime factors are prime numbers, phi(n) = n - 1
d = inverse(e, phi_n)

# Déchiffrement du message
m = pow(c, d, n)

# Conversion du message déchiffré en chaîne de caractères
plaintext = long_to_bytes(m)

print(plaintext.decode())
```

{{< admonition type=success title="Flag" open=false >}}
:triangular_flag_on_post: `MCTF{SCRIPT_ENCODER}`
{{< /admonition >}}

