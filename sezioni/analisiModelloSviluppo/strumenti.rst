Strumenti per la gestione della community
=============================================

In questo capitolo vengono analizzati i tool utili alla promozione della
Community e all’interazione fra i membri della Community stessa.

Nella mappa mentale sotto riportata, vengono indicati i vari strumenti
che saranno analizzati più in dettaglio nei capitoli successivi.

.. |image39| figure:: /immagini/1000020100000537000001B7495BA7821FA4B733.png
   :scale: 60 % 
   :alt: Mappa dei processi del Community OS

   Mappa dei processi del Community OS

In considerazione delle specificità di ognuno risulta evidente fin da
subito che è necessario al software maintainer *impegnare delle risorse*
per:

-  la predisposizione e la configurazione *una tantum* degli strumenti

-  la gestione *in itinere* in funzione delle varie fasi della roadmap
   di progetto e della “vivacità della Community che si viene a creare.

Si può inoltre ipotizzare di rendere disponibili gli strumenti di
collaboration in un momento successivo rispetto agli altri ovvero quando
la Community viene promossa e diventa più numerosa.

Sito della Community
--------------------------

L’obiettivo di un sito della Community del progetto Taccuino è quello di
avere una vetrina online per

-  spiegare il progetto e comunicare come viene portato avanti dalla
   Community

-  far crescere una community intorno al progetto

-  fare "pubblicità" all’iniziativa progettuale e alla Community stessa.

Il sito è indirizzato sia agli **utenti esterni** alla Community per

-  conoscere le caratteristiche del progetto, la sua *roadmap*\ e le sue
   finalità,

-  trovare informazioni su come scaricare e utilizzare il software
   prodotto nell’ambito del progetto,

-  trovare supporto all’utilizzo

sia agli **utenti interni**\ alla Community per trovare un unico punto
di accesso

-  alla documentazione del prodotto software

-  agli strumenti di sviluppo del codice e di redazione della
   documentazione a corredo

-  alle informazioni più tecniche come ad esempio:

   -  la descrizione delle API del back-end applicativo del Taccuino

   -  le modalità di utilizzo per i test di integrazione.

   -  il workflow pubblico che descrive come interagire con il progetto
      (comprensivo di esempi, modelli, etc)

Il sito può contenere una sezione con documenti scritti su GitHub in
formato .rst  [31]_ e visualizzati in modalità renderizzata html
sul sito, ad esempio attraverso l’uso di
`Sphinx <http://sphinx-doc.org/>` [32]_ con un
`theme <https://github.com/rtfd/sphinx_rtd_theme>`  fornito da `Read the Docs <https://readthedocs.org/>`  [33]_.

La scrittura su GitHub consente di usufruire del *sistema di versioning*
e degli strumenti di gestione di *pull requests* e di\ *issues* presenti
nella piattaforma.

Con questa modalità di gestione della documentazione, i documenti
vengono scritti in un formato testuale molte semplice (restructuredText
ovvero file .rst) e consultati in formato HTML con un *layout
responsive* che ben si adatta alla visualizzazione su *desktop o
dispositivi mobile*. La lettura via web e l’impaginazione risultano
pertanto facili ed intuitivi.

Repository pubblico
----------------------

Per la pubblicazione di un nuovo prodotto SW, come può essere la app
regionale del Taccuino, su repository pubblico realizzato con fondi
pubblici e di proprietà della pubblica amministrazione (ex. Art.69 CAD)
devono essere redatti i documenti descritti nel presente capitolo.

I documenti di seguito indicati sono intesi come documenti utili alla
comprensione del prodotto software (quindi i cosiddetti “\ **documenti
di prodotto**\ ”) mentre non sono inclusi i documenti utilizzati con la
finalità di realizzare il prodotto software (i cosiddetti “\ **documenti
di progetto**\ ”, come ad esempio la “Vista di Insieme”, l’architettura
di Deployment, le Specifiche del sistema, l’elenco dei Casi d’uso, etc…)
che possono invece essere eventualmente forniti con diverse modalità e
finalità.

