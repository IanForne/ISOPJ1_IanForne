---
layout: default
title: "Sistemes, fitxers i particions"
---

## 1. Mida secotr
El sector és la unitat mínima física del disc on es guarden les dades i per defecte són 512 bytes.

<img width="648" height="316" alt="image" src="https://github.com/user-attachments/assets/8f50ccb1-c644-4271-9ac2-417bfd857d43" />

Com es veu en la imatge, hem creat un fitxer que conté "Bon dia". Aquest fitxer mesura 8 bytes, però el sistema està utilitzan 4096 bytes per emmagatzemar aquesta informació. Per tant, estem desaprofitant molt d'espai per emmagazemar un fitxer en un bloc massa gran.

<img width="648" height="331" alt="image" src="https://github.com/user-attachments/assets/6502412f-bd90-421d-a695-c1badf98843f" />

A més, com es veu en la imatge, la mida del sector es de 512 bytes com haviem vist anteriorment.

## 2. Mida block
Un bloc o clúster és la unitat mínima lògica on es guarden les dades en el sistema operatiu, per defecte són 4096 bytes. Tot i que es pot cambiar aquesta mida quan es fromata el disc. I a més, el tamany pot ser diferent a cada partició del mateix disc.

<img width="765" height="191" alt="image" src="https://github.com/user-attachments/assets/d159cf29-96dc-4832-ad89-90d107cdfe3b" />

Per a trobar la mida del block, li hem de passar la partició que conté el nostre SO, ja que entre particions aquesta pot variar. I com veiem, la seva mida per defecte és de 4096 bytes.

## 3. Fragmentació interna

La fragmentació interna es dona quan es desaprofita espai del disc pequè els blocs són més grans del que guarden dins.

<img width="765" height="453" alt="image" src="https://github.com/user-attachments/assets/64f50c0b-cbb9-4568-bad0-8edc7c90d9ed" />

Com veiem, aquesta comanda serveix per saber si al nostre disc li fa falta fragmentar, en aquest cas no fa falta desfragmentar el disc.

## 4. Fragmentació externa

A mesura que es treballa amb un arxiu, es van separant els components d'aquest de forma que al llarg dels temps, s'arrelenteix la velocitat del disc a l'hora de llegir aquell fitxer.

## 5. Tipus de formateig

### 5.1 Baix nivell
Borra el sistema de fitxers, els fitxers, i a més borra els sectors defectuosos. És a dir, esborra totes les dades, el deixa com si fos de fàbrica. A més, no es pot formatar a partir del sistema operatiu, és necessiten programes externs especialitzats amb la formatació.

### 5.2 Mig nivell
El que borra és el sistema de fitxers, i si troba algun secor defectuós o algun lloc on no es pot emaagatzermar dades els marca per a no guardar més informació dins, però no els borra.

### 5.3 Alt nivell
Només borra el ssitema de fitxers, no borra els fixers en sí.


## 6. Gestió de particions

Una partició és un tros de disc físic, tot i que es pot treballar amb volums, que no és un tros de disc físic, sinó que és una agrupació lògica de particions i/o discs. És a dir, és com posar una capa d'abstracció damunt de les particions.

Per exemple, pots tenir diferents discs, de diferents tamanys, diferents marques, etc, i pots juntar aquests discs individuals per a treballar conjuntament amb ells de manera única. Tot i que, el més recomanat per a evitar problemes és tenir discs amb els mateixos tamanys, velocitats i de la mateixa marca.


### 6.1 GPARTED

<img width="773" height="375" alt="image" src="https://github.com/user-attachments/assets/43ab6717-f1ad-4084-8378-350fe6280a31" />

Amb el gparted, podem fer el mateix que amb les comandes, encara que l'únic que no podem fer és modificar la mida del block.

### 6.2 Comandes

<img width="1023" height="521" alt="image" src="https://github.com/user-attachments/assets/827dca80-6b89-4fc0-9127-9eb904f2d2c9" />

<img width="1023" height="277" alt="image" src="https://github.com/user-attachments/assets/176a5083-bfcb-4912-a66e-59dfac8a65f3" />


Com es veu, hem fet una partició d'aproximadament la meitat del total del disc.

<img width="1023" height="424" alt="image" src="https://github.com/user-attachments/assets/31884918-01ac-4b44-93ff-7a0b59c6616b" />
hem formatat la mida de bloc a 2048

<img width="760" height="116" alt="image" src="https://github.com/user-attachments/assets/b5671acc-2fcb-4820-bde7-0494ac3985cc" />
Com veiem, amb aquesta comanda hem comprobat que la modificació de la mida del block s'ha efectuat correctament.

<img width="798" height="116" alt="image" src="https://github.com/user-attachments/assets/ffa840b6-e1d9-419e-96f0-426272e6a914" />
Amb aquesta comanda hem modificat el bloc de la particio b a 4096 bytes.

<img width="771" height="334" alt="image" src="https://github.com/user-attachments/assets/100f3da5-f1cf-4f09-8f21-4e99dbe40ae4" />

Com veiem, totes les particions s'han efectuat correctament.

