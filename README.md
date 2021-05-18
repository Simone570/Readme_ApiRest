
# API REST
Le API REST quindi, non è altro che un’API che segue i principi REST e utilizza un protocollo HTTP o HTTPS(che però richiede un certificato), per scambiare dati, che possono essere di diverso formato: XML, JSON e YAML, una architettura API normale(SOAP) utilizza solamente i dati di tipo XML. Le API REST offrono una maggior flessibilità in termini di comunicazione dati, ossia che è in grado di servire più applicazioni client o server che comunicano usando diversi formati 
Per essere considerata RESTful, deve rispettare i criteri indicati di seguito:

- Un sistema su più livelli che organizza ogni tipo di server (ad esempio quelli responsabili della sicurezza, del bilanciamento del carico, ecc.) che si occupa di recuperare le informazioni richieste in gerarchie, invisibile al client.

- Codice on demand (facoltativo): la capacità di inviare codice eseguibile dal server al client quando richiesto, estendendo le funzioni del client. 

# I VANTAGGI DELL'UTILIZZO DELLE API REST

Numerosi sono i vantaggi derivanti dal loro utilizzo, sia su un sito WordPress(ovvero un sistema di gestione dei contenuti che ti permette di poterlo utilizzare per creare siti internet e blog senza conoscere nulla di programmazione.) o su un e-commerce. Eccone alcuni: 

- Indipendenza: le API Rest sono indipendenti dai linguaggi o da precise piattaforme. Si sanno adattare sempre e in ogni occasione, garantendo quindi la massima libertà. 

- Separazione Client-Server: non è solo uno dei principi fondamentali del REST, ma rappresenta un vero e proprio vantaggio. Grazie a tale separazione, infatti, consente di trattare indipendentemente l’evoluzione delle diverse componenti, PER ESEMPIO modificare solo una parte progettuale senza, per questo, essere obbligati a mettere mano sia al server che al client. L’interfaccia utilizzata, inoltre, è utilizzabile su diverse tipologie di piattaforme. 

- Scalabilità: la separazione Client-Server si traduce in una miglior scalabilità del sistema stesso. 
 
# ESERCIZIO

const http= require( 'http' ) "Node js offre già della api come http. Questo serve a importare il modulo e lo assegna a una variabile"
 
http.createServer(function(req,res){ "Comando per inizializzare il server, al suo interno va inserita una funzione con parametri/argomenti dove uno è la richiesta e l'altro la risposta della comunicazione"
	
           res.write('Ciao');"Questa inizia la risposta della comunicazione"
	         res.end();"Questa chiude la risposta"
		 }).listen(5000);"Porta d'ascolto"
 
 # DESCRIZIONE MATERIALI UTILIZZATI
 
 I materiali utilizzati per raccogliere le informazioni principali dell'argomento sono:
 - Microsoft Word
 - YouTube
 - GoogleChrome

Per la presentazione e spiegazione dell'argomento è stato utilizzato Microsoft PowerPoint, utilizzando il seguente file
[ApiRest.pptx](https://github.com/eltommis/ApiRest/files/6500715/Presentazione2.2.1.pptx)
<br>
Per la presentazione degli esercizi è stato utilizzato un file di tipo PDF, usando il seguente file
[Esercizi ApiRest.pdf](https://github.com/eltommis/ApiRest/files/6500697/Esercizi.ApiRest.pdf)

 
 # DESCRIZIONE STRUMENTI/TECNOLOGIE
 
Per la realizzazione dei programmi è stato consigliato di utilizzare:
- XAMP: dalla quale ci si può collegare, attivando Apache, PhpMyAdmin.
- VisualStudio: per scrivere il codice necessario per la creazione della pagina client-server
