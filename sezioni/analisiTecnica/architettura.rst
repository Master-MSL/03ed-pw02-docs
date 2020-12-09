Architettura del sistema
==========================

In questo capitolo viene descritta l’architettura AS-IS del FSE
regionale in cui si colloca la soluzione software del Taccuino
attualmente disponibile per assistiti della Regione Piemonte e per gli
operatori sanitari. Partendo dall’as-is si approfondiscono le componenti
del Taccuino per arrivare a contestualizzare e descrivere più in
dettaglio la proposta di evoluzione.

Architettura AS-IS del FSE
--------------------------------

Modello federato a livello nazionale
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A livello nazionale è stato definito un modello federato di FSE che si
basa sulla cooperazione dei nodi regionali che ospitano l’infrastruttura
tecnologica che realizza il sistema regionale di FSE.

Tutti i nodi regionali cooperano secondo una gerarchia paritetica
esponendo ed invocando i servizi realizzati dagli altri nodi necessari
alla condivisione del contenuto informativo del FSE a livello nazionale.
I nodi regionali prevedono la presenza di tutte le componenti
infrastrutturali del FSE e sono in grado di garantire tutte le
funzionalità necessarie alla gestione, ricerca e consultazione dei dati
e documenti di propria competenza (ossia relativi ai propri assistiti),
ovunque essi siano disponibili, e alla comunicazione con gli altri nodi
regionali. In particolare, il modello prevede che la Regione di
Assistenza (RDA) di un assistito abbia l’onere di mantenere la gestione
dei riferimenti ai documenti riguardanti i propri assistiti, anche se
tali documenti sono prodotti e conservati in altri domini regionali.
Pertanto, i sistemi di FSE devono essere in grado di trasmettere e
ricevere i metadati relativi ai documenti trattati e prodotti durante il
percorso di cura dell'assistito. In questo scenario di funzionamento,
ogni dominio regionale interagisce con la RDA di un paziente e comunica
con il sistema di FSE di quest’ultima. La gestione dei metadati relativi
ai documenti clinici da parte della RDA implica la costruzione di un
indice dei documenti appartenenti al FSE di un assistito. In questo
modo, per effettuare la ricerca dei metadati dei documenti di un dato
paziente, occorre interrogare unicamente l’indice presente nel nodo
regionale del sistema della RDA del paziente e recuperare i documenti
dalla regione che lo ha prodotto.

.. |image25| figure:: /immagini/1000020100000407000002A4869DEDC724F2A515.png
   :scale: 80 % 
   :alt: Federazione FSE

   Federazione FSE

Secondo tale modello i sistemi regionali di Fascicolo Sanitario
Elettronico (FSE) inter-operano con gli altri attraverso un nodo
nazionale detto INI - Infrastruttura Nazionale di Interoperabilità - al
fine di collezionare, richiedere e trasmettere metadati e documenti
sanitari attraverso modalità sicure e nel rispetto dei consensi
stabiliti dagli assistiti.

.. |image26| figure:: /immagini/10000201000004050000029686775BE5EC1D1CDA.png
   :scale: 80 % 
   :alt: Architettura dell'Infrastruttura Nazionale di Interoperabilità (INI)

   Architettura dell'Infrastruttura Nazionale di Interoperabilità (INI)

Nell’ambito dei diversi processi interregionali, ciascuna regione o
provincia Autonoma può assumere i seguenti ruoli:

-  Regione Di Assistenza (**RDA**): ha l’onere di memorizzare e di
   rendere disponibili agli attori autorizzati, tutti i riferimenti
   (metadati) ai documenti e dati generati per i propri assistiti, anche
   se prodotti in altri domini regionali.

-  Regione Di Erogazione (**RDE**): eroga una prestazione sanitaria ad
   un paziente assistito da un altro dominio regionale.

-  Regione Contenente un Documento o dato (**RCD**): rappresenta il
   domino regionale in cui è disponibile un documento o dato sanitario o
   socio-sanitario che si intende consultare.

-  Regione Precedente Di Assistenza (**RPDA**): è un dominio regionale
   che, precedentemente al cambio della regione o provincia autonoma di
   assistenza da parte di un assistito, ha svolto per questi il ruolo di
   RDA.

I **servizi di interoperabilità nazionale** che ogni infrastruttura di
FSE deve esporre sono conformi a standard internazionali applicati in
ambito nazionale, secondo quanto indicato nelle specifiche di
interoperabilità del FSE previste da AgID (Agenzia per l’Italia
Digitale). L’uso dei servizi di interoperabilità è veicolato tramite
l’INI, che permette la comunicazione tra più domini regionali.

I servizi di interoperabilità implementati dai sistemi delle regioni e
province e dall’INI sono descritti di seguito:

-  *Ricerca dei documenti:*\ consente la consultazione dell’elenco dei
   documenti presenti nel FSE di un assistito.

-  *Recupero di un documento:*\ permette la consultazione di uno
   specifico documento presente nel FSE di un assistito.

-  *Comunicazione dei metadati:*\ consente ad un dominio regionale di
   informare la RDA di una avvenuta creazione di un documento per un
   assistito di quest’ultima, trasmettendo una serie di metadati
   associati al documento.

