Instal·lar i desinstal·lar en dpkg, apt, aptitude --> Com s'instala, obrir lo progreama, desinstal·lar i obrir i veure com falla pq esta desinstal·lat. Provar vlc, pacman, gimp, phpstorm, geany, dia, smplayer...

## 1. Pacman

En primer lloc, instal·larem el .deb del pacman mitjançant el moodle. Seguidament, accedirem a la carpeta on s'ha fet la instal·lació i utilitzarem la comanda dpkg, ja que és un deb.
<img width="799" height="570" alt="image" src="https://github.com/user-attachments/assets/78534e65-db8c-47ce-94f4-dfb80b23c707" />

Com veurem en la següent imatge, si executem pacman a la terminal sen's obri el joc i podem jugar.
<img width="799" height="570" alt="image" src="https://github.com/user-attachments/assets/0842d8b8-d397-4adc-a620-0cd89e14fef2" />

Seguidament, podem desinstal·lar pacman amb apt remove.
<img width="799" height="570" alt="image" src="https://github.com/user-attachments/assets/c8f2a4a0-5049-46b3-b5f4-67615892f223" />

I com veiem, si intentem obrir Pacman un altre cop, no ens deixa, ja que l'hem desinstal·lat correctament.
<img width="800" height="160" alt="image" src="https://github.com/user-attachments/assets/4509372f-ddfa-4e0f-90ae-d741a67df7df" />

## 2. Dia

Ara farem el mateix però amb el programa Dia i des de els repositoris d'Ubuntu amb apt install.
<img width="800" height="572" alt="image" src="https://github.com/user-attachments/assets/6e600d7a-1f52-44b9-a535-1ffe2c52fede" />

Com veiem, si executem dia des del terminal s'obri correctament el programa.
<img width="1100" height="572" alt="image" src="https://github.com/user-attachments/assets/5a0facb1-b946-4da3-8128-cb439728d53f" />

Ara, amb apt purge el que farem es borrar el programa i totes les seves configuracions.
<img width="800" height="572" alt="image" src="https://github.com/user-attachments/assets/4ada11aa-2389-4afd-a061-7787ea8c027a" />

Com veiem, si intentem executar de nou el programa, no deixa ja que l'hem borrat correctament.
<img width="538" height="132" alt="image" src="https://github.com/user-attachments/assets/95ea142d-cc0a-495d-98b8-d26ee7841e8f" />

## 3. Vlc

Ara instal·larem vlc però utilitzant aptitude, i podem fer-ho per exemple accedint al root utlitzant sudo su i despres ja podem fer l'instal·lació amb aptitude install vlc.
<img width="804" height="577" alt="image" src="https://github.com/user-attachments/assets/0c849b21-a6ff-4875-8739-f2fd2486eda9" />

Ara hem de surtir del root amb exit, i podem executar vlc des de la terminal, i com veiem, funciona perfectament
<img width="804" height="577" alt="image" src="https://github.com/user-attachments/assets/2dad908b-fc5e-42f4-85ff-a84336abfc40" />

Seguidament, podem borrar vlc també amb aptitude, escribint aptitude purgue vlc a la terminal.
<img width="804" height="209" alt="image" src="https://github.com/user-attachments/assets/7fd0e7d4-ba7c-46ab-843a-a432b5d5faf3" />

I com veiem, si intento accedir un altre cop al programa, no hem deixa.
<img width="804" height="209" alt="image" src="https://github.com/user-attachments/assets/a68d441e-21d1-4f15-8643-4f45c5119935" />


## 4. Geany

Ara instal·larem geany amb apt, posarem a la terminal sudo apt install geany.
<img width="804" height="209" alt="image" src="https://github.com/user-attachments/assets/6a1529ec-276f-4b6e-b3b3-24da7c44eb77" />

Com veiem, si introdueixo geany a la terminal s'obri el programa.
<img width="804" height="574" alt="image" src="https://github.com/user-attachments/assets/d8c7a870-cc52-49a8-874f-7939529aa19c" />

Seguidament, borrarem el programa amb aptitude, escriurem a la terminal aptitude remove geany
<img width="804" height="443" alt="image" src="https://github.com/user-attachments/assets/990dd014-ab34-40c6-b35d-1c4c5e2f99db" />

I com veiem, cuan torno a escriure geany a la terminal surt error.
<img width="804" height="137" alt="image" src="https://github.com/user-attachments/assets/ab2d2be0-53a6-4901-94b9-4b959206a203" />


