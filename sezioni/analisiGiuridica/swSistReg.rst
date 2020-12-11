Software del Sistema Regionale
==================================

Principali tecnologie e librerie
--------------------------------------------

Le principali tecnologie utilizzate per la realizzazione del sistema
regionale sono:

-  linguaggio **JAVA**:

Un linguaggio di programmazione ad alto livello, orientato agli oggetti
e a tipizzazione statica, che si appoggia sull'omonima piattaforma
software di esecuzione, specificamente progettato per essere il più
possibile indipendente dalla piattaforma hardware di esecuzione (tramite
compilazione in bytecode prima e interpretazione poi da parte di una
JVM).

Attualmente esistono per lo sviluppo due tipologie di jdk (java
development kit):

-  Oracle OpenJDK 11: rilasciato con permissive `GPLv2 license agreement and related licenses <http://openjdk.java.net/legal/gplv2+ce.html>`__.

-  Oracle JDK 11: JDK binario rilasciato con `Oracle Technology Network(OTN) License Agreement <https://www.oracle.com/technetwork/java/javase/terms/license/javase-license.html>`__
   per Oracle Java SE. The OTN License permette il download senza
   pagamento di fee per uso in contesti diversi dalla produzione (es:
   dimostrazioni e prototipi, etc).

Questa suddivisione parte dalla jdk 11 e dalle sottoversioni della jdk 8
updates 211.

-  framework **Apache Struts**\ 

un framework open source java della Apache Foundation rilasciato con
licenza **Apache 2.0**\ per lo sviluppo di applicazioni web su
piattaforma Java EE conformi al design pattern MVC (Model View
Controller)

-  framework: **Spring**\ 

un framework open source java rilasciato con licenza **Apache 2.0**
utilizzato per lo sviluppo di componenti di backend con accesso al DBMS.

-  framework java per l’esposizione di servizi XML su protocollo SOAP
   realizzati dalla Apache Foundation e rilasciati con licenza **Apache
   2.0** : **Apache CXF e Apache AXIS.**

-  framework Jboss **restEasy**\ per l’esposizione di RESTful Web
   Services. E’ un’implementazione rilasciata con licenza **Apache 2.0**
   di Jakarta RESTful Web Services, una specifica della Eclipse
   Foundation per Java API di tipo RESTful Web Services over the HTTP
   protocol.\

-  linguaggio SQL per l’accesso al DB per effettuare diverse tipologie
   di operazioni:

   -  DDL (Data Definition Language): consente di creare e modificare
      schemi di database;\

   -  DML (Data Manipulation Language): consente di inserire, modificare
      e gestire i dati memorizzati;

   -  DQL (Data Query Language): consente di interrogare i dati
      memorizzati

-  linguaggio PL/pgSQL specifico per realizzare store procedure

-  linguaggi per la generazione delle interfacce utente delle web
   application fruibili da web browser

l'HyperText Markup Language è un linguaggio di markup utilizzato
principalmente per il disaccoppiamento della struttura logica di una
pagina web (definita appunto dal markup) e la sua rappresentazione,
gestita tramite gli stili CSS.\

L'HTML è un **linguaggio di pubblico dominio**, la cui sintassi è
stabilita dal World Wide Web Consortium (W3C). La versione attuale è la
5 rilasciata nell'ottobre 2014, nata per fornire direttamente le
funzionalità che in precedenza erano fruibili tramite estensioni
proprietarie all'esterno dei browser (come Adobe Flash e simili) e per
garantire una maggiore compatibilità tra i diversi browser,
indipendentemente dalla piattaforma software utilizzata, e
principalmente mirata all'espansione dei dispositivi mobili.

Considerazioni sulla pubblicazione del software del sistema regionale
del FSE

Il sistema regionale del FSE è basato su software sviluppato fin dal
2010.

Per arrivare alla pubblicazione del codice sorgente in open source, in
conformità all’art. 69 del CAD, va svolta un’analisi accurata al fine di
poterne valutare la fattibilità (pubblicabilità del software) e per
poter scegliere la licenza più adatta in relazione alla tipologia delle
componenti software presenti (es: frontend, backend, web service, etc).

