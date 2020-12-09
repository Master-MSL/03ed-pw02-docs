Analisi del contesto mobile in relazione ai device wearable e medicali
========================================================================

Nel presente capitolo viene effettuata un’analisi del contesto
tecnologico per poter individuare le possibili soluzioni software
realizzabili nell’ambito del progetto di evoluzione del taccuino al fine
di integrare **device wearable e medicali**\ da cui acquisire **nuovi
dati in modalità più automatizzata e agevole per l’utente.**

-  Modalità di integrazione dei device
-------------------------------------------

Per alimentare il sistema software del Taccuino con i dati acquisiti
dalle diverse tipologie di device è necessario individuare una
componente software (**gateway**) che ha il compito di intermediare la
comunicazione fra i dispositivi e il Taccuino del sistema regionale di
FSE (FSEr- Fascicolo Sanitario Elettronico regionale).

.. |image9| figure:: /immagini/10000201000002CF000001398C400AE171C4FBF5.png
   :scale: 60 % 
   :alt: Modalità di integrazione dei device

   Modalità di integrazione dei device

In continuità con l’approccio “mobile first” adottato nel processo di
evoluzione dell’ecosistema della sanità digitale piemontese, realizzato
secondo le linee guida nazionali [25]_, si ritiene che tale
ruolo di gateway possa essere assolto prioritariamente dallo
*smartphone*, in quanto strumento in grado di collegarsi via bluetooth
ai device ed inoltre maggiormente diffuso tra i cittadini. Il tablet
viene considerato in subordine all'uso dello smartphone anche in
considerazione del fatto che è comunque meno diffuso, le app sviluppate
per il primo funzionano anche per il secondo e comunque come strumento
seppur portatile è di fatto di dimensioni più ampie e quindi meno
appropriato per l’ambito fitness e wellness. Le modalità di integrazione
possono essere di vario tipo ma i principali modelli sono quelli
riportati di seguito:

-  **Integrazione diretta,** che presuppone le gestione completa
   dell’interfacciamento via Bluetooth con i device da parte di un app
   regionale presente su smartphone. Tale integrazione prevede la
   gestione del pairing fra app e device, il discovery dei servizi
   esposti dal dispositivo e il recupero e la relativa gestione dei dati
   sanitari provenienti dal dispositivo.

.. |image10| figure:: /immagini/10000201000003BA00000138FD0467069F8823F4.png
   :scale: 60 % 
   :alt: Modalità di integrazione diretta

   Modalità di integrazione diretta

-  **Integrazione indiretta con interscambio di dati**, che presuppone:

   -  il trasferimento dei dati dal device ad un’app di terzi

   -  successivo passaggio delle informazioni dall’app di terzi a quella
      regionale integrata con il sistema di Taccuino.

   In questo ambito si possono individuare due ulteriori sotto-scenari:

      -  *interscambio attraverso uso di SDK correlati ad Health App.* I
         sistemi operativi di smartphone e le relative app dedicate ad
         accentrare la gestione dei dati sanitari (d’ora in poi Health
         app [26]_) mettono a disposizioni API per leggere tali
         dati da app esterne, come quella regionale, previa abilitazione
         dell’app da parte dell’utente. L’app regionale dovrà
         successivamente inviare i dati recuperati sul sistema di
         Taccuino presente nel FSEr via servizi Json/rest. Le Health app
         si possono interfacciare direttamente ai device come ad esempio
         accade per alcuni smartwatch (ad esempio nel caso dell’apple
         watch con app Salute su iPhone) o a loro volta accentrano i
         dati provenienti da app di terzi previste dai fornitori dei
         device stessi (ad esempio app Omron per gestione dei dati delle
         pressione che vengono poi inseriti nell’app Salute dell’iPhone
         o nell’app Samsung Health su Smartphone Android).


.. |image11| figure:: /immagini/100002010000038900000159A836B6777EEBF1A5.png
   :scale: 60 % 
   :alt: Integrazione indiretta con interscambio di dati attraverso uso di SDK correlati ad Health App

   Integrazione indiretta con interscambio di dati attraverso uso di SDK correlati ad Health App
-  
   -  
      -  *interscambio attraverso import di file esportati da App
         sanitarie di terzi*\ ovvero le app dedicate alla gestione dei
         dati sanitari (Health app o app di fornitori di device) mettono
         a disposizione dell'utente delle funzionalità di export dei
         dati su file system dello smartphone che possono essere poi
         importati manualmente nell’app regionale che si interfaccia al
         sistema di Taccuino presente nel FSEr.

