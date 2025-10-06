# T02: Selecció d’un SAI per una empresa client  
**CFGM SISTEMES MICROINFORMÀTICS I XARXES 2B**  
**Nezar Mghari Boussaada**

---

## Índex
1. Inventari d’equips  
2. Càlcul de potència total  
3. Determinació de l’autonomia  
4. Recerca de models de SAI  

---

## Descripció del cas
L’empresa TecnoGestió S.L., dedicada a la gestió documental i assessorament informàtic, té un petit despatx amb 4 ordinadors de sobretaula, una impressora-fotocopiadora multifunció (similar a les que té l’escola) i un router d’accés a Internet. Davant les constants incidències amb el subministrament elèctric a la zona, la direcció ha decidit adquirir un SAI per garantir la continuïtat del servei i protegir els equips.

![Fotico](img/tiosai.png)

S’han posat en contacte amb l’empresa on esteu fent l’estada i el vostre responsable us ha encarregat que en feu l’estudi i tria del SAI.

---

## Tasques a realitzar

### 1. Inventari d’equips
Llista dels dispositius que es connectaran al SAI (ordinadors, monitors, router, etc.), justifiqueu si hi ha algun aparell que no hi connectareu al sistema d’alimentació ininterrompuda.

- **4x Ordinadors**  
  Els ordinadors serien el més essencial per posar en un SAI per guardar qualsevol document o cosa que s’estigui fent i no es converteixin en arxius corruptes.
- **4x Monitors**  
  Juntament amb els monitors són el més essencial per poder tenir visió a l’ordinador i guardar la informació sensible.
- **Router**  
  Com és una empresa d'assessorament informàtic, es té que tenir el router en un SAI per guardar coses si tenen el cloud o per avisar els clients del incident.
- **Impressora**  
  No fa falta implementar-la al SAI perquè no és un mecanisme important per al treball en qüestió.

Consulta de les especificacions tècniques per obtenir el consum de cada dispositiu. Seleccioneu components que s’ajustin als que podríeu trobar-vos a la seu del client. Indiqueu clarament les dades del component triat i els valors de watts i VA corresponents.

- [PCCom Work Intel Core i5-12400 16GB 500GB SSD](https://www.pccomponentes.com/pccom-work-intel-core-i5-12400-16gb-500gb-ssd)  
- [Monitor Nilox NXM22FHD1201 21.5" VA Full HD 120Hz HDMI VGA](https://www.pccomponentes.com/monitor-nilox-nxm22fhd1201-215-va-full-hd-120hz-hdmi-vga-negro)  

### Components seleccionats:
- 4x Ordinador i5-12400 16GB 500GB SSD  
- 4x Monitor Nilox NXM22FHD  
- 1x Router convencional  

---

### 2. Càlcul de potència total
Valor total de potència i valor incloent la reserva del 20%.

| Equip                      | Consum (VA) per unitat | Quantitat | Total VA |
|---------------------------|-----------------------|-----------|----------|
| Ordinador i5-12400 16GB   | 650                   | 4         | 2600     |
| Monitor Nilox NXM22FHD    | 50                    | 4         | 200      |
| Router convencional       | 39                    | 1         | 39       |
| **Total**                 |                       |           | **2839** |

Total + 20% de reserva:  
2839 VA × 1.20 = **3407 VA**

Convertim a watts (W):  
W = VA × Factor de Potència (0.9) = 3407 × 0.9 = **3066,3 W**

---

### 3. Determinació de l’autonomia
Estimació del temps mínim que el SAI ha de mantenir els equips en funcionament (ex. 10 minuts per guardar treballs i apagar correctament).

Per fer aquesta estimació tenim que assegurar la capacitat de bateria seguint la següent fórmula:

\[
\text{Capacitat de bateries (Ah)} = \frac{T \times \text{Potència (VA)}}{\text{Eficiencia} \times 60}
\]

On:  
- T = 10 minuts  
- Potència = 3407 VA  
- Eficiència = 0.9

Càlcul:  
\[
\frac{10 \times 3407}{0.9 \times 60} = \frac{34070}{54} = 630,9 \text{ Ah}
\]

---

### 4. Recerca de models de SAI
Cerca de 2 o 3 models de SAI que compleixin els requisits. Comparació de característiques: potència, autonomia, tipus de sortides, preu, marca.

| Característica           | Salicru SLC-4000-TWIN PRO3                            | Salicru SLC-4000-TWIN RT3                            |
|-------------------------|------------------------------------------------------|-----------------------------------------------------|
| Marca / model           | Salicru – sèrie TWIN PRO3                            | Salicru – sèrie TWIN RT3                            |
| Potència nominal        | 4.000 VA (aprox. 4.000 W)                           | 4.000 VA (aprox. 4.000 W)                           |
| Tecnologia              | On-line de doble conversió (corregeix tensió i freq.) | On-line de doble conversió                           |
| Factor de potència      | Proper a 1 (molt eficient en potència real)          | FP = 1 (tota la potència nominal és activa)          |
| Format físic            | Torre (pensat per instal·lació vertical)             | Convertible torre / rack                              |
| Tipus de sortides       | Sortides AC convencionals; no s’especifica el nombre | Almenys dues sortides AC; compatible racks           |
| Autonomia               | Habitualment entre 5 i 10 minuts a càrrega completa   | Similar (5–10 min), amb bateries externes opcionals  |
| Ampliació d’autonomia   | No indicada                                           | Sí, admet mòduls de bateries addicionals             |
| Pantalla / control      | Pantalla LCD bàsica d’estat                           | Pantalla LCD orientable i teclat complet             |
| Aplicacions típiques    | Servidors petits, estacions de treball crítiques     | Servidors en rack, centres de dades mitjans           |
| Preu aproximat          | Entre 1.500 € i 1.700 €                              | Al voltant dels 1.800 €                               |
| Disseny i punts destacats| Model senzill i fiable, versió “tower” pura          | Més versàtil i modular, dissenyat per entorns IT     |

---

**Fi del document.**

- [Tornar: README.md](README.md)
