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

<img width="596" height="418" alt="Captura de pantalla de 2025-10-07 10-09-20" src="https://github.com/user-attachments/assets/bc73db09-5a36-4241-8ad8-e342c03a36b7" />

En segon lloc, el /home, que es la carpeta personal de cada usuari (archius, documents, descargues, configuracions). 
<img width="596" height="418" alt="Captura de pantalla de 2025-10-07 10-07-05" src="https://github.com/user-attachments/assets/4516d637-b459-4db5-9516-f765846dacd0" />

En tercer lloc, el SWAP. És un espai virtual reservat per a quan s'ompli la memòria ram del sistema. Evita que el sistema es bloqueji si s'avaba la RAM.
<img width="596" height="418" alt="Captura de pantalla de 2025-10-07 10-15-39" src="https://github.com/user-attachments/assets/1207dc1a-8caa-47a1-9e00-f4d0479537b2" />

I finalment, he creat una partició a / per a al root. He fet servir el que quedava d'espai, deixant just 40 GB lliures. Aqui es on viu el sistema operatiu, s'utulitza per emmagatzemar els programes, les llibreries, etc.
<img width="596" height="418" alt="Captura de pantalla de 2025-10-07 10-16-34" src="https://github.com/user-attachments/assets/aec2c343-1a27-4e31-89d6-0e6cefa20395" />

I aquest ha sigut el resultat final de les particions.
<img width="963" height="682" alt="Captura de pantalla de 2025-10-07 10-17-21" src="https://github.com/user-attachments/assets/78883f98-bfb1-43ce-b965-46765c59ca63" />

A banda, he fet un clon de la màquina per a futurs projectes i per a que actui com a copia de seguretat si més endacavant deixa de funcionar la que estic utilitzant.
<img width="773" height="411" alt="Captura de pantalla de 2025-10-07 10-31-08" src="https://github.com/user-attachments/assets/b123e97b-6101-4cf0-bf49-0254832e35d5" />



----------------------
## 3. Activació del mode EFI

Per activar el mode EFI, primer que res hem d'aturar la màquina virtual. Després, hem d'accedir als paràmetres i anar a l'apartat de sistema, un cop verifiquem que estem en la pestanya de la placa base, hem de buscar i activar el mode EFI que ve per defecte desactivat.

<img width="865" height="562" alt="Captura de pantalla de 2025-10-07 10-36-54" src="https://github.com/user-attachments/assets/29dc17e7-e97b-45cc-963d-d0f5e6850ea2" />

## 4. Configuració del Windows

Un cop hem activat el mode EFI, quan iniciem la màquina ens diu que no ha pogut trobar un sistema operatiu (no he pogut fer captura) i que n'instal·lèssim un. En aquest punt, he seleccionat l'ISO de Windows 10. 
<img width="620" height="595" alt="Captura de pantalla de 2025-10-07 10-45-45" src="https://github.com/user-attachments/assets/a88039f3-9a2e-477f-aaac-4797439680e9" />

He anat avançant fins la pestanya de les particions. Un cop allí, he seleccionat la part del disc que estava lliure i he creat una nova partició amb el tamany per defecte que hem donava, que és casi tot el tamany del disc, ja que així es crea una particó que necessita el sistema per a funcionar.
<img width="620" height="199" alt="Captura de pantalla de 2025-10-07 10-50-36" src="https://github.com/user-attachments/assets/dbc47b47-2410-4b09-9525-a9b4c6ae1084" />

I com veiem, s'ha creat una petita partició addicional de 16 MB
<img width="620" height="230" alt="Captura de pantalla de 2025-10-07 10-51-49" src="https://github.com/user-attachments/assets/46e3d88f-54de-4e41-aa68-fb9cf837a765" />

Després he seguit abançant amb la instal·lació convencional de Windows 10.

<img width="1036" height="803" alt="Captura de pantalla de 2025-10-07 11-54-05" src="https://github.com/user-attachments/assets/70234776-05ac-4438-a69f-6bc735c38193" />





## Llicenciament
## Gestors d'arrencada per a instal·lacións DUALS
## Punts de restauració
## Configuració de la xarxa
## Comandes generals i instal·lacions
