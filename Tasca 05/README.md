# T05: Instal·lació del domini

## Breu descripció
Instal·lació i desplegament d’**Active Directory Domain Services** en una màquina virtual Windows Server, creant un **nou domini en un bosc nou** i generant un **script PowerShell** per automatitzar el procés (PoC per a TransLògic).

## Introducció
Com a continuació de la tasca anterior, cal desplegar el **directori actiu** sobre la màquina virtual amb l’objectiu de practicar pel posterior desplegament en el client.  
A més, aquest procediment ha de servir com a **prova de concepte (PoC)** per mostrar als responsables de **TransLògic** i, d’aquesta manera, ajustar les configuracions a les necessitats reals del client.

## Procediment a documentar

### 1) Instal·lar els rols necessaris al servidor
- Instal·lar els rols requerits per muntar un controlador de domini (**AD DS** i els components necessaris).

### 2) Crear un domini nou en un bosc nou
- Crear un domini nou en bosc nou amb el nom:
  - **translogicXX.test**
  - on **XX** és el vostre **nº de llista**.

### 3) Establir el nivell funcional
- Establir el **nivell funcional** a **2025**.

### 4) Promocionar el servidor com a controlador de domini (DC)
- Promocionar el servidor com a **controlador de domini**.
- **Important:** documentar la **pantalla resum** del procés (abans d’executar la promoció).

### 5) Guardar l’script PowerShell d’automatització
- Gravar en un arxiu l’**script PowerShell** que permet automatitzar el procés d’instal·lació i promoció.

### 6) Copiar l’script al repositori
Un cop finalitzat tot el procediment:
- Copiar l’script PowerShell a la carpeta del **repositori** que esteu utilitzant.

Mecanismes possibles:
- Copiar usant **USB**
- Enviar-lo mitjançant **Internet** (correu, Drive o serveis tipus filetransfer)
- Copiar-lo usant **scp** *(cal instal·lar SSH a Windows Server)*

## Materials i links de suport
- **Guia UD6.AA3 Instal·lació DC** *(Moodle SOX)*