Il formato dei documenti pubblicati su repository pubblico è di tipo
solo testo. Si predilige il formato **Markdown (md)**. Markdown è una
sintassi per la formattazione di testo puro, progettata in modo che
possa essere convertito in HTML utilizzando un semplice script.
Attualmente è comunemente usato come formato per file readme, per la
formattazione di messaggi nei forum o in editor di testo per la
creazione rapida di documenti di testo formattati e in molti CMS di uso
comune. Le semplicità estrema della sintassi fa sì che chiunque, anche
senza esperienza di programmazione, possa in pochissimo tempo cominciare
a scrivere documenti senza l’ausilio di guide o software particolare, ma
semplicemente di un editor di testo, spesso gli stessi utilizzati dagli
sviluppatori per i file del codice sorgente. Ambienti molto minimali
permettono la creazione di documenti relativamente complessi senza
l’ausilio di nessuna interfaccia grafica, ma semplicemente tramite
emacs, gedit o vim, per i quali esistono plugin per la syntax
highlighting di Markdown, o **Atom**, il text editor modulare presentato
da GitHub.\ ` <https://serverimg2.polito.it:9443/s/GX6yM7xNkYWmNyt#>`__

Il prodotto software, pubblicato con licenza open source su
**github.com,** dovrà essere presente internamente all’ **organization
di riferimento**\ ovvero quella relativa all’organizzazione/ente
proprietario del software.

