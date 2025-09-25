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
 
En primer lloc, he creat una partició per al EFI. La partició de l'EFI es necessària si estem utilitzant UEFI, ja que s'encarrega de fer funciomar el carregador d'arranc del sistema operatiu. Aquesta partició s'utilitza com Ext4 o FAT32 perqué és compatible amb tamanys de discs petits, i per a l'EFI no necessitem més de 512 MB.

![](./imatges/EFI.png)

## Llicenciament
## Gestors d'arrencada per a instal·lacións DUALS
## Punts de restauració
## Configuració de la xarxa
## Comandes generals i instal·lacions
