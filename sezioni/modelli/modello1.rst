Modello 1 - Community con contributi alle App regionali
=========================================================

Questo approccio prevede di impostare uno sviluppo di App regionali per
l’integrazione di device con il sistema del Taccuino del FSE della
Regione Piemonte a iniziativa e titolarità regionali, ma gestite fin
dall’inizio con modalità aperte, pubblicando tale codice in open source
su Code repository GitHub. Con questo modello il progetto punta a creare
una Community per favorire la contribuzione da parte di terzi in termini
di software, idee e conoscenze volte ad arricchire il sistema verso
l'utente finale e diffonderne l’uso.

Concretamente, si prevede la realizzazione di App
regionali  [30]_ per iOS e Android con il compito di fungere da
gateway tra il device e la piattaforma regionale del Fascicolo Sanitario
Elettronico (FSE), provvedendo all’autenticazione dell’utente e
all’acquisizione e al caricamento dei dati provenienti dai device nel
Taccuino.

I compiti delle App regionali sono descritti nel capitolo `Modalità di
integrazione dei device <#_8dnz78msojq0>`__ dove si analizzano le
possibili modalità di acquisizione dei dati utili per il Taccuino
provenienti da device medicali e wearable. Si prevede di sfruttare le
logiche di interfacciamento software (API e SDK) ed i formati in uso da
parte di applicazioni di larga diffusione, preinstallate o scaricabili
gratuitamente su tutti gli smartphone, progettate per acquisire,
archiviare e condividere informazioni sullo stato di salute e sugli
stili di vita.

Il progetto attuativo prevede, a seguito della formalizzazione della
*roadmap*\ di progetto da parte dello steering committee:

-  una prima fase di sviluppo - da parte di CSI, software maintainer -
   dedicata al “core” delle APP regionali e all’integrazione di un
   sottoinsieme significativo di device presenti sul mercato, che si
   chiude con il rilascio di funzionalità di base immediatamente
   fruibili;

-  una seconda fase, immediatamente successiva, di apertura ai
   contributi della Community, mirata all’incremento delle funzionalità
   offerte e soprattutto allo sviluppo del software necessario per
   estendere in misura sensibile l’integrazione con il Taccuino di
   ulteriori tipologie di dati, di device e di App orientate alla
   gestione di dati inerenti la Salute ed il Fitness/Wellness.

Il software sviluppato viene ospitato su repository di code hosting di
titolarità regionale `(rif. § Repository pubblico) <#_wk9a0i7p4nu0>`__.
I contributi possono essere inseriti attraverso le funzionalità messe a
disposizione dalle piattaforma di code hosting per favorire la
collaborazione degli utenti e per la gestione di pull request e delle
issue `(rif. § Strumenti di interazione per gli utenti della
Community) <#_hu9bddmya7ms>`__.

In questo modello, le soluzioni inizialmente pubblicate possono
“evolvere” anche con il contributi di terzi, mediante gli strumenti
messi a disposizione dal repository stesso, prevalentemente mediante due
modalità:

A. contributi minimali alle app già pubblicate, in termini di correzioni
   e/o miglioramenti *interni*\ al codice

B. contributi sostanziali e/o significativi (quali ad esempio ulteriori
   App, interi moduli, componenti o funzionalità complesse di nuova
   realizzazione)

In considerazione del fatto che qualsivoglia contributo è potenzialmente
creativo, ed in quanto tale comporta l’attribuzione al contributore dei
relativi diritti patrimoniali e morali, la proprietà intellettuale nel
caso A) resta in capo alla Regione Piemonte, e si prevede semplicemente
la citazione degli autori dei contributi nell’apposito file
(*Authors.txt*) su repository di code hosting.

Nel caso B) sopra descritto, invece, si possono attuare due differenti
modalità di gestione:

-  trasferimento alla Regione Piemonte dei diritti patrimoniali sul
   software (in coerenza con la licenza prescelta);

-  mantenimento della proprietà del software in capo al contributor, e
   rilascio del medesimo con licenza (compatibile con quella del
   software già rilasciato) che ne permette l’utilizzo, l’integrazione e
   la distribuzione per gli obiettivi del progetto regionale.

In entrambi i casi il mantenimento del software sarebbe in carico al
software maintainer (CSI Piemonte).

In generale le regole di contribuzione e le modalità operative con cui i
contributor possono relazionarsi con il software maintainer sono
descritte in un file apposito all’interno del repository di code hosting
(*Contributing.txt*).

Da un punto di vista delle responsabilità, tutti i contributi software
devono essere sottoposti a verifica formale da parte del software
maintainer per garantire

-  la corretta gestione dei dati personali e sanitari da un punto di
   vista della privacy

-  l’interpretazione corretta dei dati sanitari provenienti dai device

-  l’aderenza alle funzionalità previste a livello strategico e
   operativo.

In questo modello si prevede uno steering committee, come descritto nel
capitolo `Strategie <#_f6f2ogjfbtc>`__ della “Fase attuativa” del
progetto, con alto potere decisionale (composto da Regione e
CSI-Piemonte) che si concentra sulla definizione della roadmap di
progetto demandando la governance della community al CSI-Piemonte in
qualità di software maintainer.

Si tratta pertanto di un modello con potenzialità enormi che, in
relazione ai principali punti di forza e debolezza attesi (inquadrati a
livello macroscopico nella SWOT analysis riportata di seguito),
richiede:

-  un investimento iniziale da parte di una PA che definisce un
   obiettivo di sviluppo;

-  un’accurata pianificazione organizzativa e un'adeguata preparazione
   per la gestione della Community, che assume un ruolo centrale di
   tutto il progetto.


.. |image| figure:: /immagini/swotModello1.jpg
   :scale: 60 % 
   :alt: SWOT del modello basato su Community OS

   SWOT del modello basato su Community OS

.. [30] In realtà dovranno essere sviluppate due versioni analoghe della medesima APP: una per s.o. Android e una per iOS