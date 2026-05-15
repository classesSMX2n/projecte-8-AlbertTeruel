# Informe de Solució Tecnològica: TransRàpid S.L.

## 1. Diagnòstic de la situació (Punts de dolor)

Actualment, l'empresa gestiona tota la flota amb un únic fitxer d'Excel, la qual cosa provoca els següents problemes:

* Pèrdua de dades: El fitxer falla sovint i es perd informació de rutes i factures.
* No és multiusuari: Dues persones no poden treballar a la vegada en el fitxer sense que hi hagi errors.
* Errors manuals: En escriure les dades a mà, és molt fàcil cometre equivocacions en els litres de benzina o el manteniment.
* Lentitud: El fitxer s'ha fet massa gran i costa molt d'obrir i fer-lo servir.

---

## 2. Proposta de Maquinari (Hardware)

Per millorar el treball tant a l'oficina com a la carretera, es necessiten aquests equips:

* A l'oficina: Dos ordinadors de sobretaula nous per a l'administrador i el cap de logística. Es recomana fer servir una solució **Cloud** (al núvol) per no haver de comprar un servidor físic car i difícil de mantenir.
* En ruta: 6 tablets resistents (una per a cada camió i furgoneta). Aquestes tablets han de tenir una funda protectora, GPS i connexió a internet 4G/5G per poder enviar els albarans al moment.

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/6460acff-fda8-47a7-ab0d-f27f4767c192" />

---

## 3. Proposta de Programari (Software)

Hem comparat dues maneres de substituir l'Excel:

| Característica | Odoo (Programari Lliure) | SAP / SaaS Comercial |
| --- | --- | --- |
| Preu | Més econòmic al principi. | Es paga una quota cada mes. |
| Adaptació | Es pot canviar per adaptar-lo exactament al que vol l'empresa. | És més rígid i costa més de canviar. |
| Suport | El manteniment el fa la nostra empresa d'informàtica. | El suport el dóna directament el fabricant del programa. |

Decisió: Recomanem instal·lar Odoo amb els mòduls de "Flota" i "Facturació" perquè és més flexible i permetrà que l'empresa creixi sense pagar massa per cada usuari nou.

---

## 4. Seguretat i Còpies de Seguretat

Per evitar que les dades tornin a perillar, farem el següent:

* Còpies automàtiques: Cada nit el sistema guardarà una còpia de tota la informació a un lloc segur a internet.
* Usuaris personals: Cada treballador tindrà el seu nom i contrasenya per entrar-hi, així sabrem qui ha escrit cada dada.

---

## 5. Pressupost de Digitalització

Aquest és el resum del que costarà posar en marxa el pla:

| Concepte | Detalls | Preu aproximat |
| --- | --- | --- |
| Equips d'oficina | 2 ordinadors de sobretaula. | 1.400 € |
| Equips de ruta | 6 tablets resistents i suports. | 2.100 € |
| Configuració del programa | Instal·lar Odoo i passar les dades de l'Excel. | 2.000 € |
| Formació | Explicar als xofers i administratius com funciona. | 500 € |
| TOTAL |  | 6.000 € |

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/2d27696c-d62b-4e6a-8323-9b3958b6caca" />