Pur scegliendo come strategia iniziale quella di seguire le indicazioni
in termini di licenze secondo le linee guida AgID, in base ai risultati
ottenuti, in termini di compatibilità di licenze, dalla verifiche
tecniche e legali effettuabili sul software, diventa poi necessario
individuare la migliore licenza per rendere comunque il prodotto
software disponibile con una licenza comunque “aperta” secondo l’OSI
Definition https://opensource.org/osd, con modalità compatibili con i
profili tecnici e giuridici individuati nell’analisi del software. In
caso di incompatibilità di licenze, potranno essere considerate, a
titolo di esempio, alternative quali:

-  rilascio separato di singoli moduli dell’applicativo identificabili
   come opere dotate di autonomia;

-  sostituzione (con i relativi costi) dell’elemento interno
   eventualmente causa di incompatibilità (ad esempio, mediante la
   sostituzione di una libreria);

-  in extremis scelta di altra licenza, ove possibile, compatibile con
   quelle causanti incompatibilità con la licenza iniziale prevista.

Di seguito vengono riportati le attività previste nel processo per la
pubblicabilità del software in open source del CSI-Piemonte, in qualità
di software maintainer del prodotto FSE :

-  **produzione del BOM (Bill Of Materials),**\ documento in cui sono
   elencati tutti i software di terze parti (per lo più librerie e
   framework) utilizzati internamente al software oggetto di
   pubblicazione e relative licenze associate, proprietarie o open
   source. Tale elenco può essere prodotto utilizzando strumenti
   software denominati\ **source code scan tool** (ad esempio OWASP
   dependency check, sonatype).

-  **verifiche tecniche**\ della scrittura del codice sorgente e
   propedeutiche alla pubblicazione su repository pubblico e **verifiche
   legali**\ volte alla verifica della **compatibilità delle licenze
   delle librerie di terze parti** utilizzate dal software, dando
   eventualmente l'indicazione di sostituzione di librerie in quanto non
   compatibili con le altre licenze open source scelte. Maggiori
   dettagli sul tipo di verifiche da effettuare vengono riportate nei
   paragrafi successivi.

**NOTA:**\ Qualora l’esito della verifica di pubblicabilità risulti
negativo a seguito delle verifiche tecnico-legali e sia necessaria una
modifica al codice del prodotto, si prevede la formulazione di una
**valutazione tecnica ed economica della revisione software e
documentale** per risolvere i problemi che non permettono la
pubblicabilità del software as-is e la **ricerca delle relativa fonte di
finanziamento**. A seguito di tali attività viene determinato se
sospendere, temporaneamente o definitivamente, la pubblicazione del
prodotto software o se proseguire con gli interventi di modifica del
codice e/o della documentazione.

-  **indicazione della Licenza Open Source** al superamento delle
   verifiche tecnico-legali,con cui verrà pubblicato il software e la
   documentazione.

-  **Individuazione del raggruppamento dei repository e del/i repository
   di pubblicazione del prodotto sw**. In generale, i criteri utilizzati
   per determinare il repository in cui salvare il codice sono:

   -  l'organizzazione detentrice della proprietà intellettuale del
      prodotto;

   -  la scomposizione del prodotto in repository diversi;

-  **Creazione team e assegnazione abilitazioni**. Una volta creato il
   repository si crea il **team admin** del prodotto al quale viene
   associato il solo Gestore del Repository e gli eventuali **team di
   sviluppo** del prodotto (ad esempio il team collaboratori interni al
   progetto con permessi di write). Ad ogni team vengono assegnate le
   abilitazioni/permessi in funzione del ruolo.

-  **Pubblicazione del codice sorgente**. Il Gestore del Repository a
   questo punto procede con la pubblicazione su repository del codice
   sorgente e di tutta la documentazione prodotta. Per la pubblicazione
   anche su Developers Italia è necessaria la presenza del file
   *publiccode.yml*\ e dei relativi file accessori.

Verifiche legali
~~~~~~~~~~~~~~~~~~~~~~~~~

Le verifiche legali vengono effettuate da un esperto legale in ambito
open source e software sulla base del BOM prodotto dal responsabile
tecnico del progetto software.

Il BOM è, in questa verifica, lo strumento di base per:

-  la valutazione della pubblicabilità del software con licenza open
   source

-  individuare la licenza open source più adatta con cui licenziare
   l’intera opera.

Le verifiche legali vertono sull’analisi di due aspetti:

-  compatibilità con il rilascio in open source delle licenze delle
   librerie SW utilizzate internamente come link statici` [48]_`
   del codice

-  compatibilità con il rilascio in open source rispetto all'uso di link
   dinamici` [49]_` (es. Google web API)

-  compatibilità con il rilascio in open source rispetto
   all’incorporamento di software di terzi` [50]_`

Verifiche tecniche della scrittura del codice sorgente
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Si propone di seguito una possibile **checklist di verifiche in uso
presso il CSI-Piemonte**

+-----------------+-----------------+-----------------+-----------------+
| **Elementi da   | **Effettuata**  | **Esito**       | **Note in       |
| verificare**    |                 |                 | merito          |
|                 |                 |                 | all'esito**     |
+-----------------+-----------------+-----------------+-----------------+
| Verifica della  |                 |                 |                 |
| presenza di     |                 |                 |                 |
| tutti i file    |                 |                 |                 |
| utili ad        |                 |                 |                 |
| effettuare il   |                 |                 |                 |
| build del       |                 |                 |                 |
| prodotto        |                 |                 |                 |
| software        |                 |                 |                 |
| (laddove        |                 |                 |                 |
| previsto).      |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica        |                 |                 |                 |
| presenza di     |                 |                 |                 |
| riferimenti a   |                 |                 |                 |
| server e/o      |                 |                 |                 |
| informazioni    |                 |                 |                 |
| dell'infrastrut |                 |                 |                 |
| tura            |                 |                 |                 |
| CSI             |                 |                 |                 |
| internamente al |                 |                 |                 |
| codice o in     |                 |                 |                 |
| file di         |                 |                 |                 |
| properties      |                 |                 |                 |
| specifici, con  |                 |                 |                 |
| particolare     |                 |                 |                 |
| attenzione agli |                 |                 |                 |
| aspetti di      |                 |                 |                 |
| sicurezza       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica che    |                 |                 |                 |
| non siano       |                 |                 |                 |
| presenti        |                 |                 |                 |
| informazioni    |                 |                 |                 |
| relative a      |                 |                 |                 |
| credenziali     |                 |                 |                 |
| applicative o   |                 |                 |                 |
| infrastruttural |                 |                 |                 |
| i               |                 |                 |                 |
| utili al        |                 |                 |                 |
| funzionamento   |                 |                 |                 |
| del prodotto in |                 |                 |                 |
| ambiente CSI    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica che i  |                 |                 |                 |
| servizi web     |                 |                 |                 |
| (SOAP o REST)   |                 |                 |                 |
| acceduti a      |                 |                 |                 |
| runtime dal     |                 |                 |                 |
| software non    |                 |                 |                 |
| abbiano         |                 |                 |                 |
| esplicitato     |                 |                 |                 |
| l'end-point ma  |                 |                 |                 |
| siano presenti  |                 |                 |                 |
| dei placeholder |                 |                 |                 |
| che ne          |                 |                 |                 |
| indichino la    |                 |                 |                 |
| necessità di    |                 |                 |                 |
| sostituzione in |                 |                 |                 |
| fase di         |                 |                 |                 |
| runtime.        |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica che    |                 |                 |                 |
| eventuali       |                 |                 |                 |
| riferimenti a   |                 |                 |                 |
| chiamate RPC    |                 |                 |                 |
| (non Web        |                 |                 |                 |
| Service) a      |                 |                 |                 |
| servizi         |                 |                 |                 |
| esterni, nel    |                 |                 |                 |
| codice o nei    |                 |                 |                 |
| file di         |                 |                 |                 |
| properties,     |                 |                 |                 |
| siano generici  |                 |                 |                 |
| (nessun         |                 |                 |                 |
| riferimento a   |                 |                 |                 |
| server reali)   |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica che    |                 |                 |                 |
| nel caso di     |                 |                 |                 |
| dipendenze da   |                 |                 |                 |
| servizi non     |                 |                 |                 |
| pubblicabili su |                 |                 |                 |
| repertorio      |                 |                 |                 |
| pubblico        |                 |                 |                 |
| vengano         |                 |                 |                 |
| descritte e     |                 |                 |                 |
| documentate le  |                 |                 |                 |
| interfacce di   |                 |                 |                 |
| colloquio con   |                 |                 |                 |
| servizio fruito |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica che le |                 |                 |                 |
| firme dei       |                 |                 |                 |
| servizi web     |                 |                 |                 |
| esposti dal     |                 |                 |                 |
| software (sia   |                 |                 |                 |
| per uso interno |                 |                 |                 |
| che per uso     |                 |                 |                 |
| esterno) siano  |                 |                 |                 |
| dichiarate e    |                 |                 |                 |
| documentate.    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica della  |                 |                 |                 |
| qualità del     |                 |                 |                 |
| software        |                 |                 |                 |
| tramite         |                 |                 |                 |
| strumenti       |                 |                 |                 |
| automatici (es. |                 |                 |                 |
| **SonarQube**)  |                 |                 |                 |
| e conseguenti   |                 |                 |                 |
| interventi di   |                 |                 |                 |
| revisione​       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Revisione       |                 |                 |                 |
| totale dei      |                 |                 |                 |
| commenti        |                 |                 |                 |
| interni al      |                 |                 |                 |
| codice sorgente |                 |                 |                 |
| sia nel         |                 |                 |                 |
| rispetto        |                 |                 |                 |
| del\ **Code Of  |                 |                 |                 |
| Conduct**\ sele |                 |                 |                 |
| zionato         |                 |                 |                 |
| durante la fase |                 |                 |                 |
| iniziale sia    |                 |                 |                 |
| per la          |                 |                 |                 |
| leggibilità da  |                 |                 |                 |
| parte dei       |                 |                 |                 |
| soggetti        |                 |                 |                 |
| interessati.​    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Ricompilazione  |                 |                 |                 |
| del software,   |                 |                 |                 |
| test e deploy   |                 |                 |                 |
| per poter       |                 |                 |                 |
| effettuare la   |                 |                 |                 |
| verifica        |                 |                 |                 |
| funzionale di   |                 |                 |                 |
| coerenza tra il |                 |                 |                 |
| software già    |                 |                 |                 |
| rilasciato a    |                 |                 |                 |
| servizio e      |                 |                 |                 |
| quello          |                 |                 |                 |
| "revisionato"   |                 |                 |                 |
| (nel caso di    |                 |                 |                 |
| intervento di   |                 |                 |                 |
| modifica).      |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Sono state      |                 |                 |                 |
| effettuate le   |                 |                 |                 |
| verifiche di    |                 |                 |                 |
| vulnerabilità   |                 |                 |                 |
| del software    |                 |                 |                 |
| tramite gli     |                 |                 |                 |
| strumenti messi |                 |                 |                 |
| a disposizione  |                 |                 |                 |
| dall’azienda    |                 |                 |                 |
| (es. **IBM      |                 |                 |                 |
| Appscan**\ per  |                 |                 |                 |
| verifiche       |                 |                 |                 |
| statiche e      |                 |                 |                 |
| dinamiche) e    |                 |                 |                 |
| sono state      |                 |                 |                 |
| valutate le     |                 |                 |                 |
| conseguenze ed  |                 |                 |                 |
| i rischi a      |                 |                 |                 |
| seguito della   |                 |                 |                 |
| pubblicazione.  |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Sono stati      |                 |                 |                 |
| eseguiti i test |                 |                 |                 |
| di carico e gli |                 |                 |                 |
| stress test e   |                 |                 |                 |
| si è provveduto |                 |                 |                 |
| alla            |                 |                 |                 |
| predisposizione |                 |                 |                 |
| della           |                 |                 |                 |
| documentazione  |                 |                 |                 |
| per la          |                 |                 |                 |
| pubblicazione   |                 |                 |                 |
| dei risultati.  |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica della  |                 |                 |                 |
| assenza di dati |                 |                 |                 |
| sensibili       |                 |                 |                 |
| inseriti nei    |                 |                 |                 |
| file del        |                 |                 |                 |
| sorgente,       |                 |                 |                 |
| inseriti anche  |                 |                 |                 |
| solo al fine di |                 |                 |                 |
| effettuare test |                 |                 |                 |
| automatici​      |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Nel caso siano  |                 |                 |                 |
| gestiti con     |                 |                 |                 |
| software dei    |                 |                 |                 |
| dati sensibili  |                 |                 |                 |
| si è            |                 |                 |                 |
| documentata la  |                 |                 |                 |
| modalità di     |                 |                 |                 |
| gestione del    |                 |                 |                 |
| dato (cifratura |                 |                 |                 |
| lato DB o       |                 |                 |                 |
| software,       |                 |                 |                 |
| etc…). In caso  |                 |                 |                 |
| di presenza di  |                 |                 |                 |
| gestione di     |                 |                 |                 |
| dati sensibili, |                 |                 |                 |
| è obbligatorio  |                 |                 |                 |
| pubblicare      |                 |                 |                 |
| documenti       |                 |                 |                 |
| relativi alla   |                 |                 |                 |
| gestione del    |                 |                 |                 |
| dato stesso.    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| *Valutazione    |                 |                 |                 |
| :*\ traduzione  |                 |                 |                 |
| del testo della |                 |                 |                 |
| documentazione  |                 |                 |                 |
| in lingua       |                 |                 |                 |
| inglese​         |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Sono presenti o |                 |                 |                 |
| sono stati      |                 |                 |                 |
| realizzati gli  |                 |                 |                 |
| script di       |                 |                 |                 |
| installazione e |                 |                 |                 |
| configurazione  |                 |                 |                 |
| o sono stati    |                 |                 |                 |
| messi a         |                 |                 |                 |
| disposizione    |                 |                 |                 |
| dei container   |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Sono presenti o |                 |                 |                 |
| sono stati      |                 |                 |                 |
| realizzati      |                 |                 |                 |
| degli script    |                 |                 |                 |
| per             |                 |                 |                 |
| l'esecuzione di |                 |                 |                 |
| test automatici |                 |                 |                 |
| a seguito della |                 |                 |                 |
| installazione   |                 |                 |                 |
| del software su |                 |                 |                 |
| nuovi ambienti. |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Pubblicazione   |                 |                 |                 |
| su GitLab       |                 |                 |                 |
| interno (se già |                 |                 |                 |
| adottato) e     |                 |                 |                 |
| collegamento    |                 |                 |                 |
| con GitHub per  |                 |                 |                 |
| la              |                 |                 |                 |
| riconciliazione |                 |                 |                 |
| periodica delle |                 |                 |                 |
| release​.        |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Eliminazione    |                 |                 |                 |
| dei file        |                 |                 |                 |
| sorgenti non    |                 |                 |                 |
| utilizzati​      |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Eliminazione    |                 |                 |                 |
| delle librerie  |                 |                 |                 |
| di terze parti  |                 |                 |                 |
| non utilizzate  |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica        |                 |                 |                 |
| presenza del    |                 |                 |                 |
| documento di    |                 |                 |                 |
| manuale utente  |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Verifica        |                 |                 |                 |
| presenza        |                 |                 |                 |
| laddove utile   |                 |                 |                 |
| (o necessario)  |                 |                 |                 |
| della           |                 |                 |                 |
| descrizione     |                 |                 |                 |
| dell’hardware   |                 |                 |                 |
| minimo          |                 |                 |                 |
| occorrente per  |                 |                 |                 |
| il corretto     |                 |                 |                 |
| funzionamento   |                 |                 |                 |
| delle           |                 |                 |                 |
| componenti      |                 |                 |                 |
| software.       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