Nel caso del FSE e del Taccuino è pertanto la **Regione
Piemonte**\ *\ (url di riferimento
dell’organization*\ https://github.com/regione-piemonte\ *).*

.. |image40| figure:: /immagini/10000201000005F6000003E7C1381834E73D0DAE.png
   :scale: 50 % 
   :alt: GitHub - Organization Regione Piemonte

   GitHub - Organization Regione Piemonte

Il prodotto software deve prevedere una sottostruttura a repository e
directory che segue le regole:

-  Il **repository principale del prodotto**, ossia denominato con il
   nome del prodotto stesso. Questo repository conterrà tutta la
   documentazione del prodotto, i principali sorgenti per eseguire
   installazioni e configurazioni. Viene descritta la scomposizione del
   prodotto nei vari componenti nel file *publiccode.yml*. Questo
   repository diventa il repository di cui effettuare il
   “pin” [34]_ per la reperibilità del prodotto stesso sulla
   pagina dell’organization.

-  I **repository per ogni componente di prodotto autonoma**, che assume
   una propria valenza a livello di prodotto e che potrebbe essa stessa
   essere di interesse per eventuali “fork” di terzi. In linea di
   massima ogni qual volta si definisca l’architettura di un software e
   la sua scomposizione in moduli o componenti, il codice sorgente dei
   moduli implementati sarò contenuto nei repository creati per ogni
   componente.

-  Le **directory**\ sottostanti i diversi repository sono a supporto
   dell'organizzazione del prodotto, quindi la struttura annidata è
   funzionale alla comprensione del software. Le directory interne al
   repository principale possono contenere sorgenti utili alla struttura
   del prodotto e non già contenuti nei repository delle componenti.

**Si potrebbe prevedere pertanto un prodotto taccuino con due
componenti: app iOS e app Android**

La documentazione indicata di seguito è individuata da CSI attraverso
l’analisi di quanto pubblicato e disponibile sui repository pubblici di
molti prodotti open source, da quanto indicato nelle linee guida di
AgID [35]_ e da quanto già estratto dall’analisi della
documentazione di prodotti esterni:

-  **publiccode.yml:** è il descrittore del prodotto o della componente
   di prodotto per la pubblicazione su Developers Italia. Se presente a
   livello di prodotto non necessita di essere anche definito a livello
   di singola componente.

-  **License.txt:** per ogni componente del prodotto SW indicare la
   licenza associata a tutti i file (verrà comunque indicato nell’header
   di ogni file il riferimento alla licenza adottata in formato
   SPDX [36]_). Se necessario si deve prevedere l’indicazione
   di clausole aggiuntive a licenze standard (per standard si intendono
   quelle indicate nella lista spdx.org).

-  **Readme.md**: a livello di prodotto ed a livello di singola
   componente si richiede di scrivere un file Readme.md che descriva gli
   elementi significativi del software, rispettando il più possibile i
   capitoli del template specifico.

-  **Contributing.txt**: descrive le modalità operative con cui un
   contributor può relazionarsi con il maintainer così da rilasciare
   nuove proposte di modifiche o integrazioni.

-  **CodeOfConduct.md**: descrive le modalità, i comportamenti che un
   programmatore intenzionato a contribuire allo sviluppo del codice
   deve seguire ed a cui si deve attenere. Si può fare riferimento ad un
   testo standard scelto dall’azienda.

-  **Bom.csv:** è il Bill Of Materials, ovvero l’elenco di tutti i
   packages esterni utilizzati dal prodotto (o da ogni sua singola
   componente). Per completezza si segnala che un sottoprodotto del Bom,
   utilizzabile per fini di automazione dell’installazione è il
   Manifest.txt, che comprende l’elenco di tutte le librerie esterne
   usate con la sola indicazione del nome e della versione. Il Manifest
   deve essere inteso come opzionale e comunque accessorio rispetto al
   BOM;

-  **Manifest.txt**, che comprende l’elenco di tutte le librerie esterne
   usate con la sola indicazione del nome e della versione.

-  **Contributors.txt:** Elenco di enti pubblici o aziende che hanno
   contribuito a vario titolo allo sviluppo del software.

-  **Authors.txt:** il file Authors conterrà i nomi di persone (e
   eventualmente delle aziende di appartenenza) che nel tempo hanno
   contribuito alla realizzazione del prodotto software. Si richiede di
   mantenere un file Authors a livello di progetto (root) o tanti file
   Authors a livello di componente di prodotto. E’ meglio evitare di
   avere un file authors a livello di prodotto e contemporaneamente
   tanti authors a livello di componente.

-  **Release_Notes.md/ Changelog.md:** per ogni componente indicare le
   variazioni della versione X.X.X rilasciata rispetto alla precedente
   (aggiungendo quindi le info sullo stesso file), con indicazione delle
   correzioni di bugs, aggiunta di nuove funzionalità, bugs conosciuti,
   ecc… Un changelog è un file che contiene una lista curata e ordinata
   cronologicamente delle modifiche degne di nota per ogni versione di
   un prodotto.

-  **Maintainers.txt:** lista delle Aziende e modalità con cui viene
   mantenuto il codice (opzionale).

-  **Copyrights.txt:** indica chi è il detentore dei diritti d’autore.

-  **ThirdPartyNote.txt:** è l’elenco di tutti i software di terze
   parti utilizzati nel o dal software pubblicato. Tutta la
   documentazione aggiuntiva rispetto a quanto qui indicato può essere
   utilizzata eventualmente in caso di richiesta o necessità espressa da
   altri soggetti esterni, nel caso fosse ritenuto strategicamente
   perseguibile condividere la documentazione e la conoscenza.

Di seguito viene riportata una tabella che sintetizza l'obbligatorietà o
meno di ognuno di questi file.

.. |image40| figure:: /immagini/file.jpg
   :scale: 80 % 
   :alt: GitHub - file principali

   GitHub - file principali



Strumenti di interazione per gli utenti della Community
-----------------------------------------------------------



Gestione degli issue
~~~~~~~~~~~~~~~~~~~~~~~

Per ogni repository presente sotto un’organizzazione di GitHub è
possibile contribuire inserendo **issue**\ al fine di sottoporre
differenti tipologie di richieste come ad esempio:

-  *Bug report*

-  *Feature request*

-  *General issue.*

Le segnalazioni inerenti vulnerabilità o bug relative alla sicurezza del
software, in considerazione della delicatezza del tema trattato, vengono
trattate in modo differente come descritto al capitolo `Gestione delle segnalazioni inerenti la sicurezza software e vulnerability <#_5gu151hbbsiw>`__.

Di seguito viene riportato un esempio di repository di Developers Italia

.. |image41| figure:: /immagini/1000020100000305000001E6A86C6F95D0BA799E.png
   :scale: 50 % 
   :alt: Esempio di repository di Developers Italia

   Esempio di repository di Developers Italia

Le issue vengono inseriti e gestite con funzionalità apposite della
piattaforma.

Di seguito viene mostrato un esempio su un repository di prova.

.. |image42| figure:: /immagini/100002010000040A000003091A61995D8B0B0B22.png
   :scale: 50 % 
   :alt:  Repository di prova

    Repository di prova

Nel testo della issue si può utilizzare il linguaggio di `markdown <https://guides.github.com/features/mastering-markdown/>`__.

Per personalizzare e standardizzare le informazioni inserite in una
nuova issue è possibile inoltre configurare GitHub inserendo un file
**config.yml** sotto la directory **.github/ISSUE_TEMPLATE** del
repository. In questo modo è possibile ad esempio, obbligare l’utente a
specificare la tipologia di issue secondo le tre tipologie riportate in
precedenza.

Ad ogni issue può essere associato:

-  *un o più assegnatario*

-  *una o più labels (una sorta di tag) inserite dal software maintainer
   o inserite in autonomia dall’utente esterno*

-  *un progetto di riferimento*

-  *una milestone di riferimento*

-  *la relativa pull request.*

Per quanto riguarda i **progetti** su GitHub, interessante è la sezione
della piattaforma dove è possibile definire un progetto e gestirne la
pianificazione e il monitoraggio/controllo attraverso la scelta di
template legati alla metodologia **Agile** riportati di seguito:


.. |image43| figure:: /immagini/10000201000001010000017E093E3FC1DC131E33.png
   :scale: 50 % 
   :alt: Tipologie di Project Board

   Tipologie di Project Board
   
.. |image44| figure:: /immagini/10000201000003790000019481AEB168D672B44D.png
   :scale: 50 % 
   :alt: Esempio di Project Board

   Esempio di Project Board

Per **ricerca gli issue** è disponibile un form di ricerca testuale con
vari filtri relativi ai metadati correlati al issue (stato,
assegnatario, autore, label, milestone, progetto, …)


.. |image45| figure:: /immagini/10000201000003CA000001BBC0F603CB35257D44.png
   :scale: 50 % 
   :alt: Esempio di ricerca di issue

   Esempio di ricerca di issue

Le **modalità di auto-contribuzione** vengono espresse nei seguenti
file:

-  *Contributing.txt:* linee guida sul modo con cui contribuire (un esempio interesante è quello proposto da `developers.italia.it <https://github.com/italia/developers.italia.it/blob/master/CONTRIBUTING.md>`__)

-  *CodeOfConduct.md: documento che*\ definisce gli standard su come
   impegnarsi in una Community. Ha l’obiettivo di promuovere un ambiente
   inclusivo che rispetta tutti i contributi. Descrive inoltre le
   procedure per affrontare i problemi che possono sorgere tra i membri
   della community stessa. Alcuni esempi si possono trovare nei seguenti
   link `Open Source Guide <https://opensource.guide/code-of-conduct/>`__ e `GitHub Community <https://docs.github.com/en/github/site-policy/github-community-guidelines>`_.



Gestione delle pull request
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Inserire una pull request significa contribuire alla modifica del
software presente all’interno di un repository GitHub, che usa il
sistema di controllo di versione `Git <https://datasift.github.io/gitflow/IntroducingGitFlow.html>`__.

.. |image46| figure:: /immagini/10000201000001EE000002CDED689EF19359D93D.png
   :scale: 50 % 
   :alt: GitFlow

   GitFlow

In figura è riportato un esempio di linee di codice utilizzate su un
software in cui nel tempo vengono gestite tre release opportunamente
identificate da **tag**\ per consentire bug fixing urgenti (hot fix) ed
evolutive con nuove funzionalità. Le modifiche possono essere apportate
direttamente sul portale o lavorando in locale sul proprio computer.

Per creare una pull request, se non si hanno i permessi per lavorare nel
repository originale, si lavora in un fork ed è quindi necessario
seguire gli step riportati in sintesi di seguito:

-  con un account GitHub effettuare un **fork**\ del repository su cui
   si vuole contribuire con una modifica

-  creare una *copia locale del fork* fatto allo step precedente
   (accesso in lettura/scrittura)

-  aggiungere un nuovo riferimento al *repository remoto
   (*\ denominato\ *upstream)*\ del progetto originale così da poter
   sincronizzare il software del repository locale con eventuali
   modifiche che nel frattempo possono intercorrere su quello remoto
   della community (accesso in sola lettura)

-  sincronizzare la copia locale con la linea di codice corretta (vari
   *branch o master*). Se il progetto segue il *git-flow*, saranno
   presenti sia il branch *master*\ che *develop*. In caso di bugs si
   creerà il *branch*\ partendo da master, per nuove features invece da
   *develop*. Nel caso sia presente solo master si creerà partendo da
   master stesso.

-  creare branch considerando che i nomi dei branch hanno normalmente
   prefissi hotfix/ o feature/ in base al tipo di modifica che si vuole
   fare

-  effettuare la modifica al codice

-  generare la Pull Request per inviare la modifica dal repository
   locale al repository originale

-  Successivamente su `GitHub <https://github.com/>`__ andare sul fork
   creato e cliccare, “Compare & pull request”

-  Inserire titolo e descrizione della modifica effettuata osservando le
   indicazioni riportate nel file CONTRIBUTING.md presente nella root
   del repository

-  controllare il diff dei cambiamenti che la Pull Request apporta

-  cliccare su “Create Pull Request” per sottomettere la modifica al
   software maintainer per revisione.

-  se la modifica non viene accolta, è necessario, rispondere ad
   eventuali richieste di code review

La piattaforma come per gli issue consente di personalizzare e
standardizzare le informazioni inserite in una nuova pull request
attraverso gli opportuni template di configurazione.

La ricerca della pull request sul portale segue le stesse logiche della
ricerca implementata per gli issue.



Gestione delle segnalazioni inerenti la sicurezza software e vulnerability
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In considerazione dell’importanza che riveste l’aspetto della sicurezza
informatica nel contesto delle applicazioni in ambito sanitario che
trattano dati personali e sensibili, risulta fondamentale definire nella
Community del Taccuino le modalità con cui trattare eventuali
segnalazioni di bachi e vulnerabilità di sicurezza rilevate dagli
utenti.

Tali bug devono essere trattati con maggiore attenzione rispetto ai bug
di programmazione gestibili attraverso il processo di gestione delle
pull request.

A questo scopo è best practice indicare le modalità di gestione delle
vulnerabilità in una sezione del sito del progetto dedicata alle
**Responsible Disclosure Policy.**

Si può prevedere di inviare le *segnalazioni via e-mail* ad un apposito
indirizzo di posta del software maintainer. Si consiglia di utilizzare
una cifratura (con chiave PGP) sui dettagli della segnalazioni per
evitare che le informazioni critiche siano utilizzabili da terzi per
fini malevoli. La segnalazione deve essere corredata dalle informazioni
utili che consentano di riprodurre la vulnerabilità come ad esempio:

-  *tipo di vulnerabilità;*

-  *servizio o URL o IP interessati;*

-  *requisiti per riprodurre il problema;*

-  *informazioni necessarie per riprodurre il problema;*

-  *impatto della vulnerabilità insieme a una spiegazione di come un
   utente malintenzionato potrebbe trovarla e sfruttarla.*

Nel caso dei progetti della PA centrale “PagoPA” e “IO”, la sezione
suddetta è stata denominata “sicurezza” ed è linkata in fondo alla
homepage del sito dei rispettivi progetti.

.. |image47| figure:: /immagini/100002010000063100000399379C06D5FF5CC3DB.png
   :scale: 50 % 
   :alt: Sezione sicurezza di App IO

   Strumenti di collaboration



Editing condiviso con Wiki
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In ogni repository di GitHub è inoltre disponibile un wiki, uno
strumento facile e veloce per redigere documenti in modalità condivisa.

Nell’esempio sono state create due pagine e in particolare la
**Home** ha un collegamento ipertestuale alla pagina di prova **Pagina1**

.. |image48| figure:: /immagini/10000201000003DD000001A1268673E4320169B3.png
   :scale: 50 % 
   :alt: Esempio di Wiki

   Esempio di Wiki

Le pagine possono essere scritte in vari linguaggi come ad esempio
mediaWiki (conosciuto per Wikipedia), markdown (.md) e reStructuredText
(.rst).

.. |image49| figure:: /immagini/10000201000003D2000001BF2F8D869764C6F6D9.png
   :scale: 50 % 
   :alt: Linguaggi delle pagine Wiki

   Linguaggi delle pagine Wiki

Strumenti di collaboration
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A completamento degli strumenti in precedenza descritti, si possono
aggiungere servizi per favorire la collaborazione fra gli utenti della
Community del Taccuino Personale e quindi gestire **comunicazioni
asincrone**, come ad esempio forum, mailing list e newsletter, e
**sincrone**, come la chat.

Tali strumenti possono essere predisposti in funzione delle esigenze
specifiche e della crescita della Community stessa. Si deve considerare
inoltre che troppi strumenti possono “confondere” e “disperdere le
informazioni che si vogliono veicolare” e pertanto deve essere
attentamente valutato il loro inserimento per convergere su quelli più
efficienti ed efficaci per gli scopi comunicativi che si vogliono
raggiungere.

Nel primo caso la comunicazione prevede un interazione fra gli utenti
non istantanea (del tipo “scrivo e aspetto”) ed è più strutturata. Nel
**forum** è richiesto un gestore dei contenuti che vengono pubblicati e
pertanto lo strumento deve essere presidiato. Un esempio di tool open
source è *Discourse*, utilizzato peraltro da Developers
Italia.

.. |imageC| figure:: /immagini/100002010000012400000058F047157144C9A970.png
   :scale: 50 % 
   :alt: Discourse

   Discourse


Altri tipi di strumento di comunicazione asincrona sono:

-  la **mailing list**  ovvero l’invio di email su temi specifici ad una
   lista di utenti che possono interagire fra di loro. Tali email
   vengono normalmente rese accessibili pubblicamente online e
   indicizzate.

-  la **newsletter**  ovvero l’invio di email per la comunicazione di
   news (ad esempio nuove release software) in modalità unidirezionale
   verso gli utenti iscritti.

E’ da notare come le piattaforme di gestione delle email tendano ad
includere funzionalità tipiche sia di mailing list sia di newsletter.
Esempi di strumenti open source sono: *Dada Mail, GNU Mailman, phpList e
OpenEMM.* 

Per le comunicazioni istantanee fra gli utenti si possono predisporre
strumenti di comunicazione sincrona. Nel caso di una Community come
quella del Taccuino si può prevedere che i Team di progetto siano utenti
dello strumento di **chat**  per favorire il coinvolgimento degli utenti
e contributori. 

Developers Italia ad esempio utilizza il servizio SaaS di chat Slack
(soluzione proprietaria).

Alternative open source a questo strumento possono essere: *Mattermost,
Zulip Chat e Rocket.Chat*. 

E’ da notare come sul repository GitHub sia nativamente integrato lo
strumento di chat *Gitter*.

.. |imageC| figure:: /immagini/collaboration.jpg
   :scale: 50 % 
   :alt: Strumenti di collaboration

   Strumenti di collaboration
