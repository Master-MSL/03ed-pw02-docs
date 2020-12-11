App regionali di interfacciamento ai device integrate con il sistema Taccuino del FSE regionale
==================================================================================================================

Come definito in precedenza, per l’evoluzione del Taccuino al fine di
facilitare l’acquisizione di dati provenienti da device medicali e
wearable, si è considerata la necessità di sviluppare app regionali per
i sistemi operativi più diffusi sul mercato: Android e iOS.

Sistemi operativi mobile e linguaggi
-------------------------------------------

**Android** è un sistema operativo per dispositivi mobili sviluppato da
Google e basato sul kernel Linux, progettato principalmente per sistemi
embedded come smartphone e tablet, televisori (Android TV), automobili
(Android Auto), orologi da polso (Wear OS), occhiali (Google Glass),
etc. 

E’ distribuito con **licenza Apache 2.0.**\

Le app sono le applicazioni software installabili su Android scaricabili
sia dal catalogo ufficiale Google Play, sia da altri cataloghi, come
l'Amazon Appstore di Amazon.com, o **F-Droid**\ che contiene solo
applicazioni FOSS (Free and Open Source Software). Le app possono essere
installate direttamente a partire da un file APK.\ 

Le applicazioni Android sono Java-based.

**iOS**\ è un sistema operativo sviluppato da Apple per iPhone, iPod
touch e iPad. Da Settembre 2019, per i tablet iPad è stato sostituito da
iPadOS.\ 

Come per macOS (sistema operativo per PC Apple), iOS è una derivazione
di UNIX (famiglia BSD) ed è utilizzabile solo su dispositivi prodotti da
Apple con SoC (System On a chip) della serie di processori Apple A.

Dal 2008 è stato distribuito un SDK (software development kit) che
permette agli sviluppatori di creare applicazioni (cosiddette app) per
iPhone e iPod touch e di testarle in un simulatore. Tuttavia il
caricamento di una applicazione nei dispositivi è possibile solamente
dopo aver pagato una tassa di iscrizione all'iOS Developer Program di
Apple. Le app vengono pubblicate e scaricate dagli utenti dall’App
Store.\

L'ambiente di sviluppo per iOS SDK è Xcode, disponibile solamente per il
sistema operativo macOS. Le app possono essere sviluppate in Objective-C
o Swift.\ 

Gli sviluppatori sono liberi di definire qualsiasi prezzo per le loro
app pubblicate su App Store, ma riceveranno il 70% del ricavo (il 30%
viene trattenuto dalla Apple). Essi possono anche optare per pubblicare
gratuitamente l'applicazione non pagando nessun costo di pubblicazione
eccetto la tassa di sottoscrizione al programma developer.

App Regionale del Taccuino
----------------------------------

Prendendo in considerazione esclusivamente il software che realizza le
app regionali per la gestione del Taccuino del FSE e prendendo come
riferimento le indicazioni delle Linee guida Agid su acquisizione e
riuso di software per le pubbliche amministrazioni al capitolo “3.5.3
Scelta di una licenza”, si valuta il rilascio del software con licenza
copyleft debole `EUPL 1.2 <https://spdx.org/licenses/EUPL-1.2.html>`__\ **(codice
SPDX** [51]_\ **: EUPL-1.2)** a meno di utilizzo in corso di
sviluppo di librerie irrinunciabili rilasciate con licenze AGPL, GPL 2 o
GPL 3, che, in ragione delle caratteristiche di viralità sopra esposte,
richiederebbero una ri-valutazione relativa al rilascio del sistema nel
suo complesso, presumibilmente da pubblicare in coerenza con una delle
suddette licenze “forti”.

Al netto di tale ipotesi, la scelta della licenza europea, derivata
dalle indicazioni inserite nelle linee guida Agid, è motivata anche
dalle seguenti caratteristiche:

-  **licenza multilingua:** la licenza è scritta in 23 lingue della
   comunità europea con uguale valore legale (diversamente da altre
   licenze OS che ha valore legale solo la versione in lingua inglese)

-  **contesto giuridico:** è conforme alla normativa europea sulla
   tutela del diritto d’autore e del software (diversamente da altre
   licenze OS che fanno riferimento al contesto giuridico statunitense).