Verifiche tecniche propedeutiche alla pubblicazione su repository pubblico
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Si propone di seguito una possibile **checklist di verifiche in uso
presso il CSI-Piemonte**:

+-----------------+-----------------+-----------------+-----------------+
| **Elementi da   | **Effettuata**  | **Esito**       | **Note/Osservaz |
| verificare**    |                 |                 | ioni            |
|                 |                 |                 | in merito       |
|                 |                 |                 | all'esito**     |
+-----------------+-----------------+-----------------+-----------------+
| E' presente     |                 |                 |                 |
| l'organization  |                 |                 |                 |
| GitHub (o altra |                 |                 |                 |
| piattaforma     |                 |                 |                 |
| code hosting)   |                 |                 |                 |
| sotto cui       |                 |                 |                 |
| effettuare la   |                 |                 |                 |
| pubblicazione   |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Sono presenti   |                 |                 |                 |
| sotto           |                 |                 |                 |
| l'organization  |                 |                 |                 |
| GitHub (o altra |                 |                 |                 |
| piattaforma     |                 |                 |                 |
| code hosting) i |                 |                 |                 |
| repository      |                 |                 |                 |
| sotto cui       |                 |                 |                 |
| effettuare la   |                 |                 |                 |
| pubblicazione   |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Le utenze       |                 |                 |                 |
| GitHub (create  |                 |                 |                 |
| secondo quanto  |                 |                 |                 |
| previsto dalle  |                 |                 |                 |
| specifiche      |                 |                 |                 |
| )sono state     |                 |                 |                 |
| abilitate alla  |                 |                 |                 |
| pubblicazione   |                 |                 |                 |
| sui repository  |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| È presente il   |                 |                 |                 |
| file README.md  |                 |                 |                 |
| sotto il        |                 |                 |                 |
| repository del  |                 |                 |                 |
| prodotto        |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| È descritta nel |                 |                 |                 |
| file README.md  |                 |                 |                 |
| l'architettura  |                 |                 |                 |
| del software    |                 |                 |                 |
| utile a         |                 |                 |                 |
| comprenderne    |                 |                 |                 |
| l'articolazione |                 |                 |                 |
| in componenti e |                 |                 |                 |
| le dipendenze   |                 |                 |                 |
| con system      |                 |                 |                 |
| software di     |                 |                 |                 |
| terze parti.    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| È presente il   |                 |                 |                 |
| file            |                 |                 |                 |
| LICENSE.txt     |                 |                 |                 |
| sotto il        |                 |                 |                 |
| repository del  |                 |                 |                 |
| prodotto        |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Nel file        |                 |                 |                 |
| LICENSE.txt     |                 |                 |                 |
| sono riportati  |                 |                 |                 |
| tutti i testi   |                 |                 |                 |
| delle licenze   |                 |                 |                 |
| indicate nelle  |                 |                 |                 |
| componenti di   |                 |                 |                 |
| terze parti     |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| È presente il   |                 |                 |                 |
| file            |                 |                 |                 |
| CHANGELOG.md o  |                 |                 |                 |
| RELEASENOTES.md |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| È presente il   |                 |                 |                 |
| file            |                 |                 |                 |
| COPYRIGHT.txt o |                 |                 |                 |
| è indicato il   |                 |                 |                 |
| Copyright nel   |                 |                 |                 |
| README.md       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| È presente il   |                 |                 |                 |
| file BOM.csv    |                 |                 |                 |
| e/o il          |                 |                 |                 |
| MANIFEST.txt in |                 |                 |                 |
| ogni repository |                 |                 |                 |
| del prodotto    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| È presente il   |                 |                 |                 |
| file            |                 |                 |                 |
| publiccode.yml  |                 |                 |                 |
| (e ne è stata   |                 |                 |                 |
| verificata la   |                 |                 |                 |
| validità) nel   |                 |                 |                 |
| repository      |                 |                 |                 |
| principale del  |                 |                 |                 |
| prodotto        |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| E' stato        |                 |                 |                 |
| inserito        |                 |                 |                 |
| l’Header con    |                 |                 |                 |
| indicazione     |                 |                 |                 |
| della licenza   |                 |                 |                 |
| scelta e del    |                 |                 |                 |
| copyright       |                 |                 |                 |
| corretto in     |                 |                 |                 |
| tutti i file    |                 |                 |                 |
| sorgente​       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

.. [48] link statico: si riferisce ad una libreria software che nel proprio prodotto viene collegata staticamente in fase di compilazione

.. [49] link dinamico: si riferisce ad una libreria software che nel proprio prodotto viene caricata dinamicamente in fase di esecuzione

.. [50] incorporamento: inserimento di porzioni di codice di terze parti all’interno del proprio prodotto software