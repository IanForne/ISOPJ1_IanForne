---
layout: default
title: "Gestió d'usuaris grups i permisos"
---

## 1. Fitxers importants

<img width="1206" height="719" alt="image" src="https://github.com/user-attachments/assets/a013fca0-9fd1-4e8e-a287-a935474fb85a" />

Conté tots los usuaris del sistema, normalment dalt de tot l'usuari root i baix de tot los usuaris que anirem creant al sistema. Per a identificar els usuaris que poden accedir gràficament al sistema podem vure el tipus de shell, que sol ser /bin/bash o /bin/sa, segons l'intèrpret podrem utilitzar unes comandes o unes altres.

<img width="584" height="58" alt="image" src="https://github.com/user-attachments/assets/21ac0c33-df8b-4e77-87d6-b620dd991dff" />

Nom Usuari:contrassenya pero a un altre fitxer:identificador del usuari: identificador del grup principal: informació variada: home del usuari per a podere accedir gràficament.

<img width="1206" height="719" alt="image" src="https://github.com/user-attachments/assets/cf0c8a24-0abe-4f24-b675-b59bf3c2df58" />

Comtrasseyes encriptades. Es pot elegir el mètode d'encriptació. També conté informació de quan es van cambiar, la seva caduvitat, etc.

<img width="1206" height="719" alt="image" src="https://github.com/user-attachments/assets/d3985080-c93e-4bf8-9ef6-ecb8d0bea73e" />

En aquest fitexer podem veire tots los usuaris del sistema i a quins grups pertanyen. Sempre que creem un usuari es crea un grup, al final podem veure l'identificadro del grup

<img width="1206" height="719" alt="image" src="https://github.com/user-attachments/assets/8db89da3-48f4-4fc0-9fde-2fd77f52c7ac" />

Podem veure els usuaris que son part d'un grup i l'administrador de cada grup, que només pot hi haver un.

<img width="724" height="437" alt="image" src="https://github.com/user-attachments/assets/2d51ade2-a3e2-4f56-b7af-182b4c9c13e8" />

Amb l'eina system-tools també es poden crear usuaris i administrar grups, tot i que nosaltres ho farem tot en comandes, pot ser una eina útil per a persones que no es volen complicar molt la vida.


## 2. Comandes bàsiques

<img width="724" height="468" alt="image" src="https://github.com/user-attachments/assets/4609809e-07ee-4348-bfae-8a55743dbc14" />
**adduser** per a crear un nou usuari.

<img width="892" height="248" alt="image" src="https://github.com/user-attachments/assets/81bd2247-facf-401f-b7f8-cde83ad5b5d2" />

Podem comprovar que ens l'ha creat fent les seguents comprovacions i veient que ens ha creat les carpetes corresponens, menys les que es creen quan iniciem gràficament l'usuari per primera vegada.

**deluser** per a borrar l'usuari

<img width="644" height="92" alt="image" src="https://github.com/user-attachments/assets/c2147786-5882-46da-86d0-659087e3260a" />


<img width="623" height="132" alt="image" src="https://github.com/user-attachments/assets/2f9fa265-0d7e-48e4-9424-060fe4412a3f" />

<img width="623" height="132" alt="image" src="https://github.com/user-attachments/assets/34778678-d2d8-48ea-b1b8-0b140e8c76ae" />

<img width="623" height="104" alt="image" src="https://github.com/user-attachments/assets/8e4a3157-b93a-4431-b948-84784fdd6fa2" />

<img width="623" height="123" alt="image" src="https://github.com/user-attachments/assets/386c7a81-ce84-44d4-b304-8676c11b8f9c" />

<img width="623" height="161" alt="image" src="https://github.com/user-attachments/assets/c25a03cb-697d-4700-a925-4ed470180022" />

<img width="623" height="248" alt="image" src="https://github.com/user-attachments/assets/044c0e44-4214-47c9-a281-cca20801f7db" />

Per a crear un usuari amb useradd hem de crear el nom d'usuari, crar el directori home li hem donat permisos a la seva carpeta, li hem creat una contrassenya i opcionalment es pot canviar el seu interpret

## 3. Directoris i fitxers importants


## 4. Gestió avançada


## 5. PAM
