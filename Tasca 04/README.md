# T04: Instal·lació Windows Server 2025

## Breu descripció
Desplegament d’una màquina virtual amb **Windows Server 2025** seguint bones pràctiques, fent una **instal·lació de prova** i elaborant una **guia d’instal·lació en Markdown** que servirà de base per a la implantació real a TransLògic S.A.

## Introducció al cas
Després del nostre assessorament, **TransLògic S.A.** ens encarrega el desplegament dels seus servidors **Windows Server 2025**.

Per aquest motiu, haurem de desplegar diverses màquines virtuals i, amb l’objectiu de ser eficients i seguir bones pràctiques, realitzarem una instal·lació de prova que servirà tant per aprendre els procediments com per elaborar una **guia d’instal·lació**, que ha de proporcionar una documentació de base a la posterior implantació als sistemes del client.

## Procediment

### 1) Crear la màquina virtual (VM)
Configurar una VM amb:
- **RAM:** 8 GB  
- **CPU:** 2 processadors  
- **Discs:**
  - Disc principal: **32 GB** (instal·lació del SO)
  - Disc secundari: **10 GB**
- **Xarxa (2 interfícies):**
  - Interfície 1: **NAT (no NAT)**  
  - Interfície 2: **host-only**

### 2) Instal·lar Windows Server 2025
- Instal·lar **Windows Server 2025 en mode GUI** (Desktop Experience).
- **Idioma del sistema:** US  
- **Configuració regional i teclat:** espanyol

### 3) Canviar el nom de l’equip
- Canviar el nom a: **DCxx**  
  - on **xx** és el vostre **número de llista**.

### 4) Actualitzar la VM
- Actualitzar completament la màquina virtual.
- Un cop actualitzada, **pausar les actualitzacions** el màxim temps possible.

## Contingut de la guia (a incloure al README / documentació)

### A) Comparativa amb requisits de Microsoft
Comparar la configuració de la VM amb els requisits mínims publicats per Microsoft per a Windows Server (apliquen també a Windows Server 2025, incloent Desktop Experience). :contentReference[oaicite:0]{index=0}

**Requisits mínims rellevants (resum):**
- **Disc:** mínim **32 GB**. :contentReference[oaicite:1]{index=1}  
- **RAM:** per a *Server with Desktop Experience* mínim **2 GB** (Microsoft recomana **4 GB**). :contentReference[oaicite:2]{index=2}  
- **CPU:** suport per **SLAT (EPT/NPT)**, instruccions **SSE4.2** i **POPCNT**. :contentReference[oaicite:3]{index=3}  

**Són coherents?**
- **Sí.** La VM proposta (**8 GB RAM**, **2 CPU**, **disc principal 32 GB + secundari 10 GB**) compleix i supera els mínims típics; per a un entorn de pràctiques/PoC és una configuració raonable. :contentReference[oaicite:4]{index=4}

### B) Procediment documentat amb captures
Documentar els passos de la instal·lació amb:
- **Captures de pantalla** (creació de la VM, selecció d’edició GUI, configuració idioma/teclat, primer inici, canvi de nom, Windows Update, etc.)
- **Observacions** (incidències, decisions de configuració, punts a repetir en producció)

> Recordatori: el format a utilitzar és **Markdown**.

## Materials i links de suport
- **UD.6. AA2. Instal·lació Window Server 2025** *(Moodle 0224 Sist. Operatius en Xarxa)*
- **Requisitos de hardware para Windows Server** *(Microsoft Learn)* :contentReference[oaicite:5]{index=5}

---

- [**Solucio**](Solucio.md)
- [**Tornar el projecte**](../README.md)

