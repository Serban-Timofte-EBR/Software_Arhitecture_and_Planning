## Analiza orientata obiect a sistemelor informatice

1. **Diagrama de clase**

&emsp;&emsp;&emsp; - Pentru fiecare sistem este o singura diagrama de clase

&emsp;&emsp;&emsp; - Poate rezulta automat structura bazei de date

2. **Diagrama de obiecte**

&emsp;&emsp;&emsp; - Ne spune daca modelul obtinut este corect sau trebuie corectat

3. **Diagramele de stare**

&emsp;&emsp;&emsp; - Prin ce stari vor trece obiectele sistemului

&emsp;&emsp;&emsp; - Multiple, pentru fiecare obiect al sistemului

&emsp;&emsp;&emsp; - Cate clase avem in diagrama de clase, atatea diagrame de stare avem

4. **Diagramele de activitate**

&emsp;&emsp;&emsp; - Cum sa desfasoare use case-urile din diagrama de cazuri

&emsp;&emsp;&emsp; - Plecam de la functionalitatile sistemului

5. **Diagramele de interactiune**

&emsp;&emsp;&emsp; 5.1. **De seventa**

&emsp;&emsp;&emsp; - Ce mesaje de transmit intre actiuni

&emsp;&emsp;&emsp; 5.1. **De comunicare**

&emsp;&emsp;&emsp; - Pune accent pe grupul de mesaje din actiuni

### OBS

1. Diagrama de clase o realizam in doi pasi. Forma initiala include clasele (indeficarea lor - a denumirilor). Ulterior, stabilim legaturile intre clasele respective

## Definirea unui atribut

- Trebuie descris prin nume, vizibilitate, tipul (derivat sau nu), tip de data, mutiplicitate, val implicita, proprietate

- Proprietatile sunt informatii suplimentare despre un atribut

## Definirea unei relatii

- Denumire (optional), multiplicitate, roluri ale asocierii, directie de navigare

- Tipuri de asociereȘ unare, binare, n-are

Ex:

<code>
Profesor ---------------------------> * Student

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;tine curs pentru &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
</code>
- Un profesor tine curs pentru mai multi studenti

**Multiplicarea**: 


Persoana (0>) ---------------------------(0,1) Masina

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;detine

- Cate masini poate detine o persoana? Min: 0, Max: inf.

- O masina de cat persoane poate fi detinuta? Min: 0 Max: 1 

Persoana (0,1)---------------------------(0,1) Masina

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;conduce

- O persoana cate masini poate conduce? Min: 0, Max: 1

- O masina poate fi condusa de Min: 0, Max: 1 persoana

O pesoana asociata unei persoane in 2 roluri distince: Parinte - Copil

- O persoana este parinte pentru min. 1 parinte, max. oricati (O persoana parintele unuia sau mai multor parinti)

- Consideram parinte biologic: O persoana este copilul a 2 parinti

## Clasa asociere


&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Program de studiu

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; |

Inscriere -------------- |

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; |

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Student

- Inscriere este clasa asociere
- Daca asocieze notUnique marcam faptul ca un student poate avea multiple inscriere la programe de studiu

## Agregarea

- Relatia Parte / Intreg

- **Partajata**

&emsp;&emsp;&emsp; - Disparitia intregului nu duce la disparitia partilor componente

- **Compusa**

&emsp;&emsp;&emsp; - Disparitia intregului duce la disparitia partilor componente

EX: 

Calculator format din placa de baza, ram, etc (**Agregare compusa**)

- Dezmembrez unitatea de calculator, dar componentele exista

Cladirea formata din sali (**Agregare compusa**)

- Daca dispare cladirea, salile dispar

- Sala NU o pot lua si sa o pun in alta cladire