---
layout: default
title: "Sprint 1: Instal·lació i configuració inicial"
---

## 1. Virtualització i instal·lació del so Ubuntu

El primer que he fet ha sigut crear una màquina virtual. Per a saber les especificacions per la mateixa, he preguntat al chatGPT amb el meu cas específic quines serien les millors especificacions. En el meu cas, m'ha recomanat posar 8gb de memòria ram i 4 nuclis de cpu virtual.

![Imatge1](./imatges/Virtualitzacio_1.png)

A continuació, he asignat 80gb d'espai per a la màquina virtual.

![](./imatges/Disc.png)

-------------------------------

## 2. Creació de les particions
 
En primer lloc, he creat una partició per al EFI. La partició de l'EFI es necessària si estem utilitzant UEFI, ja que s'encarrega de fer funciomar el carregador d'arranc del sistema operatiu. 
Aquesta partició s'utilitza com FAT32 o VFAT perqué UEFI només funciona amb aquest tipus. El tamany de 512 MB és suficient. 
El punt de muntatge està a: /boot/efi. Sense aquesta partició, el sistema no arrancaria en mode UEFI.

![](./imatges/EFI.png)

En segon lloc, he creat una partició per a al /root. Aqui es on viu el sistema operatiu, s'utulitza per emmagatzemar els programes, les llibreries, etc.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e69331cc-e0ce-4ad8-a189-eadf25ec3dce" />

En tercer lloc, el SWAP. És un espai virtual reservat per a quan s'ompli la memòria ram del sistema. Evita que el sistema es bloqueji si s'avaba la RAM.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a6f062cb-eaa5-4cd9-8fbf-9ca7a3b6624a" />

I finalment, el /home, que es la carpeta personal de cada usuari (archius, documents, descargues, configuracions).
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a7149ad9-7fd5-44c7-8a2b-7a67bff6a8ed" />

----------------------
## 3. Comparativa dels dieferents SO

Hi ha molts tipus de sistemes operatius, però hem centraré en els tres més principals: Windows, Linux i macOS. Cadascún d'ells ha estat especificament dissenyat per a diferents funcions. A més, els seus tipus de llicència poden variar molt entre ells.

Per exemple, Windows és el sistema operatiu més utilitzat tant en l'entorn domèstic com empresarial. Ofereix una interfície gràfica intuïtiva i una gran compatibilitat amb programari i maquinari, però és de llicència privativa i requereix pagament. S’utilitza sobretot per a treball d’ofimàtica, videojocs i aplicacions d’empresa.
<img width="31,8" height="15,9" alt="image" src="https://github.com/user-attachments/assets/6a0bb343-ca24-4d70-8222-390693d731e9" />


Així com macOS, que està desenvolupat per Apple, també és privatiu, i a més, només pot funcionar amb maquinari de la marca. Les seves principals característiques son un disseny molt cuidat i una gran optimització amb el seu ecosistema, cosa la cual el converteix en una opció molt popular en entorns creatius com el disseny gràfic, l’edició i producció de vídeo o àudio.

En canvi, Linux és un sistema de codi obert amb moltes distribucions diferents, com Ubuntu, Debian, Fedora, etc. Destaca per la seva seguretat, estabilitat i flexibilitat, i normalment és de llicència gratiuta. Tot i que té menos presència en ordinadors personals, és el que més s'utilitza en servidors, superordinadors, núvol i desenvolupament de programari.

## Llicenciament
## Gestors d'arrencada per a instal·lacións DUALS
## Punts de restauració
## Configuració de la xarxa
## Comandes generals i instal·lacions
