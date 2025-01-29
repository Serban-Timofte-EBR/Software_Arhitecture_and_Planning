# Limbajul BPMN (1)

- Standard creat de OMG, similar UML

- Modelele BPMN pot fi create in scopul identificarii, validarii, imbunatatirii sau automatizarii proceselor

- Permit optimizarea proceselor din lumea reala, prin simulare

## Elemente de baza

![Elementele de baza ale limbajului BPMN](img/topic9_1.png)

## Actiuni

- Sunt obiecte de flux

![Actiuni](img/topic9_2.png)

## Evenimente

![Evenimente](img/topic9_3.png)

## Exemplu

![Exemplu evenimente BPMN](img/topic9_4.png)

## Porti exclusive

![Porti exlusive](img/topic9_5.png)

## Porti inclusive si paralele

![Porti inclusive si paralele](img/topic9_6.png)

## Porti complexe

![Porti complexe](img/topic9_7.png)

## Porti pe baza de evenimente

![Porti pe baza de evenimente](img/topic9_8.png)

## Diagrama de colaborare

- Sunt reprezentate comunicatiile dintre doua componente prin mesaje

![Containere](img/topic9_9.png)

## Aprofundam

1. Tipuri de divergenta

![Divergenta1](img/topic9_10.png)

- Poarta din diagramă este reprezentată printr-un romb cu condiții atașate fiecărui flux.

- Condițiile („Homepage selectată”, „Ziar selectat”, „Portal job-ri selectat”) indică faptul că doar unul dintre fluxuri va fi ales în funcție de condiția evaluată ca adevărată.

- In acest caz avem **divergenta exclusiva**

![Divergenta2](img/topic9_11.png)

- Toate activitățile („Publică postare intern” și „Publică postare extern”) vor fi executate simultan.

- In acest caz avem **divergenta paralela**
