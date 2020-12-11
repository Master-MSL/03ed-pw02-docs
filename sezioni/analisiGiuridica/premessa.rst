Premessa: elementi giuridici sul software e su FOSS (Free and Open Source Software)
=========================================================================================

Il software è un bene immateriale che costituisce un valore che deve
essere protetto. Gli strumenti a tutela del software sono:

-  il **diritto d'autore**: strumento che protegge il software per come
   è scritto in qualità di opera creativa. Vengono tutelati dal diritto
   d'autore il codice sorgente e binario; si possono includere i lavori
   preparatori ma non gli algoritmi (l’algoritmo è l’idea utilizzata per
   descrivere la logica utile all’automazione di un processo e non la
   forma in cui viene realizzato)` [37]_`.

-  l’istituto del **brevetto**: strumento che tutela il programma come
   metodo e quindi da un punto di vista della sequenza delle fasi che
   vengono eseguite, espresse sia in forma logica sia in forma di
   algoritmo.

Il brevetto si applica ad una soluzione (ad un problema tecnico) che ha
carattere di *novità, originalità, liceità e
industrialità.*` [38]_`

A questi strumenti di tutela si possono affiancare:

-  **marchio**, ovvero “tutti i segni che siano atti a distinguere i
   prodotti o i servizi di una impresa da quelli di altre imprese e che
   possano essere rappresentati nel registro in modo da consentire la
   determinazione chiara e precisa dell’oggetto della protezione
   conferita al titolare” (art. 7 del Codice della Proprietà
   Industriale, di seguito “CPI”). Inoltre, la normativa richiede che i
   marchi, per poter essere registrati, siano dotati dei requisiti di
   novità (art. 12), capacità distintiva (art. 13), e liceità (art. 14);

-  **modelli e disegni industriali** (art. 31 e segg. e segg. CPI);

-  **segreto commerciale**, inteso come “valore esclusivo” e/o
   *know-how* (art. 39 TRIPS` [39]_`, Direttiva UE UE 2016/943,
   art. 98 CPI) e concorrenza sleale (art. 99 CPI, artt. 2595-2601
   c.c.); in aggiunta sono strettamente correlati i concetti di:

-  

   -  obbligo di fedeltà (art. 2105 c.c.);

   -  patto di non concorrenza (art. 2125 c.c.);

   -  rivelazione di segreto professionale (art. 622 c.p.)e rivelazione
      di segreto scientifico e commerciale (art. 623 c.p.).

Copyleft, licenze e loro compatibilità
----------------------------------------

La licenza d’uso è un negozio giuridico (contratto) tramite cui vengono
concesse alcune facoltà/diritti a determinate condizioni. Esistono:

-  Licenze proprietarie, che concedono al licenziatario generalmente il
   solo diritto d’uso non esclusivo di un programma con accesso al SOLO
   codice binario. Il proprietario si riserva il diritto di modifica e
   distribuzione;

-  Licenze libere, che si basano anch’esse sul diritto d’autore
   declinandolo però in termini di libertà (anziché di restrizioni a
   favore della condivisione del codice sorgente). L’autore, licenziando
   il proprio software con licenze libere, concede a terzi i diritti di
   esecuzione, studio, ridistribuzione e modifica sotto determinate
   condizioni. In base a come vengono declinate le condizioni di
   modifica e ridistribuzione esistono diverse categorie di licenze
   libere` [40]_`:

   -  permissive (o no copyleft)

   -  copyleft debole

   -  copyleft forte

   -  network copyleft

di seguito schematizzate efficacemente in forma grafica.

.. |image56| figure:: /immagini/100002010000054D000002AD49A6931C5F7BB1A7.png
   :scale: 80 % 
   :alt: Schema di categorie software di Chao-Kuei

   Schema di categorie software di Chao-Kuei

Si sono formate nel corso del tempo due correnti pensiero che hanno
portato alla costituzione di organizzazioni specifiche le cui
caratteristiche sono sintetizzate nella tabella sottostante.

+-----------------------------------+-----------------------------------+
| **Free Software**                 | **Open source**                   |
+-----------------------------------+-----------------------------------+
| Richard Stallman nel 1985         | Eric Raymond e Bruce Perens nel   |
|                                   | 1998                              |
+-----------------------------------+-----------------------------------+
| Copyleft (vs copyright) =         | Copyleft                          |
| permesso (left) di copia          |                                   |
+-----------------------------------+-----------------------------------+
| Free Software Foundation (FSF)    | Open Source Iniziative (OSI)      |
+-----------------------------------+-----------------------------------+
| Il software libero si basa su 4   | La definizione di open source si  |
| libertà                           | basa su 10 principi               |
|                                   |                                   |
| 1 e 3: prerequisito dell'accesso  |                                   |
| al codice sorgente                |                                   |
+-----------------------------------+-----------------------------------+

Il **copyleft**\ (o permesso d’autore) è una condizione per la quale il
licenziatario che intende ridistribuire il software originario - o
(anche) un software basato sul software originario - non può aggiungere
alla licenza restrizioni ulteriori rispetto alle condizioni previste
nella licenza originaria (ovvero, tendenzialmente, con la medesima
licenza di origine).\ |image57|

