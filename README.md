# Projecte 2: Seguretat Lògica - Recuperant accés a sistemes

## Descripció del projecte
Aquest projecte consisteix en recuperar l'accés a un sistema Linux (Zorin OS) quan s'ha oblidat la contrasenya de l'usuari principal. Per fer-ho, es treballa sobre un disc virtual clonat per evitar danys al sistema original.

A més, es protegeix l'accés al gestor d'arrencada GRUB per evitar que qualsevol persona pugui reiniciar la contrasenya mitjançant la modificació de la configuració d'arrencada.

## Tasques realitzades
- Creació d'una màquina virtual amb el disc virtual proporcionat.
- Accés a la màquina virtual i identificació dels usuaris existents.
- Recuperació i modificació de la contrasenya de l'usuari.
- Investigació i implementació de mesures de seguretat per protegir l'accés al GRUB amb contrasenya.
- Documentació detallada del procés, incloent-hi captures de pantalla.

## Objectius específics
- Recuperar l'accés a sistemes amb contrasenya oblidada.
- Fortificar l'accés al GRUB per protegir la configuració d'arrencada.

## Materials de suport
- Disc virtual amb la imatge clonada.
- Apunts RA1AA4 Seguretat Lògica.
- Guia de recuperació de contrasenya en Linux: [Recuperando password en Ubuntu](https://waytoit.wordpress.com/2013/06/06/recuperando-password-en-ubuntu/).

## Instruccions d'ús
1. Crear una màquina virtual i muntar el disc virtual proporcionat.
2. Arrencar la màquina i accedir al sistema via GRUB.
3. Seguir el procediment de recuperació de contrasenya per l'usuari identificat.
4. Configurar protecció per contrasenya al GRUB per evitar modificacions no autoritzades.
5. Verificar que el nou accés funciona correctament i que el GRUB està protegit.

## Fonts i referències
- Documentació oficial de Zorin OS i GRUB.
- Recursos en línia sobre recuperació de contrasenyes en Linux.
- Procediments de seguretat en configuració d'arrencada.

## Autor
[Nezar Mghari Boussaada]

## Data
[06/10/2025]
