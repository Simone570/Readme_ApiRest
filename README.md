# Readme_ApiRest
API REST 

Prima di poter parlare di cosa sono le API REST, è necessario fare una breve parentesi sulle singole parole: REST ed API. 
 
COSA SONO LE API?

Le API (acronimo “application programming interface”) sono set di definizioni e protocolli con i quali vengono realizzati e integrati software applicativi. Consentono ai tuoi prodotti o servizi di comunicare con altri prodotti o servizi senza sapere come vengono implementati, semplificando così lo sviluppo delle app e consentendo un netto risparmio di tempo. Durante la creazione di nuovi strumenti e prodotti, le API offrono flessibilità e semplificano la progettazione. 
 
A COSA SERVONO LE API?

Al giorno d’oggi, diversi produttori di software mettono a disposizione le API per facilitare l’accesso dei programmatori ai componenti software. SAP, Amazon e Google, ad esempio, offrono API per diverse aree di applicazione. Gli sviluppatori possono utilizzare queste interfacce per eseguire varie attività:

-inoltrare un comando del programmatore al software e riceverne la risposta

-inserire contenuti nei servizi web

-riutilizzare i codici delle app attraverso l’interazione tra programmi

-controllare l’accesso da parte di altri programmatori

Nell’uso quotidiano, le API vengono utilizzate, ad esempio, nei servizi web.

COME FUNZIONANO LE API? 

Anche se le API offrono diversi vantaggi all’utente finale, servono principalmente ai programmatori. L’Application Programming Interface viene solitamente fornita dagli sviluppatori di un software in modo che i programmatori di altre applicazioni possano utilizzarla. L’interfaccia di programmazione determina come le informazioni e i dati vengono ricevuti e restituiti tra i moduli. Google, ad esempio, pubblica l’API per consentire ad altri programmatori di ancorare le proprie applicazioni ai servizi Google. A questo scopo si utilizza poi uno standard specifico, a cui il software esterno deve aderire.

Il protocollo REST è molto popolare per la comunicazione tra le applicazioni, soprattutto sul web.

Quali tipi di API esistono? 

Esistono fondamentalmente quattro diverse classi di interfacce di programmazione:

-API orientate alle funzioni  

-API orientate ai file 

-API orientate al protocollo  

-API orientate agli oggetti 

La scelta della classe dipende dall’area di applicazione. Le interfacce di programmazione orientate alle funzioni sono interfacce relativamente complesse. Consentono, ad esempio, agli sviluppatori di accedere ai componenti hardware. In esse vengono richiamate sempre solo le funzioni. Le API orientate ai file consentono la connettività a livello di file. I dati possono quindi essere interrogati e scritti. L’interfaccia orientata al protocollo viene utilizzata per la comunicazione standardizzata tra programmi, ma è indipendente dai sistemi operativi o dall’hardware. Le API orientate agli oggetti possono essere utilizzate in modo flessibile.

COS'E' il REST? 
 
Quando si parla di REST (Representational State Transfer) ci si riferisce a un’architettura software, questo approccio architetturale è USATO per creare web API basandosi sul protocollo HTTP. 

Il REST è infatti un sistema di trasmissione dei dati che utilizza l’HTTP e che fa un grande uso delle sue funzioni, ricorrendo ai comandi: 

-GET: usato per richiedere informazioni al server. 

-POST: usato per inviare nuovi dati al server. 

-PUT: è necessario per aggiornare i dati presenti nel server. 

-DELETE: invia una richiesta per la cancellazione di informazioni. 

Grazie a questi si riesce ad identificare ben precise risorse presenti in tutto il vasto web. Questa architettura nonostante faccia un enorme uso del protocollo di trasferimento HTTP, funziona molto bene anche con i protocolli di trasferimento come SNMP o SMTP. 
 
PRINCIPI E VINCOLI rest

I principi che deve rispettare una architettura REST sono:

-CLIENT-SERVER

in questo caso si parla di separazione dei compiti (SoC) per indicare che il client e il server hanno compiti tra loro ben definiti e dedicati. Ognuno di loro si occupa di ben determinati aspetti e funzionalità, evitando così qualsiasi accavallamento di competenze;

-STATELESS

questo principio si basa sull’assenza di stato durante la comunicazione tra server e client. Quando il client invia una richiesta al server, essa deve contenere tutte le informazioni

-CACHE

in un Architettura REST i messaggi di risposta dal servizio ai suoi consumatori sono esplicitamente etichettati come cachabili o non. In questo modo, il servizio, il consumatore o uno dei componenti middleware intermediari possono memorizzare nella cache la risposta per il riutilizzo nelle richieste successive.

-INTERFACCIA UNIFORME

Per avere un caching efficiente in una rete, i componenti devono essere in grado di comunicare tramite un’interfaccia uniforme. Con un’interfaccia uniforme, il carico utile può essere trasferito in un formato standard.
 
API REST  

Le API REST quindi, non è altro che un’API che segue i principi REST e utilizza un protocollo HTTP o HTTPS(che però richiede un certificato), per scambiare dati, che possono essere di diverso formato: XML, JSON e YAML, una architettura API normale(SOAP) utilizza solamente i dati di tipo XML. Le API REST offrono una maggior flessibilità in termini di comunicazione dati, ossia che è in grado di servire più applicazioni client o server che comunicano usando diversi formati 
Per essere considerata RESTful, deve rispettare i criteri indicati di seguito:

-Un sistema su più livelli che organizza ogni tipo di server (ad esempio quelli responsabili della sicurezza, del bilanciamento del carico, ecc.) che si occupa di recuperare le informazioni richieste in gerarchie, invisibile al client.

-Codice on demand (facoltativo): la capacità di inviare codice eseguibile dal server al client quando richiesto, estendendo le funzioni del client. 

I VANTAGGI DELL'UTILIZZO DELLE API REST

Numerosi sono i vantaggi derivanti dal loro utilizzo, sia su un sito WordPress(ovvero un sistema di gestione dei contenuti che ti permette di poterlo utilizzare per creare siti internet e blog senza conoscere nulla di programmazione.) o su un e-commerce. Eccone alcuni: 

-Indipendenza: le API Rest sono indipendenti dai linguaggi o da precise piattaforme. Si sanno adattare sempre e in ogni occasione, garantendo quindi la massima libertà. 

-Separazione Client-Server: non è solo uno dei principi fondamentali del REST, ma rappresenta un vero e proprio vantaggio. Grazie a tale separazione, infatti, consente di trattare indipendentemente l’evoluzione delle diverse componenti, PER ESEMPIO modificare solo una parte progettuale senza, per questo, essere obbligati a mettere mano sia al server che al client. L’interfaccia utilizzata, inoltre, è utilizzabile su diverse tipologie di piattaforme. 

-Scalabilità: la separazione Client-Server si traduce in una miglior scalabilità del sistema stesso. 
 
ESERCIZIO

const http= require( 'http' ) "Node js offre già della api come http. Questo serve a importare il modulo e lo assegna a una variabile"
 
http.createServer(function(req,res){ "Comando per inizializzare il server, al suo interno va inserita una funzione con parametri/argomenti dove uno è la richiesta e l'altro la risposta della comunicazione"
	
           res.write('Ciao');"Questa inizia la risposta della comunicazione"
	         res.end();"Questa chiude la risposta"
 
}).listen(5000);"Porta d'ascolto"
 
 
 
 