-  **compatibilità:** l’opera rilasciata in EUPL e le sue modifiche
   devono rimanere licenziate in EUPL, ma un “larger work” derivato da
   combinazioni di detta opera con elementi rilasciati con una tra le
   licenze presenti nella lista di compatibilità, potranno essere
   rilasciati sotto quest’ultima. Si cita il seguente estratto ripreso
   da
   https://joinup.ec.europa.eu/collection/eupl/news/understanding-eupl-v12
   “EUPL v1.2 has a wider coverage: it cover “the Work” (meaning
   copyrighted work) and not exclusively “the software”. Therefore it is
   easier to apply the EUPL v1.2 to related documentation, handbooks,
   standard specifications etc. EUPL v1.2 has a wider compatibility: the
   software itself (copies or modifications/improvements) will stay
   covered by the EUPL without possibilities of re-licensing by
   recipients, but it may also be merged in a new – other - larger work
   with other software components covered by compatible licences. When
   needed and for avoiding licence conflicts, this other derivative work
   can then be distributed under the compatible licence. The list of
   compatible licences includes both the GPLv2 and v3, the AGPL, MPL,
   EPL, LGPL and other licences. Regarding documents, compatibility
   includes the Creative Common licence CC BY SA. The purpose of this
   compatibility list is not to endorse or recommend the listed
   licences: it is finding interoperable solutions to possible licence
   conflicts. This is the reason why the list includes SA (share alike)
   or copyleft licences, and not the most permissive ones.”.

.. |image73| figure:: /immagini/10000201000002C10000031CB83DE4010C4D129A.png
   :scale: 50 % 
   :alt: fonte: `https://joinup.ec.europa.eu/collection/egovernment/document/eup <https://joinup.ec.europa.eu/collection/egovernment/document/eupl>`__

   fonte: `https://joinup.ec.europa.eu/collection/egovernment/document/eup <https://joinup.ec.europa.eu/collection/egovernment/document/eupl>`__


Può risultare utile in fase di sviluppo tenere presente la
matrice\ **“Matrix of EUPL compatible open source licences”** pubblicata
nell’ambito del progetto europeo joinup all’indirizzo
https://joinup.ec.europa.eu/collection/eupl/matrix-eupl-compatible-open-source-licences
che aiuta nel valutare la compatibilità fra software EUPL e software di
terze parti rilasciato in differenti licenze open source integrato
secondo le modalità:

-  *incorporamento* (inserimento di porzioni di codice di terze parti
   all’interno del proprio prodotto software)

-  *link statico* (si riferisce ad una libreria software che nel proprio
   prodotto viene collegata staticamente in fase di compilazione)

-  *link dinamico* (si riferisce ad una libreria software che nel
   proprio prodotto viene caricata dinamicamente in fase di esecuzione)

**Il titolare del software nonché licenziante è la Regione
Piemonte** [52]_ che verrà indicata nel file copyright.txt e in
tutti documenti in cui deve essere esplicitato tale copyright. Tale
titolarità, dovrà poi essere gestita nel rispetto dei diritti coinvolti
in fase di amministrazione della community e dei relativi auspicabili
contributi.

Riprendendo l’art. 6 della legge italiana sul **diritto d’autore (L. 22
aprile 1941, n. 633, d’ora in poi “LDA“)** il diritto d’autore (e il suo
corrispondente anglo-americano copyright) è lo strumento giuridico per
eccellenza posto a tutela dell’attività creativa, quale particolare
espressione del lavoro intellettuale. Inoltre, in base alle disposizioni
di cui all’art. 2 LdA, anche i programmi per elaboratore vengono
tutelati alla stregua di “opere creative”, con le conseguenze di seguito
sommamente sintetizzate.

*Il diritto d’autore tutela il programma come codice ovvero nella forma
in cui è scritto e non tutela l’idea che ne sta alla base (algoritmo).
La tutela si estende anche ai lavori preparatori.*\ Come le opere
creative, la LDA definisce che il software nasce con la sua creazione.
Si costituisce in capo al “creatore” individuale che acquisisce un
fascio di diritti.

**Il diritto d’autore comprende sia i diritti morali (art. 20 e segg.)
sia quelli patrimoniali/economici (art. 64 bis e segg.) secondo la
LDA.**

.. |image74| figure:: /immagini/10000201000003CD00000202EAA0270ADB2D4E8E.png
   :scale: 80 % 
   :alt: Fonte: Avv. Vitrani “Diritto d'autore: diritti esclusivi e limitazioni”, Master “Management Software Libero” 2019/2020

   Fonte: Avv. Vitrani “Diritto d'autore: diritti esclusivi e limitazioni”, Master “Management Software Libero” 2019/2020


I **diritti morali** sono i diritti del creatore a essere riconosciuto
come autore dell’opera e a rivendicarne la paternità. Sono diritti
inalienabili, imprescrittibili e irrinunciabili, cioè possono essere
esercitati indipendentemente dai diritti patrimoniali derivanti dalla
creazione dell’opera e anche nel caso in cui questi ultimi siano stati
ceduti a terzi.