.. |image12| figure:: /immagini/100002010000038E000001327ADFABAFB39D7493.png
   :scale: 60 % 
   :alt: Integrazione indiretta con interscambio di dati attraverso import di file esportati da App sanitarie di terzi

   Integrazione indiretta con interscambio di dati attraverso import di file esportati da App sanitarie di terzi

Rientrano nelle Health app ad esempio le seguenti
applicazioni:

-  app Salute presente su iPhone con sistemi operativi Apple iOS. E’
   disponibile un SDK HealthKit per sviluppare app native su iOS e
   watchOS . Il badge “Works with Apple Health” viene utilizzato per comunicare
   visivamente la compatibilità di un app con l'app Salute di Apple su iPhone. 
   
.. |image13| figure:: /immagini/1000020100000117000000EE36CCBEBAB94F98D9.png
   :scale: 100 % 
   :alt: HealthKit di Apple

   HealthKit di Apple

.. |image14| figure:: /immagini/10000201000001200000005C30CA5C1606DAFF18.png
    :scale: 100 % 
    :alt: Badge “Works with Apple Health”

    Badge “Works with Apple Health”
   

-  app Google Fit disponibile per sistemi operativi Android e iOS. E’ da
   notare che la versione dell’app Google Fit con iOS si interfaccia
   all’app Salute di Apple per riceverne i dati se autorizzata
   dall’utente. Google Fit inoltre mette a disposizione API rest
   fruibili da qualsiasi piattaforma per smartphone, tablet o PC.

.. |image15| figure:: /immagini/100002010000044E0000026DA1319B3F0D2871EA.png
    :scale: 100 % 
    :alt: Rest API di Google

    Rest API di Google https://developers.google.com/fit/rest


-  app Samsung Health disponibile per sistemi operativi Android e iOS.
   In ambito android Samsung mette a disposizione degli sviluppatori un
   SDK per l’interfacciamento con l’app e una SDK per consentire ai
   fornitori di device partner di Samsung di connettere i propri
   dispositivi compatibili Bluetooth Low Energy (BLE) all’app Samsung
   Health. Samsung Health dispone anche di un cloud per il salvataggio
   dei dati ma non mette a disposizione API rest fruibili da qualsiasi
   piattaforma. E’ da notare che la versione dell’app per iOS si
   interfaccia all’app Salute di Apple per riceverne i dati se
   autorizzata dall’utente.

.. |image16| figure:: /immagini/10000201000001200000005C30CA5C1606DAFF18.png
    :scale: 100 % 
    :alt: Samsung Health SDK for Android

    Samsung Health SDK for Android https://developer.samsung.com/health/android/overview.htmlt


.. |image17| figure:: /immagini/10000201000001200000005C30CA5C1606DAFF18.png
    :scale: 100 % 
    :alt: Samsung Health SDK for Device

    Samsung Health SDK for Device https://developer.samsung.com/health/device/overview.html


Di seguito viene riportata un’analisi comparativa delle modalità di
integrazione individuate.

.. |imagetab| figure:: /immagini/tabella1.png
   :scale: 60 % 
   :alt: Modalità di integrazione

   Modalità di integrazione

In considerazione della disamina riportata nella tabella precedente,
emerge come lo scenario B sia quello più perseguibile.

Lo scenario C sia di fatto affiancabile al B in un secondo tempo o
comunque a corredo/completamento di esso.

Lo scenario A, in considerazione della complessità e maggiore
onerosità, sia di fatto utile se si individua un’applicazione e
necessità specifica.

-  Ampiezza del bacino di utenza
----------------------------------------

In considerazione degli scenari sopra descritti, delle attuali quote di
mercato riportate di seguito e ricavate dal sito
https://gs.statcounter.com/:

.. |imageDiff| figure:: /immagini/diffusioneDevice.jpg
   :scale: 80 % 
   :alt: Diffusione dei device e dei sistemi operativi mobile

   Diffusione dei device e dei sistemi operativi mobile

si ritiene opportuno per garantire la fruizione dei dati ad un
significativo bacino di utenza che l'APP regionale di acquisizione dei
dati sanitari dai dispositivi per l'alimentazione del Taccuino del FSE
Regionale sia sviluppata sia per sistema operativo **Android**\ sia per
**iOS**.

Si prevede di integrare nel Taccuino personale del FSE regionale

-  **dispositivi medici (ai sensi D. Lgs. n. 46/1997)**

-  **dispositivi wearable.**

integrabili con smartphone.


-  Analisi comparativa delle HealthApp
---------------------------------------------------

