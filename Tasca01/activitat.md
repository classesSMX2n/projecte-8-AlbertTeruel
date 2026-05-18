# Informe de Solució Tecnològica: TransRàpid S.L.

## 1. Diagnòstic de la situació (Punts de dolor)

Actualment, l'empresa gestiona toda la flota amb un únic fitxer d'Excel, la qual cosa provoca els següents problemes:

* Pèrdua de dades: El fitxer falla sovint i es perd informació de rutes i factures.
* No és multiusuari: Dues persones no poden treballar a la vegada en el fitxer sense que hi hagi errors.
* Errors manuals: En escriure les dades a mà, és molt fàcil cometre equivocacions en els litres de benzina o el manteniment.
* Lentitud: El fitxer s'ha fet massa gran i costa molt d'obrir i fer-lo servir.

---

## 2. Proposta de Maquinari (Hardware)

Per millorar el treball tant a l'oficina com a la carretera, es necessiten aquests equips concrets amb preus reals de mercat (IVA inclòs):

* A l'oficina (2 equips complets):
* Ordinador de sobretaula: Lenovo ThinkCentre M70q Gen 5 Tiny (Processador Intel, format compacte per a empreses). Preu: 889,01 € per unitat.
* Monitor: DELL SE2422H de 23,8" Full-HD (75 Hz). Preu: 202,00 € per unitat.
* Nota d'infraestructura: Es descarta la compra d'un servidor físic local per evitar costos de manteniment i reparació. Es farà servir una solució Cloud (al núvol) per allotjar el programa de gestió.


* En ruta (6 vehicles):
* Tablet robusta: Samsung Galaxy Tab Active5 5G de 8" (6GB RAM / 128GB emmagatzematge, color verd, resistent a l'aigua, pols i impactes). Preu: 393,00 € per unitat.
* Suport professional: Suport carregador de la marca RAM Mounts (Referència exacta RAM-HOL-SAM60CPU, model form-fit de la sèrie EZ-Roll'r amb pins de càrrega pogo integrats i connexió USB-C, totalment compatible amb la tablet Tab Active5). Preu: 84,15 € per unitat.



---

## 3. Proposta de Programari (Software)

Hem comparat dues maneres de substituir l'Excel:

| Característica | Odoo (Programari Lliure) | SAP / SaaS Comercial |
| --- | --- | --- |
| Preu | Més econòmic al principi. | Es paga una quota cada mes. |
| Adaptació | Es pot canviar per adaptar-lo exactament al que vol l'empresa. | És més rígid i costa més de canviar. |
| Suport | El manteniment el fa la nostra empresa d'informàtica. | El suport el dóna directament el fabricant del programa. |

Decisió: Recomanem instal·lar Odoo amb els mòduls de Flota i Facturació perquè és més flexible i permetrà que l'empresa creixi sense pagar massa per cada usuari nou.

---

## 4. Seguretat i Còpies de Seguretat

Per garantir la disponibilitat immediata de la informació i protegir les dades de facturació i rutes, s'estableix la següent política tècnica:

* Estratègia de còpies de seguretat 3-2-1:
1. 3 còpies de dades: Es mantindrà la base de dades en viu (Odoo Cloud), una còpia de seguretat diària automatitzada al mateix proveïdor del núvol, i una segona còpia deslocalitzada en un servidor d'emmagatzematge independent (com AWS S3 o Google Cloud Storage).
2. 2 suports diferents: Les dades estaran en servidors de producció i en discs d'emmagatzematge d'arxiu en xarxa diferents.
3. 1 còpia fora de l'oficina: Totes les còpies de seguretat estaran fora de les instal·lacions físiques de TransRàpid S.L. per evitar pèrdues en cas d'incendi o robatori. Es mantindrà un històric de retenció de 30 dies.


* Control d'accés per rols (RBAC): Cada treballador tindrà un usuari uniquíssim i contrasenya. Els xofers tindran un perfil restringit a la tablet on només podran visualitzar la seva pròpia ruta i registrar els seus albarans. No tindran accés a les dades de facturació global ni a la informació dels altres vehicles, protegint la confidencialitat de l'empresa.

---

## 5. Pressupost de Digitalització

Resum tancat de la inversió requerida per a la implementació del projecte amb l'actualització de preus reals (tots els preus de maquinari inclouen l'IVA):

| Concepte | Detalls del model i quantitat | Preu Total |
| --- | --- | --- |
| Ordinadors d'oficina | 2 unitats de Lenovo ThinkCentre M70q Gen 5 Tiny. | 1.778,02 € |
| Monitors d'oficina | 2 unitats de DELL SE2422H de 23,8". | 404,00 € |
| Tablets de ruta | 6 unitats de Samsung Galaxy Tab Active5 5G. | 2.358,00 € |
| Suports de vehicle | 6 unitats de suports carregadors RAM Mounts RAM-HOL-SAM60CPU. | 504,90 € |
| Configuració del sistema | Instal·lació d'Odoo al núvol, alta d'usuaris i migració de les dades de l'Excel. | 2.000,00 € |
| Formació de personal | 8 hores de formació pràctica per a xofers i personal administratiu. | 500,00 € |
| TOTAL INVERSIÓ |  | 7.544,92 € |

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/23c2d23c-1585-4db6-958c-01b81d266f43" />