-  *Cancellazione dei metadati:*\ consente ad un dominio regionale di
   richiedere la cancellazione dei metadati associati ad uno specifico
   documento nel FSE.

-  *Trasferimento dell’indice del FSE:*\ consente alla RPDA di
   trasferire alla nuova RDA l’insieme dei riferimenti dei documenti del
   FSE e delle politiche di accesso ad essi associati.

-  *Gestione dei consensi e delle informative:*\ consente ad un dominio
   regionale di comunicare le informative regionali e i consensi
   raccolti all’INI.

-  *Gestione delle notifiche:*\ consente all’INI di notificare alla RDA
   eventi occorsi a propri assistiti in domini regionali differenti.

.. |image27| figure:: /immagini/10000201000002D30000017423289E90ECF0A19F.png
   :scale: 80 % 
   :alt: Specifiche tecniche per l’interoperabilità tra i sistemi regionali di FSE Framework e dataset dei servizi base

   Specifiche tecniche per l’interoperabilità tra i sistemi regionali di FSE Framework e dataset dei servizi base_Versione 2.1 pubblicate su https://www.fascicolosanitario.gov.it/



Modello regionale
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Il sistema del FSE della Regione Piemonte (FSEr) è stato progettato
secondo un’architettura fortemente distribuita, service oriented e
basata su standard aperti.

Di seguito vengono descritte le componenti del modello di
interoperabilità previsto a livello regionale:

-  una progressive web application (PWA) per il cittadino che gli
   consente di:

   -  gestire i dati personali di profilo;

   -  esprimere il consenso informato all’alimentazione e consultazione
      del proprio fascicolo e gestire i criteri di visibilità dei dati
      presenti nel proprio FSE;

   -  consultare la propria storia clinica presente nel fascicolo;

   -  consultare gli accessi ai dati del FSE da parte degli operatori;

-  una web application responsive per operatori sanitari per la
   consultazione del fascicolo sanitario dei propri assistiti;

-  una web application per operatori amministrativi che consente di
   attivare “punti assistiti” in cui gli operatori delle ASR (Azienda
   Sanitaria Regionale) o di altri enti abilitati possono agire in nome
   e per conto del cittadino e offrire ai propri assistiti i seguenti
   servizi:

   -  aprire il Fascicolo di un cittadino;

   -  gestirne i consensi al livello generale;

   -  effettuare l’oscuramento di documenti specifici;

   -  ritirare i referti online e consegnarne una copia cartacea;

-  un nodo centrale (componente centrale) comprensivo di

   -  un Indice Regionale degli Eventi Clinici (IREC), privo di dati
      sensibili, nel quale sono mantenute le informazioni degli
      assistiti della Regione Piemonte che hanno creato il proprio FSE e
      sono presenti i riferimenti alle componenti locali in cui
      risiedono i metadati dei documenti clinici conservati nel
      repository aziendale;

   -  servizi di interoperabilità a livello regionale per la gestione
      dei consensi, per l’invio di varie tipologie di notifiche, per
      operazioni di consultazione di metadati e documenti, etc

   -  servizi di interoperabilità per il colloquio con i sistemi delle
      altre regioni e province autonome attraverso INI;

