# T06: Configuració del domini

## Breu descripció
Configuració i desplegament d’un domini creant els objectes principals (OU, grups, usuaris i equips) i verificant el funcionament amb inici de sessió al client.

## Introducció
Un cop tenim ja el nostre domini creat, el següent pas és desplegar el domini, és a dir, crear els diferents objectes que el formaran: **grups, usuaris i màquines**.  
En aquesta tasca veurem la utilitat d’organitzar els objectes amb **unitats organitzatives (OU)**.

## Procediment pràctic

### 1) Crear l’estructura d’unitats organitzatives (OU)
Crear la següent estructura d’OU:
- *(A definir segons l’enunciat complet / esquema de la pràctica)*

> Nota: Assegura’t d’incloure com a mínim la OU **equips** (es fa servir al punt d’aprovisionament de PC1).

### 2) Definir l’estructura de grups
Crear els grups següents:
- **gestio**
- **magatzem**
- **gerencia**
- **personal**

Afegir com a membres del grup **personal** els tres grups anteriors:
- gestio ∈ personal  
- magatzem ∈ personal  
- gerencia ∈ personal  

### 3) Crear plantilles d’usuari (una per cada grup)
Crear una plantilla d’usuari per a:
- **Gestio**
- **Magatzem**
- **Gerencia**

Cada plantilla ha de tenir:
- **Pertinença al grup** corresponent
- **Creació de la carpeta personal** (home folder)

### 4) Crear usuaris de prova
Definir **un usuari de prova** per cadascuna de les plantilles:
- Usuari prova (Gestio)
- Usuari prova (Magatzem)
- Usuari prova (Gerencia)

### 5) Aprovisionar un equip (PC1) dins la OU equips
- Crear l’objecte equip **PC1**
- Ubicar-lo dins la OU **equips**

### 6) Crear una VM Windows 11 i unir-la al domini
- Crear una **VM amb Windows 11**
  - **RAM:** 4 GB
  - **Disc:** suficient
  - **Xarxa:** NAT
- Un cop instal·lat l’equip, **afegir-lo al domini**

### 7) Comprovació de funcionament
Comprovar el correcte funcionament iniciant sessió a l’equip client amb:
- usuari de prova (Gestio)
- usuari de prova (Magatzem)
- usuari de prova (Gerencia)

## Materials i links de suport
- **UD6.AA3 Desplegament** *(Moodle 0224 SOX)*
