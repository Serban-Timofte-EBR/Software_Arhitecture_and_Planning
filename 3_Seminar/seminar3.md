## Diagrama de utilizare

**1. Actori**

&emsp;&emsp;&emsp; - Reprezentati prin userii care vor folosi aplicatia

**2. Caz de utilizare**

&emsp;&emsp;&emsp; - Modalitatile prin care actorii (userii) vor interactiona cu aplicatia

&emsp;&emsp;&emsp; - Se marcheaza printr-un verb

**3. Relatie de asociere**

&emsp;&emsp;&emsp; - Relatia dintre un actor si un caz de utilizare

&emsp;&emsp;&emsp; - Reprezentate prin sageti cu sens (de regula discuta)

**3. Relatie de generalizare sau paritcularizare**

&emsp;&emsp;&emsp; - Relatia dintre doi actori

&emsp;&emsp;&emsp; - Actorului copil ii voi fi disponibile toate caracteristicele actorului parinte

&emsp;&emsp;&emsp;&emsp; - **Ex:** Actor parinte <- Actor copil

**3. Relatie dintre doua usecaseuri**

&emsp;&emsp;&emsp; - Generalizare

&emsp;&emsp;&emsp;&emsp; - Intre doua cazuri de utilizare

&emsp;&emsp;&emsp;&emsp; - Trasaturi generale in clasa parinte si cazuri specifice in clasa copil

&emsp;&emsp;&emsp;&emsp; - Sustine examen cu Sustine examen online, Sustine examen in campus (Adica putem sustine un examen si online si in campus)

**Ex:**


&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Plaseaza comanda

Comanda telefonica &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Comanda prin interent

Client telefonic &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Client interent

**Plaseaza comanda**: Selecteaza produse, Selecteaza adresa de livrare, Introducere date personale

**Comanda telefonica, Comanda prin interent**: Modalitati de plata diferite

&emsp;&emsp;&emsp; - Includere

&emsp;&emsp;&emsp;&emsp; - A &rarr; (include) B

&emsp;&emsp;&emsp;&emsp; - Initiem A &rarr; Folosim si B. B nu poate fi utilizat de A

&emsp;&emsp;&emsp;&emsp; - **Ex:** Creeaza cont bancar, Retrage bani includ Valideaza date

<code>
Creeaza cont bancar &rarr; (include) Valideaza date

Retrage bani &rarr; (include) Valideaza date
</code>

<i>Cazul de baza nu este complet fara celelalte actiuni. Cazyl de baza este Valideaza date</i>

&emsp;&emsp;&emsp; - Extindere

&emsp;&emsp;&emsp;&emsp; - A &rarr; (extend) B

&emsp;&emsp;&emsp;&emsp; - Directia este opusa fata de include. Catre cazul de baza pointeaza sageata

&emsp;&emsp;&emsp;&emsp; - Se executa A si daca selecteaza utilizatorul sau se indeplineste un set de functionalitati se initiaza si B

&emsp;&emsp;&emsp;&emsp; - **Ex:** Solicita card de fidelitate, Verifica eligibilitatea, Efecteaza verificari suplimentare

<code>
Solicita card de fidelitate, &rarr; (include) Verifica eligibilitatea &larr; (extends) Efecteaza verificari suplimentare

</code>

<i>Daca cerem card de fidelitate facem Verificare eligibilitate. Daca clientul care cere cardul este strain atunci verificam eligibilitatea. Adica daca cerem card NU este necesar sa verificam suplimentar, ci doar daca este un client strain sau problematic</i>

**Info:**

- Login NU este caz de utilizare

- Daca conectez doi actori la un usecase inseamna ca acel usecase are nevoie de cei doi actori pentru a folosi acel feature (use case)