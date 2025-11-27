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

<img width="809" height="202" alt="image" src="https://github.com/user-attachments/assets/18635000-9588-4b91-af22-c306f20761c6" />

<img width="809" height="144" alt="image" src="https://github.com/user-attachments/assets/d965aedc-ce03-4bf3-91fc-030a73424f0e" />

<img width="809" height="536" alt="image" src="https://github.com/user-attachments/assets/c4c807a0-a68e-463c-9cc0-b0754d6bae26" />

<img width="817" height="303" alt="image" src="https://github.com/user-attachments/assets/3c10dc6c-4da8-418a-9aa7-7dcdb58f3f26" />

<img width="681" height="234" alt="image" src="https://github.com/user-attachments/assets/bd5e3364-bf8e-47e0-a68c-4eb8b0a232d4" />

<img width="695" height="282" alt="image" src="https://github.com/user-attachments/assets/7fcf5369-62ac-4520-a139-2b5375cac28d" />

<img width="695" height="146" alt="image" src="https://github.com/user-attachments/assets/c79f0b17-4029-42d5-85c3-a3d6c019e155" />


**EXERCICI 1:** Quines comandes he d'utilitzar quan vull canviar un nom d'usuari correctament, és a dir, que estigui relacionat amb la seva home, el nom de la seva carpeta, etc.
**EXERCICI 2** Tot el que puguem fer en una única comanda per a crear un nou usuari, com haviem fet en comandes separades amb useradd, però junt.



## 3. Directoris i fitxers importants

<img width="622" height="254" alt="image" src="https://github.com/user-attachments/assets/3177f4ef-149d-4338-b0ee-9ea1b43135bf" />


## 4. Gestió avançada

<img width="372" height="173" alt="Captura de pantalla de 2025-11-25 13-13-00" src="https://github.com/user-attachments/assets/2b18827c-2dab-48f7-a758-e3f9d246f72f" />

<img width="708" height="351" alt="Captura de pantalla de 2025-11-25 13-15-20" src="https://github.com/user-attachments/assets/527b33f9-6801-4934-97e8-cf76700495d8" />

<img width="547" height="245" alt="Captura de pantalla de 2025-11-25 13-17-40" src="https://github.com/user-attachments/assets/7bb19804-1f5b-466c-b363-08b8fecf4e04" />

<img width="547" height="245" alt="Captura de pantalla de 2025-11-25 13-19-04" src="https://github.com/user-attachments/assets/712a544c-061d-45ed-ac78-bdaf4ca16ffd" />

<img width="547" height="245" alt="Captura de pantalla de 2025-11-25 13-19-34" src="https://github.com/user-attachments/assets/9dacaf0d-4175-4d5e-8968-b8c69472d533" />


<img width="392" height="168" alt="image" src="https://github.com/user-attachments/assets/03da7385-5f68-4162-907d-1e5a2dd8ef80" />

<img width="561" height="228" alt="image" src="https://github.com/user-attachments/assets/c9a14f33-7408-46ed-b859-f29acab957b4" />

<img width="480" height="187" alt="image" src="https://github.com/user-attachments/assets/81aa59d1-f5aa-4c86-b5c2-ecbd12d3c547" />

## 5. PAM