Come noto, e già osservato in precedenza, l’attuale diffusione degli
smartphone e la loro versatilità ne fanno il device principale per la
fruizione di servizi on line e già oggi è significativa la casistica di
processi articolati su più fasi: autenticazione (anche con credenziali
forti), interazione con l’utente, erogazione del servizio richiesto,
notifica ed eventuali integrazioni con altri servizi, disponibili
tramite apposite App (si pensi agli acquisti on line, all’internet
banking, al ritiro referti on line, ecc.).

Anche nel settore del wellness (e della cura della persona in generale),
sono numerose le applicazioni che consentono di utilizzare lo
smartphone, direttamente o tramite la connessione con ulteriori device
dedicati (es. fitband, activity tracker, smartwatch, e altri
dispositivi) come collettore per il monitoraggio degli stili di vita, di
eventuali percorsi terapeutici, e più in generale per l’acquisizione di
di informazioni utili per i medici che prendono in cura l'assistito.

Tali soluzioni possono considerarsi ormai piuttosto consolidate, e in
alcuni casi possono costituire un effettivo riferimento per dati e
misurazioni che i cittadini possono autonomamente acquisire e gestire
con profitto ai fini dell'archiviazione.

A tale proposito si è ritenuto utile ai fini della successiva
implementazione dell’App Taccuino, svolgere uno scouting sulle
informazioni gestite dalle principali applicazioni, rappresentato in
forma comparativa.

Considerate le quote di mercato delle più diffuse piattaforme, dei
principali vendor e - non ultimo - il successo in termini di gradimento
da parte della clientela, quest’ultimo valutato empiricamente tramite
numero di download e valutazione degli utenti registrato sulle
piattaforme di distribuzione delle App (App Store e Google Play), sono
stati presi in considerazione le seguenti:

-  app Salute presente sui sistemi operativi Apple iOS

-  app Samsung Health disponibile per sistemi operativi Android e iOS

-  app GoogleFit disponibile per sistemi operativi Android e iOS

.. |imageApp| figure:: /immagini/healthApp.jpg
   :scale: 80 % 
   :alt: HealthApp di Apple, Google e Samsung

   HealthApp di Apple, Google e Samsung


Di seguito un raffronto delle principali informazioni gestite e
funzionalità offerte, con indicazione relativa alla presenza nei dati
attualmente gestiti dal Taccuino FSE ovvero all’interesse per
un’eventuale fase di evoluzione del medesimo (con particolare
riferimento alle grandezze che più si prestano ad acquisizioni
automatizzate e/o massive).

.. |image| figure:: /immagini/tabella2.png
   :scale: 60 % 
   :alt: Analisi comparativa delle HealthApp

   Analisi comparativa delle HealthApp

È immediato osservare che solo una piccola parte delle informazioni è
gestita da tutte le App e più in generale si rileva che le informazioni
gestite nelle diverse soluzioni non sono omogenee.

A valle di tale analisi speditiva si è acquisita una visione più precisa
delle tipologie di informazioni attualmente gestite dalle App più
diffuse, e del diverso grado di maturità e dettaglio nelle differenti
soluzioni proposte.

È evidente che offrire funzionalità di integrazione con il taccuino
analoghe per utenti Apple e Android e garantire loro la gestione dello
stesso set di informazioni ipotizzando di utilizzare la App attuali come
“collettori” non sia per nulla agevole, se non prevedendo un ampio
ricorso alla possibilità di inserimenti manuali e/o all’upload di file
in formato standard, che sono però soluzioni di scarso appeal per gli
utenti.

Inoltre è opportuno considerare che anche le App esaminate in taluni
casi prevedono l’integrazione con altri dispositivi - spesso di
specifici vendor al fine di un’integrazione ottimale - in grado di
acquisire i dati, talvolta di notevole interesse per i processi di cura
(es. livelli di stress, frequenza cardiaca in continuo, durata e qualità
del sonno, ecc.).

Tali considerazioni costituiscono un elemento importante nella
valutazione funzionale all’individuazione dell’approccio più conveniente
secondo il quale organizzare il progetto e la programmazione della fase
attuativa.

.. [25] Linee guida sull'accessibilità degli strumenti informaticiguida AgID https://www.agid.gov.it/it/design-servizi/accessibilita/linee-guida-accessibilita-strumenti-informatici

.. [26] Sono app di grandi vendor che implementano un sistema di gestione di dati in ambito salute accentrando le misurazioni provenienti da: 1) dispositivi medicali esterni: ossimetri, glucometri, bilance, termometri, misuratori di pressioni e frequenza cardiaca 2) smartwatch e activity tracker