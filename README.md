# FCSC 2021 Suspicious SMS

En analysant le trafic entre mon téléphone et le réseau, j’ai détecté un SMS de classe 0. Ce SMS contient des instructions pour installer un applet Java Card sur ma carte SIM.

Je vous ai extrait le contenu de l’applet (<code>jc_dump.bin</code>). Cela ressemble à du Java Card 3.0.1. Notre expert étant absent, nous ne pouvons pas le solliciter.

Une fois cet applet installé, j’ai découvert que des APDUs chiffrés étaient échangés entre la carte SIM et le réseau opérateur. J’ai détecté cette réponse APDU, mais je n’ai pas pu capter le début des échanges. Son contenu semble chiffré.

<code> 
C6 5F 56 69 08 F8 A0 4A 4D CE 35 C0 1A 4B B2 AB 29 D4 1C FC EA 3D FF 7E 97 E3 42 F6 4F 60 27 14 9C C7 83 4A 04 F9 D7 C2 DE 8F 35 0E 96 77 09 6F 81 EA D0 CD 09 FB BE 74 58 D7 FE 45 2D 9D A4 43 11 87 63 31 24 EF 65 3D 6E 55 DF 54 34 AC E0 A5 90 00
</code>


Pouvez-vous retrouver le secret caché ?



Fichier : [jc_dump.bin](jc_dump.bin)



Auteur : _Stroumph

Origine : [Suspicious SMS](https://hackropole.fr/fr/challenges/hardware/fcsc2021-hardware-suspicious-sms/)




-----------

## Installation manuel
Vous n'utilisez pas l'application **les CTFs de Cyrhades** ? C'est dommage !
Mais voici comment installer ce CTF manuellement :

> git clone https://github.com/Hack-Oeil/fcsc2021-hardware-suspicious-sms.git

> cd fcsc2021-hardware-suspicious-sms


-----------

## Sur le site officiel hackropole.fr
> https://hackropole.fr/fr/challenges/hardware/fcsc2021-hardware-suspicious-sms/