La clausola di copyleft, nelle intenzioni dei promotori, difende il
principio di “apertura” del codice originario.

Le **licenze permissive** non sono vincolate alla clausola copyleft e
quindi consentono anche l’utilizzo di codice aperto in combinazione con
combinazione con software disciplinato da licenze diverse, eventualmente
anche non Open Source; inoltre non limitano in alcun modo la
distribuzione dei prodotti derivati. Il licenziatario generalmente
richiede la citazione dell’autore e/o una frase che identifica la fonte
del documento e, ove fattibile, un collegamento alle pertinenti
informazioni sulla licenza, non ponendo particolari limitazioni
all’utilizzo o alla modifica dell’opera di ingegno.

La **licenza copyleft** ha la clausola copyleft al fine di assicurare
che il codice resti libero o aperto, prevedendo condizioni alla
ridistribuzione dei prodotti derivati (es. GPL` [41]_`).

La caratteristica “copyleft” delle licenze viene poi qualificata “forte”
o “debole” a seconda dell’ampiezza del vincolo stesso applicato alla
nozione di “modifica” e di “redistribuzione”.

Una licenza copyleft è considerata più o meno forte a seconda del modo
in cui si propaga nelle **opere derivate**. Per opera derivata si
intende, secondo l’art. 4 della L. 633/1941 sul diritto d’autore,
un’opera realizzata attraverso “elaborazioni di carattere creativo
dell'opera stessa, quali le traduzioni in altra lingua, le
trasformazioni da una in altra forma letteraria od artistica, le
modificazioni ed aggiunte che costituiscono un rifacimento sostanziale
dell'opera originaria, gli adattamenti, le riduzioni, i compendi, le
variazioni non costituenti opera originale”.

Con "**copyleft debole**" ci si riferisce alle licenze per le quali non
è richiesto che tutte le opere derivate ereditino la stessa licenza
copyleft. Solo le modifiche al software rilasciato con queste licenze
dovranno essere ridistribuite con la stessa licenza copyleft, ma tale
obbligo non si estende ad opere più ampie come ad esempio quelle che
utilizzano librerie rilasciate sotto licenza copyleft debole.

Questa licenza mantiene intatta la viralità per quanto riguarda
modifiche al codice originario, ma ne permette l’integrazione esterna da
parte di un software distribuito sotto qualunque licenza.` [42]_`

Con "**copyleft forte**" si intendono quelle licenze per cui tutte le
opere derivate, nella più ampia concezione del termine, ereditano la
stessa licenza copyleft (libertà 3 più vincolante a favore della
condivisione). In questo caso il copyleft forte può voler condizionare
tutti o quasi i codici che in qualche modo interagiscono con il software
originario per produrre l'eventuale programma eseguibile binario. La
licenza copyleft forte diventa anche “viralizzante” se il codice
protetto da copyleft viene combinato con codice non protetto da
copyleft.` [43]_` .

Si intende con “\ **Network copyleft**\ ”, quel tipo di licenze per cui
è necessario rendere disponibile il codice sorgente del programma
tramite un servizio `on demand <https://it.wikipedia.org/wiki/On_demand_(informatica)>`__
online, collegandosi al server presso il quale il software è eseguito
come servizio (`Software as a service o “SaaS” <https://it.wikipedia.org/wiki/Software_as_a_service>`__).
Risulta quindi ancora più restrittivo e quindi più viralizzante del
copyleft forte.` [44]_`

In base alle tipologie di licenze sopra descritte, alle caratteristiche
di ognuna e in particolare alla clausola di copyleft, è evidente come la
combinazione di software licenziati in modo differente possa portare
problemi di **compatibilità di licenze** sul software risultante.

Due licenze di software libero o open sono compatibili quando,
rispettando le condizioni poste da entrambe, è possibile combinare il
codice sorgente dei programmi licenziati per realizzare un’opera
derivata da essi, come sinteticamente descritto nella tabella seguente.

+------------------+-------------+
| **Licenza**      | **Esempio** |
+------------------+-------------+
| permissiva       |             |
+------------------+-------------+
| copyleft debole  |             |
+------------------+-------------+
| copyleft forte   |             |
+------------------+-------------+
| network copyleft |             |
+------------------+-------------+

Bisogna inoltre porre attenzione al fatto che la compatibilità non
sempre è bi-laterale e di fatto non è detto a priori che per software
diversi, il semplice fatto di essere liberi possano essere
“liberamente”combinati tra di loro.

In base a queste considerazioni, diventa fondamentale progettare e
realizzare un nuovo software ponendo particolare attenzione a due
aspetti:

-  valutare in itinere e non a sviluppo terminato le licenze di software
   terzi eventualmente coinvolte (sia sw linkato sia sw incorporato);

-  effettuare scelte coerenti con la licenza con cui si vuole rilasciare
   il software finale (**strategia di licensing iniziale**).

