---
layout: default
title: "Sprint 1: Instal·lació i configuració inicial"
---

## Virtualització i instal·lació del so Ubuntu

El primer que he fet ha sigut crear una màquina virtual. Per a saber les especificacions per la mateixa, he preguntat al chatGPT amb el meu cas específic quines serien les millors especificacions. En el meu cas, m'ha recomanat posar 8gb de memòria ram i 4 nuclis de cpu virtual.

![Imatge1](./imatges/Virtualitzacio_1.png)

A continuació, he asignat 80gb d'espai per a la màquina virtual.

![](./imatges/Disc.png)

-------------------------------

## Creació de les particions
 
En primer lloc, he creat una partició per al EFI. La partició de l'EFI es necessària si estem utilitzant UEFI, ja que s'encarrega de fer funciomar el carregador d'arranc del sistema operatiu. 
Aquesta partició s'utilitza com FAT32 o VFAT perqué UEFI només funciona amb aquest tipus. El tamany de 512 MB és suficient. 
El punt de muntatge està a: /boot/efi. Sense aquesta partició, el sistema no arrancaria en mode UEFI.

![](./imatges/EFI.png)

En segon lloc, he creat una partició per a al /root. Aqui es on viu el sistema operatiu, s'utulitza per emmagatzemar els programes, les llibreries, etc.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e69331cc-e0ce-4ad8-a189-eadf25ec3dce" />

En tercer lloc, asduiashdishadhasdad
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a6f062cb-eaa5-4cd9-8fbf-9ca7a3b6624a" />

I finalment, el /home
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a7149ad9-7fd5-44c7-8a2b-7a67bff6a8ed" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fb213c40-2ecf-4c5a-84bc-4056604309a5" />

## Llicenciament
## Gestors d'arrencada per a instal·lacións DUALS
## Punts de restauració
## Configuració de la xarxa
## Comandes generals i instal·lacions
