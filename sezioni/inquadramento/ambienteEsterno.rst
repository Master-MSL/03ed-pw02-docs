Analisi dell’ambiente esterno
==============================

E’ facile rilevare come il progetto di Evoluzione del Taccuino Personale
e più in dettaglio il sistema organizzativo di una Community Open Source
possano essere influenzati da diversi fattori che fanno parte
dell’ambiente esterno al contesto di riferimento e che appartengono a
diversi ambiti: legislativo, politico-economico, tecnologico-culturale,
sociale e fisico.

Fattori politico-legislativi
-------------------------------

Normativa di riferimento per il FSE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Da un punto di vista politico-legislativo, il Taccuino e più in generale
il sistema di fascicolo sanitario sono soggetti alla normativa nazionale
e comunitaria in materia di protezione dei dati personali, ed in
particolare:

-  D.L. n. 196 del 30 giugno 2003 "Codice in materia di protezione dei
   dati personali" e s.m.i.;

-  Regolamento Ue 2016/679, noto anche come GDPR (General Data
   Protection Regulation)

integrata da specifici indirizzi da parte del Garante privacy, nonché
alla normativa specifica, i cui capisaldi sono:

-  il D.L. n. 179 del 18 ottobre 2012 convertito con L. n. 221 del 17
   dicembre 2012, che (rif. Art. 12) ha di fatto istituito il FSE (Art.
   12);

-  il `DPCM n.178 del 29 settembre 2015 "Regolamento in materia di
   fascicolo sanitario
   elettronico" <http://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.del.presidente.del.consiglio.dei.ministri:2015-09-29;178!vig=>`__
   norma principale in materia, che definisce il primo modello di
   riferimento disciplinando contenuti, ruoli nonché modalità di
   realizzazione e fruizione del FSE;

-  la L. n. 232 dell’11 dicembre 2016 che, al fine di assicurare
   omogeneità a livello nazionale, ha variato il quadro di riferimento
   per gli scenari di evoluzione e diffusione del FSE con l’introduzione
   (art. 1, c. 382) dell’Infrastruttura Nazionale per l’Interoperabilità
   (INI) dei Fascicoli Sanitari Elettronici regionali, nonché con la
   revisione di adempimenti e scadenze previsti per la realizzazione dei
   progetti di FSE da parte delle Regioni.

Sulla base di tali atti fondamentali, è stata approvata una serie di
documenti tecnici e relative disposizioni che, a partire dal D.M. `4
agosto 2017 "Modalita' tecniche e servizi telematici resi disponibili
dall'infrastruttura nazionale per l'interoperabilita' del Fascicolo
sanitario elettronico (FSE)
[...]” <http://www.gazzettaufficiale.it/eli/id/2017/08/22/17A05772/sg>`__
e insieme ad altre disposizioni tecniche di rango inferiore hanno
costituito la base per l’implementazione o l’adeguamento tecnico del
FSE.

L’elenco completo della normativa di riferimento è riportato in
`Appendice A <https://taccuino-community-os.readthedocs.io/en/latest/12.appendice-normativa.html>`__.

Per la realizzazione dell’interoperabilità fra i sistemi regionali di
FSE attraverso INI, è stata emessa (a più riprese in relazione alla
complessità dell’argomento) abbondante documentazione tecnica, tra cui
linee guida di riferimento, manuali e documenti tecnici per lo sviluppo
e la gestione del Fascicolo Sanitario Elettronico (FSE) secondo quanto
stabilito dalla legge.

Le linee guida tecniche di riferimento in ambito nazionale per lo
sviluppo e l'implementazione dei documenti sanitari hanno altresì
previsto la definizione e l’adozione di standard documentali ottenuti
come risultato della collaborazione tra HL7 Italia\ :sup:` [4]_` e AgID
nell'elaborazione dei risultati dei Gruppi Tematici interregionali del
FSE istituiti da Ministero della Salute e da AgID stessa.