I **diritti patrimoniali** sono trasferibili e individuano una serie di
diritti relativi allo sfruttamento ed alla messa a disposizione
dell’opera.

Si specifica inoltre che la normativa vigente dà disposizioni relative
al\ **lavoro dipendente**, e quindi secondo art. 12 bis della LDA,
“Salvo patto contrario, il datore di lavoro è titolare del diritto
esclusivo di utilizzazione economica del programma per elaboratore o
della banca di dati creati dal lavoratore dipendente nell'esecuzione
delle sue mansioni o su istruzioni impartite dallo stesso datore di
lavoro.”

**Si precisa infine che i diritti relativi alla titolarità del SW
vengono definiti dal CSI con Regione Piemonte e con i propri fornitori
ed attribuiti contrattualmente in forma chiara ed esauriente,
rispettivamente sia nei documenti del ciclo attivo (PTE, CTE, etc.) che
passivo (Contratti, Capitolati, etc.) con apposite clausole
contrattuali.**

*Gli sviluppi previsti per l’evoluzione del taccuino, nella fattispecie
la realizzazione delle app regionali potrebbero essere sviluppate
internamente al CSI (vedi sopra citato art. 12 bis della LDA) oppure
affidate tramite appalto a fornitori esterni vincolati da contratto con
clausole specifiche che consentono di attribuire la titolarità del
software alla Regione Piemonte.*

Citando le linee guida Agid su acquisizione e riuso di software per le
pubbliche amministrazioni, “Ad esempio, espressioni come quelle che
seguono, ove presenti nei contratti per lo sviluppo di software
consentono di ritenere che l’amministrazione sia titolare dei diritti
nel senso richiesto dall’articolo 69 del CAD:

-  «il committente sarà titolare del software sviluppato»;

-  «la proprietà della soluzione informatica oggetto del contratto farà
   capo al committente o all’Amministrazione»;

-  «al termine del contratto la proprietà intellettuale sulla soluzione
   informatica oggetto di sviluppo competerà all’amministrazione
   committente»;

-  «tutti i diritti d’autore sul software sviluppato verranno
   trasferiti, a seguito del completamento dell’opera,
   all’amministrazione committente che ne diverrà titolare»;

-  «tutti i diritti di sfruttamento economico sul software oggetto del
   contratto competono all’amministrazione committente».

Sempre tali linee guida danno indicazioni in tal senso prevedendo quanto
segue:

-  “Ogni amministrazione deve, in sede di negoziazione di un contratto
   volto a commissionare lo sviluppo di un software, garantirsi,
   all’esito dell’esecuzione del contratto, la piena ed esclusiva
   titolarità di tutti i diritti sul software oggetto di sviluppo,
   [...]”;

-  “Un’amministrazione, ai sensi dell’articolo 69, deve egualmente
   acquisire la totalità dei diritti di proprietà intellettuale e
   industriale su eventuali personalizzazioni o moduli software
   destinati a integrarsi o interfacciarsi con un software proprietario.
   In tal caso, l’obbligo di cui all’art. 69 avrà ad oggetto
   esclusivamente il modulo o la parte del software oggetto di sviluppo;
   tale modulo dovrà quindi essere separato dal resto del software e
   rilasciato secondo le modalità indicate in Sviluppo di software ex
   novo (pagina 30), avendo cura di indicare la necessaria dipendenza
   proprietaria nella documentazione.”;

-  “La mancata acquisizione della titolarità dell’opera non può essere
   utilizzata per ottenere condizioni economiche più vantaggiose, poiché
   non costituisce comprovata ragione di carattere tecnico-economico ai
   sensi dell’articolo 69 comma 2 del CAD.”.

In ragione di quanto sopra, quindi, la soluzione pubblicata
correttamente viene rilasciata come titolarità di Regione Piemonte, pur
rimanendo i diritti morali in capo ai singoli sviluppatori che andranno
richiamati nel file authors.txt incluso nella documentazione del
prodotto e pubblicato sul code hosting repository (l’autore può chiedere
l’anonimato ossia la pubblicazione senza indicazione del proprio nome o
dietro pseudonimo).

Per la documentazione tecnica del software, si intende utilizzare la
licenza Creative Commons `CC-BY 4.0 <https://spdx.org/licenses/CC-BY-4.0.html>`__\ **(codice SPDX: CC-BY-4.0)**. Questa licenza permette un riutilizzo semplice della
documentazione e degli esempi di codice in essa contenuta.

.. [51] **Codice sPDX è un codice identificativo univoco delle licenze riconosciute dalla OSI**

.. [52] **Vi è trasferimento dei diritti di utilizzazione economica del software creato su commissione da CSI-Piemonte a Regione Piemonte**
