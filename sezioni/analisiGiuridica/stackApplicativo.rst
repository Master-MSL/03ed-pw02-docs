Stack Applicativo
==================

Si riporta di seguito lo Stack [46]_ Applicativo relativo
all’attuale infrastruttura software del sistema regionale di FSE e del
Taccuino

.. |imageIn1| figure:: /immagini/tabellaInfr1.jpg
   :scale: 80 % 
   :alt: Stack AS-IS

   Stack AS-IS

In caso di migrazione allo Stack Applicativo relativo al sistema cloud
Nivola sarebbero modificati esclusivamente gli strati del s.o. e il
sistema di virtualizzazione, come segue:

.. |imageIn2| figure:: /immagini/tabellaInfr2.jpg
   :scale: 80 % 
   :alt: Stack TO-BE

   Stack TO-BE

Dall’analisi sopra evidenziata, emerge quindi la presenza di software
sotto “copyleft debole” accanto a soluzioni a “copyleft forte”. Tuttavia
deve anche aggiungersi che gli elementi a copyleft forte riguardano le
componenti di sistema (sistema operativo), in sé non necessariamente
“viralizzanti” i sistemi applicativi verticali in essi operanti ed
eseguiti, in ragione delle relative condizioni e limiti, come meglio di
seguito esposto.

In considerazione della clausola 2 del capitolo “Terms and conditions
for copying, distribution and modification” della licenza GPLv2
associata a CentOS [47]__ un software applicativo verticale costituito da componenti web (web application, web service, etc.) che viene eseguito in un ambiente di runtime costituito da un application server (LGPL), che a sua volta viene eseguito su un sistema operativo (GPLv2), non viene viralizzato da quest’ultimo non essendo in alcun modo un’opera derivata.

.. [46] La pila (o stack), in informatica, è un tipo di dato astratto che viene usato in diversi contesti per riferirsi a strutture dati, le cui modalità di accesso ai dati in essa contenuti seguono una modalità LIFO (Last In First Out), ovvero tale per cui i dati vengono estratti (letti) in ordine rigorosamente inverso rispetto a quello in cui sono stati inseriti (scritti). fonte: https://it.wikipedia.org/wiki/Pila_(informatica)

.. [47] “\ \ *2. You may modify your copy or copies of the Program or any portion of it, thus forming a work based on the Program, and copy and distribute such modifications or work under the terms of Section 1 above, provided that you also meet all of these conditions:*

   *a) You must cause the modified files to carry prominent notices
   stating that you changed the files and the date of any change.*

   *b) You must cause any work that you distribute or publish, that in
   whole or in part contains or is derived from the Program or any part
   thereof, to be licensed as a whole at no charge to all third parties
   under the terms of this License.*

   *c) If the modified program normally reads commands interactively
   when run, you must cause it, when started running for such
   interactive use in the most ordinary way, to print or display an
   announcement including an appropriate copyright notice and a notice
   that there is no warranty (or else, saying that you provide a
   warranty) and that users may redistribute the program under these
   conditions, and telling the user how to view a copy of this License.
   (Exception: if the Program itself is interactive but does not
   normally print such an announcement, your work based on the Program
   is not required to print an announcement.)*

   *These requirements apply to the modified work as a whole.*\ \ \ **If
   identifiable sections of that work are not derived from the Program,
   and can be reasonably considered independent and separate works in
   themselves, then this License, and its terms, do not apply to those
   sections when you distribute them as separate works. But when you
   distribute the same sections as part of a whole which is a work based
   on the Program, the distribution of the whole must be on the terms of
   this License, whose permissions for other licensees extend to the
   entire whole, and thus to each and every part regardless of who wrote
   it.**

   **Thus, it is not the intent of this section to claim rights or
   contest your rights to work written entirely by you; rather, the
   intent is to exercise the right to control the distribution of
   derivative or collective works based on the Program.**

   *In addition, mere aggregation of another work not based on the
   Program with the Program (or with a work based on the Program) on a
   volume of a storage or distribution medium does not bring the other
   work under the scope of this License.*\ \ ”