L’elenco esteso della principale documentazione tecnica ad oggi emessa è
riportato in `Appendice B <https://taccuino-community-os.readthedocs.io/en/latest/13.appendice-specifiche-nazionali.html>`__; eventuali aggiornamenti
sono conosultabili sulla pagina web
https://www.fascicolosanitario.gov.it/area-tecnica curata da AgID.

Normativa in ambito Open Source
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

L’art. 69 del Codice per l’amministrazione digitale (CAD) prevede, salvo
casi particolari, che “[...] le pubbliche amministrazioni che siano
titolari di soluzioni e programmi informatici realizzati su specifiche
indicazioni del committente pubblico, hanno l’obbligo di rendere
disponibile il relativo codice sorgente, completo della documentazione e
rilasciato in repertorio pubblico sotto licenza aperta, in uso gratuito
ad altre pubbliche amministrazioni o ai soggetti giuridici che intendano
adattarli alle proprie esigenze [...]”; in considerazione della natura
del software sviluppato per la realizzazione del FSE e del Taccuino
emerge come anche il FSE e il Taccuino siano soggetti alla normativa
sopra citata.

Inoltre le linee guida Agid per l’acquisizione e il riuso software nelle
PA\ :sup:` [5]_` prevedono (nel relativo Allegato A intitolato “Guida
alla pubblicazione di software come open source”) che sia individuato
uno strumento di code hosting da utilizzare per il rilascio. Allo stato
attuale, in virtù di tali indicazioni, il CSI-Piemonte, in qualità di
software maintainer incaricato dalle Amministrazioni titolari di
software (maintainer come da ruolo Agid\ :sup:` [6]_`), ha scelto il
sistema di code hosting GitHub (https://github.com/).

Modello regionale e nazionale del FSE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Essendo i sistemi di FSE regionali un insieme di servizi fortemente
influenzati dal modello di sanità digitale specifico di ogni di regione
e di conseguenza realizzati su paradigmi che poco si prestano alla
realizzazione di soluzioni disponibili in “riuso” o direttamente
acquisibili sul mercato, il FSE della Regione Piemonte (come in altre
Regioni) è stato realizzato nell’ultimo decennio e poi fatto evolvere,
come sistema strategico sviluppato ad hoc, per l’integrazione con INI
(Infrastruttura Nazionale per l’Interoperabilità) .

Con tale evoluzione, i sistemi regionali di Fascicolo Sanitario
Elettronico (FSE) inter-operano con INI al fine di collezionare,
richiedere e trasmettere dati e documenti sanitari attraverso modalità
sicure e nel rispetto dei consensi stabiliti dagli assistiti.

Nell’ambito dei diversi processi interregionali, ciascuna regione o
provincia Autonoma può assumere i seguenti ruoli:

-  Regione Di Assistenza (RDA): ha l’onere di memorizzare, e di rendere
   disponibili agli attori autorizzati, tutti i riferimenti (metadati)
   ai documenti e dati generati per i propri assistiti, anche se
   prodotti in altri domini regionali.

-  Regione Di Erogazione (RDE): eroga una prestazione sanitaria ad un
   paziente assistito da un altro dominio regionale.

-  Regione Contenente un Documento o dato (RCD): rappresenta il domino
   regionale in cui è disponibile un documento o dato sanitario o
   socio-sanitario che si intende consultare.

-  Regione Precedente Di Assistenza (RPDA): è un dominio regionale che,
   precedentemente al cambio della regione o provincia autonoma di
   assistenza da parte di un assistito, ha svolto per questi il ruolo di
   RDA.

I servizi di interoperabilità che ogni infrastruttura di FSE espone
devono essere conformi agli standard adottati, secondo quanto indicato
nelle specifiche di interoperabilità del FSE previste da AgID. Il loro
utilizzo, che permette le azioni di ricerca, recupero e gestione dei
documenti e delle notifiche previste, è veicolato tramite l’INI, che
permette la comunicazione tra più domini regionali come schematicamente
di seguito rappresentato.

.. |image2| figure:: /immagini/10000201000002D30000017423289E90ECF0A19F.png
   :scale: 80 % 
   :alt: Stakeholder del Taccuino Personale del FSE

   fonte: Specifiche tecniche per l’interoperabilità tra i sistemi regionali di FSE Framework e dataset dei servizi base_Versione 2.1 pubblicate su  https://www.fascicolosanitario.gov.it/



Il Taccuino - Dataset standard e soluzioni tecniche
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Come riportato in Premessa, il “Taccuino personale dell’assistito” è la
una sezione del FSE (e in quanto tale soggetta alle medesime regole di
visibilità e interoperabilità), la cui alimentazione è riservata
esclusivamente al cittadino, articolata in:

-  un insieme standard (nel seguito “data set”) di dati inseriti dal
   cittadino, condivisi e gestiti all’interno del proprio taccuino da
   tutte le Regioni;

-  un insieme di documenti caricati in auto-contribuzione direttamente
   dal cittadino (ad esempio upload di un referto proveniente da una
   struttura pubblica o privata accreditata non ancora integrata al
   FSE).

I contenuti informativi costituenti il data set standard sono
raggruppate in sezioni ed elementi secondo la logica di seguito
sintetizzata (elenco di dettaglio in `Appendice D <https://taccuino-community-os.readthedocs.io/en/latest/15.appendice-dataset.html>`__
licenziato dal GdL a dicembre 2019).

La sezione di interesse è quella naturalmente delle osservazioni
personali, in particolare l’elemento “parametri osservabili” costituito
da dati strutturati che potranno essere gestiti ed eventualmente estesi,
partendo dalle indicazioni del GdL per eventuali fasi successive di
lavoro:

A. elaborazioni dei dati quali per presentazione di medie, grafici e
   andamenti ecc.

B. evoluzione del data set, anche a seguito di un primo periodo di
   valutazione dell’utilizzo, attraverso l’analisi di ulteriori
   informazioni

C. rilevazione dati da strumenti di uso quotidiani (tramite opportune
   soluzioni sw/APP su dispositivi mobile o di altra natura);

D. ulteriori dati di dettaglio sui farmaci.

+-----------------------+-----------------------+-----------------------+
| **SEZIONE**           | **ELEMENTO**          | **CONTENUTO           |
|                       |                       | INFORMATIVO**         |
+-----------------------+-----------------------+-----------------------+
| Osservazioni          | Note generali         | Annotazioni libere    |
| personali             |                       |                       |
+-----------------------+-----------------------+-----------------------+
| Eventi\ :sup:` [11]_` | Eventi significativi  |                       |
|                       | ultimi 6 mesi         |                       |
+-----------------------+-----------------------+-----------------------+
| Parametri osservabili | Peso                  |                       |
|                       |                       |                       |
|                       | Circonferenza vita    |                       |
|                       |                       |                       |
|                       | Pressione             |                       |
|                       |                       |                       |
|                       | Frequenza cardiaca (a |                       |
|                       | riposo)               |                       |
|                       |                       |                       |
|                       | Frequenza             |                       |
|                       | respiratoria          |                       |
|                       |                       |                       |
|                       | Colesterolo           |                       |
|                       |                       |                       |
|                       | Trigliceridi          |                       |
|                       |                       |                       |
|                       | Ossimetria            |                       |
|                       |                       |                       |
|                       | Glicemia a digiuno    |                       |
|                       |                       |                       |
|                       | Emoglobina glicata    |                       |
|                       |                       |                       |
|                       | Temperatura corporea  |                       |
+-----------------------+-----------------------+-----------------------+
| Segni e sintomi       | Segni e sintomi       |                       |
|                       |                       |                       |
|                       | Dolore                |                       |
+-----------------------+-----------------------+-----------------------+
| Contatti con          | Contatti con          | Contatti con          |
| strutture             | strutture medico      | strutture medico      |
|                       | sanitarie             | sanitarie (anche      |
|                       |                       | fuori dal             |
|                       |                       | SSN\ :sup:` [12]_`) o |
|                       |                       | MMG/PLS\ :sup:` [13]_ |
|                       |                       | `                     |
+-----------------------+-----------------------+-----------------------+
| Medicina non          | Contatti con          |                       |
| convenzionale         | strutture di medicina |                       |
|                       | non convenzionale     |                       |
+-----------------------+-----------------------+-----------------------+
| Farmaci e integratori | Assunzione di farmaci | Codice                |
|                       |                       | AIC\ :sup:` [14]_`    |
|                       |                       |                       |
|                       |                       | Descrizione           |
|                       |                       |                       |
|                       |                       | Note (°)              |
+-----------------------+-----------------------+-----------------------+
| Assunzione di altri   | Descrizione           |                       |
| prodotti              |                       |                       |
|                       | Note (°)              |                       |
+-----------------------+-----------------------+-----------------------+

*(°)Il campo Note può contenere data/modalità di assunzione*

Il contenuto del project work intende focalizzarsi sul punto C
dell’elenco sopra riportato, tenuto conto dei seguenti vincoli emersi in
fase di stesura del deliverable da parte del GdL.

In relazione ai requisiti di sicurezza informatica e protezione dei dati
personali richiesti dal contesto normativo, su indicazione del Ministero
della Salute, infatti, il GdL ha ritenuto di escludere per il momento
un’interazione diretta tra dispositivi e piattaforma FSE mediante APP di
mercato, ma che questa debba sempre prevedere il tramite del cittadino,
rilevando in proposito l’utilità, nell’ambito delle interfacce che da
realizzare, di funzionalità di caricamento massivo attivabili on demand
mediante specifiche azioni da parte del cittadino, per agevolare
l’inserimento di valori oggetto di rilevazioni a carattere routinario
(es. misurazione pressione arteriosa).

Fattori politico-economici
-----------------------------

Indirizzo e risorse nazionali
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In ambito politico-economico, si può rilevare come nell’ultimo decennio
uno dei principali obiettivi sia stato il controllo quantitativo e
qualitativo della spesa pubblica anche ai fini del rilancio della
crescita del Paese. A fronte delle difficoltà riscontrate nel perseguire
un percorso di consolidamento dei conti pubblici necessario ai fini del
rispetto degli obiettivi finanziari concordati in sede europea, è emersa
la necessità di potenziare il monitoraggio dei flussi di finanza
pubblica, di effettuare un’analisi puntuale dei meccanismi incidenti
sull'andamento della spesa pubblica e di individuare interventi mirati
al suo contenimento. In questa prospettiva è stato avviato un cosiddetto
programma di "spending review". In questo ambito il decreto legge n.
69/2013 ha dettato inoltre una serie di norme sostanziali riguardanti il
miglioramento della qualità delle procedure di acquisto centralizzato di
beni e servizi, incrementandone significativamente l'utilizzo. E’ stato
così introdotto l'obbligo, da parte di tutte le pubbliche
amministrazioni e delle in-house, di rispettare i parametri
prezzo-qualità dei bandi Consip per le procedure di acquisto di beni e
servizi comparabili, limitando notevolmente la possibilità di
affidamenti.

Indirizzi e risorse regionali
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Al FSE è stato riconosciuto il ruolo di elemento unificante del
patrimonio informativo sanitario di ciascun assistito, alimentato da
ogni contatto tra lo stesso e il SSR, ed “architrave informatica”
abilitante per la realizzazione di servizi digitali ad elevato valore
aggiunto per cittadini ed operatori sanitari. In questa logica, esso
dovrebbe progressivamente assumere un ruolo centrale nel governo del SSR
e della salute e del benessere dei cittadini piemontesi, e gli
interventi individuati per consentirne l’evoluzione e la diffusione sono
compresi nelle principali linee programmatiche riferite alla sanità
digitale.

Essi rientrano nelle iniziative approvate dall’amministrazione regionale
con D.G.R. 19-4900 del 20.4.2017 “[…] «Soluzioni tecnologiche per la
digitalizzazione e l’innovazione dei processi interni dei vari ambiti
della P.A. nel quadro del Sistema pubblico di connettività, quali ad es.
la giustizia, la sanità […]” che ha assegnato risorse a valere sui fondi
comunitari POR-FESR 2014-2020 e con D.G.R. 27-6517 del 23.2.2018 “Linee
di indirizzo della sanità digitale Piemontese – Progetti regionali
2018-2020” nella quale sono previste ulteriori risorse del Fondo
sanitario, in continuità con la “Strategia per la Crescita Digitale
2014-2020” della Presidenza del Consiglio dei Ministri (marzo 2015) che
prevede in Italia lo sviluppo di soluzioni di sanità digitale integrate,
caratterizzate da una forte interazione dei sistemi informativi
sanitari, regionali e delle Aziende Sanitarie e punta ad utilizzare il
digitale come leva di trasformazione economica e sociale.

Tali iniziative sono altresì ricomprese nel “Programma triennale ICT
2019-2021” approvato con D.G.R. 27 dicembre 2018, n. 4-8239.

In particolare l’evoluzione del Taccuino costituisce un intervento
previsto dal Piano di progetto attuativo FSE-SoL\ :sup:` [15]_`
articolato nelle seguenti fasi:

1. l’adeguamento del taccuino piemontese, già disponibile, agli standard
   nazionali di prossima adozione (in corso di realizzazione);

2. la sua evoluzione con ulteriori informazioni rispetto al dataset
   minimo;

3. l’introduzione di sezioni aggiuntive dedicate alle misurazioni da
   realizzarsi individuando, nel rispetto delle norme vigenti. modalità
   in grado di agevolare il cittadino nell’inserimento di dati anche a
   partire da strumenti di uso quotidiano.

Altri fattori
-------------------

Da un punto di vista tecnologico-culturale, vanno considerati due
fattori: da una parte, quasi tutte le fasce di età sono ormai abituate
all’utilizzo di device per la misurazione di parametri vitali per
esigenze di cura, fitness, wellness o come semplici oggetti di moda e,
dall’altra, sul mercato esistono un gran varietà di tipologie di
dispositivi a differenti costi che offrono però soluzioni software
proprietarie per la gestione dei dati generati dall’uso dei device che
poco o per nulla si integrano con sistemi esterni e che raramente
consentono l’esportazione di tali dati.

Se si analizza invece l’ambito sociale, la diffusione di questi
dispositivi e l’inserimento dei dati prodotti sul FSE, ai fini della
consultazione da parte degli operatori sanitari (medici di base,
pediatri e medici specialisti) che hanno in carico il paziente, può
assumere una rilevanza e ricaduta sociale nel momento in cui si rende
possibile, tramite l’analisi e il monitoraggio continuo di parametri
vitali e di misurazioni specifiche, prevenire/rilevare andamenti anomali
e l’insorgenza di malattie, controllare il proprio stile di vita ed
infine aiutare i malati cronici a gestire la propria patologia in modo
più semplice e controllato.

Se si vogliono analizzare infine i fattori fisici che influenzano il
sistema in esame, va considerato di fatto che gli utilizzatori sono
cittadini dislocati sul territorio e, grazie alla realizzazione del
progetto, potrebbero inviare dati rilevati da dispositivi al taccuino
del FSE regionale senza doversi spostare dal luogo in cui risiedono e
ricevere al tempo stesso consigli, alert o feedback dai medici curanti
direttamente sui propri cellulari/tablet o sull’applicazione web del
FSE. A regime, a seguito della diffusione dell’uso del taccuino da parte
del paziente e del FSE da parte del medico, si potrebbero persino
ottimizzare le visite medico-paziente per le situazioni che davvero lo
necessitano diminuendo di fatto anche i fattori stressanti per il
paziente e per il medico e quelli inquinanti nell’ambito urbano.


.. [4]
    HL7 Italia si e' formata nel 2003 come parte di HL7 International ed
   è responsabile della localizzazione dello standard nella realtà
   italiana e, più in generale, ha l'obiettivo di stimolare e
   convogliare i contributi regionali e nazionali allo sviluppo dello
   standard e favorire la modernizzazione del IT sanitario italiano. I
   suoi membri rappresentano dal lato dei fornitori la quota
   maggioritaria del mercato dell'IT sanitario. Sono inoltre membri di
   HL7 Italia alcune Regioni italiane e diverse In-House Regionali,
   Agenzie Governative e Istituti di Ricerca Pubblici oltre ad Aziende
   Sanitarie e singoli professionisti.

.. [5]
    G.U. n.119 del 9/5/2019

.. [6]
   Dalle “Linee guida Agid per l’acquisizione e il riuso software nelle
   PA” si cita: “All’interno di un progetto open source, il maintainer è
   il soggetto che svolge un’attività di controllo e direzione degli
   sviluppi sul progetto, e a cui la community che afferisce al software
   (es: utilizzatori) può segnalare problematiche o discutere
   miglioramenti. Per tutta la durata dell’attività di manutenzione
   connessa al software, l’Amministrazione titolare svolgerà il ruolo di
   maintainer del progetto open source, affidandone l’esecuzione
   all’Incaricato, il quale inserirà il nome della propria azienda o
   ente e i riferimenti di contatto nei file README e publiccode.yml del
   repository, con l’eventuale data di termine dell’incarico.
   L’Incaricato dovrà quindi, per conto dell’Amministrazione, gestire
   l’attività sul progetto derivante dalle interazioni con gli utenti
   esterni.” Pertanto, l’amministrazione Committente del progetto sarà
   Titolare del Software e Maintainer che incarica il CSI-Piemonte come
   software maintainer (esecutore) nell’ambito del progetto open source.

.. [7]
   Include avvenimenti significativi recenti, quali viaggi, vaccinazioni
   non obbligatorie, disturbi del sonno, informazioni sugli stili di
   vita, ecc., il cui inserimento da parte dell’utente sarà guidato
   tramite opportune istruzioni, tutorial ed esempi da predisporre nelle
   interfacce regionali.

.. [8]
    Servizio Sanitario Nazionale

.. [9]
    Medici di Medicina Generale/Pediatri di Libera Scelta

.. [10]
   |  L’Autorizzazione all’Immissione in Commercio (AIC) è definita
     mediante un sistema di codifica che identifica univocamente ogni
     confezione farmaceutica venduta in Italia. Tali codici sono
     rilasciati dall’Agenzia Italiana del Farmaco (AIFA) e permettono
     inoltre di identificare univocamente la confezione farmaceutica
     distinguendola anche in base al numero di compresse/unità, alla
     percentuale di principio attivo, alla via di somministrazione, ecc.
   | (https://www.fascicolosanitario.gov.it/sistemi-codifica-dati/informazioni/aic)

.. [11]
   Include avvenimenti significativi recenti, quali viaggi, vaccinazioni
   non obbligatorie, disturbi del sonno, informazioni sugli stili di
   vita, ecc., il cui inserimento da parte dell’utente sarà guidato
   tramite opportune istruzioni, tutorial ed esempi da predisporre nelle
   interfacce regionali.

.. [12]
    Servizio Sanitario Nazionale

.. [13]
    Medici di Medicina Generale/Pediatri di Libera Scelta

.. [14]
   |  L’Autorizzazione all’Immissione in Commercio (AIC) è definita
     mediante un sistema di codifica che identifica univocamente ogni
     confezione farmaceutica venduta in Italia. Tali codici sono
     rilasciati dall’Agenzia Italiana del Farmaco (AIFA) e permettono
     inoltre di identificare univocamente la confezione farmaceutica
     distinguendola anche in base al numero di compresse/unità, alla
     percentuale di principio attivo, alla via di somministrazione, ecc.
   | (https://www.fascicolosanitario.gov.it/sistemi-codifica-dati/informazioni/aic)

.. [15]
    Approvato con D.D. 544 del 28/11/2018

