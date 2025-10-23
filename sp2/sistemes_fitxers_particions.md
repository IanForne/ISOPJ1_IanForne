---
layout: default
title: "Sistemes, fitxers i particions"
---

## 1. Mida secotr

El sector és la unitat mínima física del disc on es guarden les dades i per defecte són 512 bytes.
Un bloc o clúster és la unitat mínima lògica on es guarden les dades en el sistema operatiu, per defecte són 4096 bytes. Tot i que es pot cambiar aquesta mida quan es fromata el disc. I a més, el tamany pot ser diferent a cada partició del mateix disc.

## 2. Mida block



## 3. Fragmentació interna

La fragmentació interna es dona quan es desaprofita espai del disc pequè els blocs són més grans del que guarden dins.

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

### 6.1 GPARTED

### 6.2 Comandes
