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

<img width="318" height="159" alt="image" src="https://github.com/user-attachments/assets/6a0bb343-ca24-4d70-8222-390693d731e9" />

Així com macOS, que està desenvolupat per Apple, també és privatiu, i a més, només pot funcionar amb maquinari de la marca. Les seves principals característiques son un disseny molt cuidat i una gran optimització amb el seu ecosistema, cosa la cual el converteix en una opció molt popular en entorns creatius com el disseny gràfic, l’edició i producció de vídeo o àudio.

<img width="320" height="180" alt="image" src="https://github.com/user-attachments/assets/7527b08e-14bb-4791-b236-83d4df50904c" />

En canvi, Linux és un sistema de codi obert amb moltes distribucions diferents, com Ubuntu, Debian, Fedora, etc. Destaca per la seva seguretat, estabilitat i flexibilitat, i normalment és de llicència gratiuta. Tot i que té menos presència en ordinadors personals, és el que més s'utilitza en servidors, superordinadors, núvol i desenvolupament de programari.

<img width="330" height="165" alt="image" src="https://github.com/user-attachments/assets/1e2320ff-3800-4ec6-a64a-06f794d50a27" />

-----------------------------------------
## 3. Tècniques d'actualització i rescat del sistema
### 3.1. Prevenció
En aquest apartat explorarem la prevenció d'errors o de seguretat que podem aplicar al nostre sistema operatiu per evitar el màxim d'inconvenients futurs.
#### 3.1.1 Primera arrencada del sistema

És molt important mantenir el sistema actualitzat des d'un inici, i a més, instal·lar unes eines bàsiques per al millor rendiment del nostre nou i bàsic sistema operatiu

Per començar, podem actualitzar manualment la llista de paquets amb "sudo apt update". Aquesta comanda fa saber al sistema quins paquets tenen versions noves, i si hi ha actualitzacions disponibles. Per exemple, si ha sortit una nova versió del Firefox, aquesta comanda ho farà saber al sistema, però no l'instal·larà.

<img width="480" height="300" alt="image" src="https://github.com/user-attachments/assets/805e6630-4e00-400f-9a6e-699aafe0308e" /> <img width="480" height="300" alt="image" src="https://github.com/user-attachments/assets/59532ca5-1fc9-4075-a070-79b90916dadf" />

Per a seguidament, aplicar actualitzacions de seguretat i millores en el sistema amb "sudo apt upgrade -y". Aquesta comanda el que fa és instal·lar totes les actualitzacions disponibles dels paquets del sistema. Aixó fa que sigui molt més segur, ja que aplica les ultimes millores i correccions de seguretat.

<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/6e9b26b8-8f52-43cc-9761-65da6843bb67" />

I finalment, eliminar els paquets innecessaris amb "sudo apt autoremove -y". Això, el que fa es eliminar els paquets que han quedat desactualitzats o que ja no s'utilitzen despres d'instal·lar els més actuals.

<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/8f8fa28e-9ba2-4548-8748-14dd8f8432f4" />

A part, també és recomanable instal·lar eines addicionals.

<img width="1280" height="800" alt="image" src="https://github.com/user-attachments/assets/d816844a-6dde-458b-853a-a709f72da8c8" />

### 3.1.2 Actualitzacions periòdiques de seguretat
Per començar, podem programar actualitzacions periòdiques de seguretat per al sistema, ja que fer-ho és la millor manera per mantenir la màxima seguretat en el sistema sense trencar dependències. Així doncs, el sistema de seguretat està el màxim actualitzat possible sempre, així com es manté la màxima compabilitat amb tot el programari que puguem utilitzar.

Per fer això, podem començar per fer un "sudo apt install unattended-upgrades -y" (normalment abans es fa un "sudo apt update", però l'hem fet recentment en l'apartat anterior així que no es necessàri). Aquesta comanda, el que fa es instal·lar el paquet "unattended-upgrades", que permet aplicar actualitzacions automàtiques.

<img width="1280" height="800" alt="imatge" src="https://github.com/user-attachments/assets/4cebd7f6-1107-4b42-9fdd-7b8e85b4ed66" />

A continuació, hem de fer un "sudo nano /etc/apt/apt.conf.d/50unattended-upgrades", que obrirà el fitxer de configuració "unattended-upgrades". Aqui es on li direm al sistema que nomes actualitzi els paquets de seguretat.

<img width="817" height="538" alt="imatge" src="https://github.com/user-attachments/assets/df355c16-e04b-4ddf-a433-fc95945cb381" />
Clicarem Control+T per executar la seguent linia ""${distro_id}:${distro_codename}-security";"
<img width="817" height="538" alt="imatge" src="https://github.com/user-attachments/assets/84480f15-6dc9-4ee3-a917-d6f3e560f33a" />

I finalment, podem modificar la freqüència en que es fan aquestes actualitzacions. Això ho podem fer amb "sudo nano /etc/apt/apt.conf.d/20auto-upgrades". 

Com es veu en la imatge, la primera fila de codi serveix per a actualitzar la llista de paquets disponibles, i el numero "1" es per indicar la freqüència en dies. En el meu cas, no ho modificaré per a estar el més actualitzat disponible cada dia.

D'altra banda, la segona linia s'encarrega d'actualitzar els paquets de seguretat cada "1" dia també.
<img width="817" height="538" alt="imatge" src="https://github.com/user-attachments/assets/759a0c23-e38c-414e-a7a3-2a9fc3b74d4a" />



### 3.1.3 Backups i snapshots

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b3371d2c-3a39-40d7-ba6a-e69341c61c12" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a882a72c-e044-4009-950e-826f7b3ee3d7" />











## Llicenciament
## Gestors d'arrencada per a instal·lacións DUALS
## Punts de restauració
## Configuració de la xarxa
## Comandes generals i instal·lacions