In generale è interessante quanto riportato in modo sintetico nelle
linee guida Agid sull’acquisizione e il riuso del software per la
PA` [45]_` (Allegato C, cap. “Compatibilità tra le licenze”) che
per comodità si riporta di seguito:

“\ *La compatibilità delle licenze dipende dalla cessione dei diritti
intellettuali da parte dell’autore. Le licenze che in questo senso
cedono meno diritti, al fine di preservare maggiormente nel tempo la
libertà e riutilizzabilità del software creato, sono le licenze
copyleft.*

*Quando si parla di compatibilità occorre distinguere due casi:*

-  *La creazione di una nuova opera a partire da componenti già
   esistenti, con licenza unica*

-  *L’assemblaggio e la distribuzione di più componenti interagenti,
   ognuna con licenza differente.*

*Per quanto riguarda il caso di creazione di una nuova opera sotto una
licenza unica, la matrice di compatibilità è la seguente:*

-  *Opere rilasciate sotto dominio pubblico sono rilasciabili con
   qualunque altra licenza*

-  *Opere rilasciate sotto licenze non-copyleft sono rilasciabili con
   licenze copyleft*

-  *Opere rilasciate sotto licenze copyleft possono essere solo
   rilasciate con licenze copyleft, a condizione che le due licenze
   siano compatibili*

*Nel secondo caso invece:*

-  *Opere rilasciate sotto licenza di pubblico dominio, non-copyleft o
   copyleft debole possono interagire come componenti a sé stanti con
   qualunque altro applicativo, pur rispettando le eventuali clausole
   riguardo riferimenti al codice originali e la distribuzione di
   eventuali modifiche.*

-  *Opere rilasciate sotto licenza copyleft possono interagire come
   componenti a sé stanti solo con altri componenti rilasciati con
   licenza copyleft compatibile.*\ ”

.. [37] Secondo l’art. 2, c. 8 della L. 633/1941 (aggiornata dalla L.37/2019), n. 37 LDA, sono tutelati «\ \ *i programmi per elaboratore, in qualsiasi forma espressi purché originali quale risultato di creazione intellettuale dell'autore. Restano esclusi dalla tutela accordata dalla presente legge le idee e i principi che stanno alla base di qualsiasi elemento di un programma, compresi quelli alla base delle sue interfacce. Il termine programma comprende anche il materiale preparatorio per la progettazione del programma stesso.*\ \ »

.. [38] *Il perimetro della brevettabilità del software è in evoluzione anche se formalmente non è brevettabile, ai sensi dell’art. 52 della Convenzione del Brevetto Europeo (Trattato internazionale che ha istituito l'Organizzazione Europea dei Brevetti al fine di offrire un brevetto unico valido in tutti gli Stati) e dell’art. 45 del Codice della Proprietà industriale (D. Lgs. 10/2/2005, n. 30). Si sta però affermando l’interpretazione secondo cui sono brevettabili soluzioni che integrino un dispositivi/apparecchiature e software ritenuto innovativo, nuovo e idoneo a produrre un “effetto tecnico” che è “ulteriore” rispetto alla mera interazione con la macchina.*

.. [39] Agreement on Trade Related Aspects of Intellectual Property Rights, trattato internazionale promosso dall'Organizzazione mondiale del commercio, meglio conosciuta WTO, al fine di fissare lo standard per la tutela della proprietà intellettuale, ufficializzato a Marrakech nel 1994, al termine del negoziato Uruguay Round. (fonte: https://it.wikipedia.org/wiki/Accordo_TRIPs)

.. [40] https://it.wikipedia.org/wiki/Licenza_libera

.. [41] `https://it.wikipedia.org/wiki/GNU_General_Public_License#:~:text=La%20GNU%20General%20Public%20License,per%20il%20sistema%20operativo%20GNU. <https://it.wikipedia.org/wiki/GNU_General_Public_License#:~:text=La%20GNU%20General%20Public%20License,per%20il%20sistema%20operativo%20GNU.>`__

.. [42] Ad esempio la MPL 2.0 definisce “\ \ *Permissions of this weak copyleft license are conditioned on making available source code of licensed files and modifications of those files under the same license (or in certain cases, one of the GNU licenses). Copyright and license notices must be preserved. Contributors provide an express grant of patent rights. However, a larger work using the licensed work may be distributed under different terms and without source code for files added in the larger work*\ \ ”

.. [43] Ad esempio la GNU GPLv3 riporta ”\ \ *Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights*\ \ ”.

.. [44] * Ad esempio la GNU AGPLv3, oltre a quanto indicato nella GPL3, riporta quanto segue: “When a modified version is used to provide a service over a network, the complete source code of the modified version must be made available”.*

.. [45] `https://www.agid.gov.it/sites/default/files/repository_files/lg-acquisizione-e-riuso-software-per-pa-docs_pubblicata.pdf <https://www.agid.gov.it/sites/default/files/repository_files/lg-acquisizione-e-riuso-software-per-pa-docs_pubblicata.pdf>`__