-  un nodo locale (componente locale) dedicato a:

   -  ogni ASR,

   -  strutture Private accreditate al SSN con e senza Repository in cui
      vengono conservati e resi disponibili i documenti clinici

   -  gestione dei metadati e dei documenti (patient summary, bilancio
      di salute e piano di cura personalizzato) prodotti dalle cartelle
      cliniche elettroniche (CCE) di MMG (Medici di Medicina Generale) /
      PLS (Pediatri di Libera Scelta,

   -  gestione di ricette indicizzate da INI
      (specialistiche/farmaceutiche, prescritto/erogato),

   -  gestione dei metadati di documenti clinici prodotti da altre
      Regioni per gli assistiti piemontesi,

   -  taccuino personale

   e costituito da:

-  

   -  un Indice locale degli Eventi Clinici (ILEC) che gestisce i
      metadati clinici utili all’interoperabilità regionale e nazionale;

   -  servizi di interoperabilità verso il nodo centrale per la gestione
      delle anagrafiche e per

      -  la gestione delle richieste di consultazione dei fascicoli e
         dei documenti da parte di operatori sanitari operanti in altre
         regioni o province autonome;

      -  la gestione delle ricette farmaceutiche e specialistiche
         (erogato e prescritto) provenienti da altre Regioni e/o dal
         SistemaTS attraverso INI;

      -  la gestione dei documenti clinici interoperabili provenienti da
         altre regioni attraverso INI;

      -  la gestione del Taccuino Personale;

   -  servizi di interoperabilità per:

      -  l’integrazione di sistemi dell'area clinica delle ASR e
         strutture private (via HL7 o WS XML/SOAP);

      -  l’integrazione di cartelle cliniche elettroniche (CCE) di
         MMG/PLS (via WS XML/SOAP secondo tracciati INI usati per le
         regioni in sussidiarietà).

.. |image28| figure:: /immagini/10000201000003C3000002923F782D3D320232E0.png
   :scale: 80 % 
   :alt: Architettura logica del sistema AS-IS del FSE della Regione Piemonte

   Architettura logica del sistema AS-IS del FSE della Regione Piemonte



Architettura TO-BE del Taccuino personale
------------------------------------------------

Nella figura riportata di seguito, si focalizza in particolare
l’attenzione sull’architettura del taccuino rispetto al precedente
diagramma “Architettura logica del sistema FSE della Regione Piemonte”.

.. |image29| figure:: /immagini/10000201000002D800000174C6150F2C15790F7A.png
   :scale: 80 % 
   :alt: Architettura logica del sistema AS-IS del FSE della Regione Piemonte (focus Taccuino)

   Architettura logica del sistema AS-IS del FSE della Regione Piemonte (focus Taccuino)


Si può rilevare come il sistema di Taccuino venga realizzato attraverso
più componenti, colorate in rosso, distribuite nel sistema FSEr:

-  componente dedicata all’interno della progressive web application
   (PWA) rivolta al cittadino che si interfaccia via API Json/rest al
   backend su più tier per l’alimentazione, gestione e consultazione dei
   dati e documenti presenti nel taccuino

-  componente dedicata all’interno della web application rivolta agli
   Operatori Sanitari che si interfaccia via Web Services (WS) al
   backend su più tier per la consultazione dei dati e documenti
   presenti nel taccuino non oscurati dal cittadino

-  servizi specifici per realizzare l’interoperabilità a livello
   regionale e in futuro nazionale;

-  componente locale dedicata alla gestione dei metadati, dei dati e dei
   documenti del Taccuino.

In base agli scenari di integrazione individuati al capitolo `Modalità
di integrazione dei device <#_8dnz78msojq0>`__, si riporta un diagramma
architetturale che evidenzia come le nuove componenti APP per smartphone
si possano inserire nel sistema regionale complessivo di Taccuino e di
FSE. In particolare si prevede la realizzazione di un'\ **app regionale
nativa per sistemi IOS e Android**\ in grado di interfacciarsi ai device
medicali e wearable nelle modalità descritte in precedenza:

1. integrazione diretta

2. integrazione indiretta attraverso uso di SDK/API di Health App

3. integrazione indiretta attraverso export/import di dati da Health
   App/app di terzi

al fine di migliorare ed automatizzare il più possibile le modalità di
acquisizione dei dati da parte di diverse tipologie di device medicali e
wearable.

.. |image30| figure:: /immagini/10000201000003B100000293319256ABC22C5E7D.png
   :scale: 80 % 
   :alt: Architettura logica del sistema TO-BE del FSE della Regione Piemonte

   Architettura logica del sistema TO-BE del FSE della Regione Piemonte


L’app regionale deve inoltre interfacciarsi al sistema regionale di FSE
invocando le API rest rese disponibili per l’accesso alle risorse del
Taccuino.

L’integrazione fra l’app regionale e le API del Taccuino, esposte su
Internet, in particolare, deve implementare **protocolli di sicurezza**
in grado di garantire la protezione dei dati personali e sensibili
trattati. Deve essere progettato e realizzato un meccanismo in grado di
verificare che l’app che richiede l’accesso ad una risorsa del Taccuino
sia autorizzata e che l’utente che accede all’app sia effettivamente il
proprietario della risorsa richiesta e resa disponibili attraverso le
API rest del Taccuino.

L’app inoltre deve consentire all’utente di autenticarsi con
**credenziali imputabili**\ come ad esempio\ **SPID.**

Per migliorare l’usabilità dell’app, si può anche prevedere di gestire
una `sessioni lunga
revocabile <https://docs.italia.it/AgID/documenti-in-consultazione/lg-openidconnect-spid-docs/it/bozza/sessioni-lunghe-revocabili/ambiti-e-limiti-di-utilizzo.html>`__
dopo l’autenticazione che ad ogni accesso all’app richieda l’inserimento
di un **PIN locale** scelto dall’utente o in alternativa l’uso di
**identificazione biometrica** disponibile sullo smartphone: *impronta
digitale oppure riconoscimento facciale (solo iOS)[27]_

.. |image31| figure:: /immagini/10000201000003CC000002928AC45E7B303F1A41.png
   :scale: 80 % 
   :alt: Architettura logica delle App del Taccuino

   Architettura logica delle App del Taccuino


Nella fase di analisi e progettazione dell’app saranno analizzati ed
approfonditi i protocolli necessari a garantire gli adeguati livelli di
sicurezza (come ad esempio OpenID Connect e OATH2) nell’ambito
dell’autenticazione e autorizzazione degli utenti e delle app per
l’accesso alle risorse del Taccuino del sistema regionale del FSE.

Si ritiene pertanto necessario prevedere una POC (Proof of Concept) per
verificarne in dettaglio l’applicabilità di tali aspetti e gli impatti
infrastrutturali di questi sull’intera soluzione software.

.. [27] *l’ipotesi di usare una sessione lunga revocabile, PIN locale e riconoscimento biometrico è ispirata all’attuale gestione fatte dall’*\ \ \ `app IO <https://io.italia.it/>`__