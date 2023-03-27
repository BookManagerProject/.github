# 📚 Book Finder

## Descrizione
BookFinder è un sistema software il cui obbiettivo è quello di permettere agli utenti di trovare libri e di catagolarli comodamente attraverso un bot Telegram. Gli utenti potranno cercare comodamente tramite foto o testo i propri libri e aggiungerli ai preferiti tutto tramite il bot messo a disposizione

## 🌐 Descrizione dei servizi utlizzati 🌐

- **Bot di Azure**: è un servizio di Azure che consente di creare bot conversazionali altamente scalabili e personalizzati, che possono interagire con gli utenti tramite diverse piattaforme come Facebook Messenger, Skype, Slack e altri.

- **Servizio app**: è un servizio di Azure che consente di creare, ospitare e gestire applicazioni web, mobili e API in modo semplice e scalabile. Supporta una vasta gamma di tecnologie di sviluppo e linguaggi di programmazione, tra cui ASP.NET, Node.js, PHP, Python e altri.

- **App Spring di Azure**: è un servizio di Azure che offre un'esperienza di hosting per le applicazioni basate sul framework Spring, che è molto popolare tra i programmatori Java. Con questo servizio, è possibile creare rapidamente applicazioni Java Spring in Azure, configurando l'infrastruttura sottostante e i servizi correlati.

- **Bing Search**: è un servizio di ricerca Web offerto da Microsoft che consente di integrare la ricerca in un'applicazione o un sito Web. Fornisce una vasta gamma di funzionalità di ricerca avanzate, tra cui ricerche di immagini, notizie, video e mappe.

- **Language Understanding (LUIS)**: è un servizio di Azure che consente di creare e personalizzare modelli di linguaggio naturale per le applicazioni di intelligenza artificiale. Con LUIS, è possibile aggiungere funzionalità di analisi del linguaggio naturale alle applicazioni, comprese le capacità di riconoscimento dell'intento e di estrazione delle entità.

- **Account multi-servizi Servizi cognitivi**: è un account di Azure che consente di accedere a una vasta gamma di servizi cognitivi di Microsoft, tra cui la visione artificiale, il riconoscimento vocale e la comprensione del linguaggio naturale. Con questo account, è possibile utilizzare questi servizi per aggiungere funzionalità di intelligenza artificiale alle proprie applicazioni.

- **Azure SQL**: è un servizio di database relazionale gestito offerto da Microsoft Azure, progettato per supportare tutte le funzionalità del database SQL Server e per fornire un'esperienza di gestione dei dati scalabile e sicura per le applicazioni aziendali.


## ☁ Vantaggi offerti da un ambiente cloud ☁

L'utilizzo di un ambiente cloud come Azure offre numerosi vantaggi in termini di flessibilità, sicurezza, scalabilità e affidabilità. Di seguito sono riportati alcuni vantaggi specifici dei servizi citati:

- Bot di Azure: gli ambienti cloud offrono la flessibilità di implementare facilmente bot su diverse piattaforme di messaggistica, senza dover preoccuparsi di gestire l'infrastruttura sottostante. Inoltre, Azure fornisce servizi avanzati di AI e machine learning che consentono ai bot di comprendere il linguaggio naturale e di fornire risposte più intelligenti e personalizzate.

- Servizio app: l'utilizzo di un ambiente cloud per ospitare le applicazioni offre numerosi vantaggi in termini di scalabilità e disponibilità. Ad esempio, Azure consente di scalare automaticamente le risorse del servizio app in base alla richiesta di traffico, in modo che le applicazioni siano sempre disponibili e performanti.

- Bing Search: l'utilizzo di un servizio di ricerca come Bing Search offre vantaggi significativi in termini di velocità e precisione. Inoltre, Azure consente di personalizzare la ricerca utilizzando API e servizi avanzati di machine learning, in modo che i risultati della ricerca siano sempre pertinenti e pertinenti.

- Servizi cognitivi: l'utilizzo di servizi di intelligenza artificiale come il riconoscimento del testo da un'immagine offre numerosi vantaggi in termini di automazione dei processi e miglioramento dell'esperienza utente. Ad esempio, Azure consente di utilizzare l'API di Visione artificiale per identificare gli oggetti nelle immagini e di utilizzare l'API di Riconoscimento vocale per trasformare il parlato in testo.

- Azure SQL: l'utilizzo di un database SQL come Azure SQL offre numerosi vantaggi in termini di prestazioni, scalabilità e sicurezza. Ad esempio, Azure SQL offre funzionalità avanzate di scalabilità orizzontale e verticale, consentendo di gestire grandi quantità di dati in modo efficiente e affidabile.

In generale, l'utilizzo di un ambiente cloud come Azure offre numerosi vantaggi in termini di riduzione dei costi, flessibilità, sicurezza e prestazioni, consentendo di concentrarsi sullo sviluppo dell'applicazione e sul miglioramento dell'esperienza utente, senza doversi preoccupare dell'infrastruttura sottostante.

## 💻 Arhitettura del sistema 💻 

![Architettura del sistema](https://github.com/BookManagerProject/.github/blob/main/image/architettura.png?raw=true)

L'immagine di cui sopra ci mostra l'architettura del sistema Book Finder, in cui vengono riassunte tutte le interazioni tra le componenti software.

La lettura del diagramma può iniziare dalla Azure Web App: La quale è il cuore pulsante dell'Azure Bot, esso è il suo endpoint di messagistica che risponde ale richieste ricevute attraverso Telegram

I comandi vengono intepretati da LUIS il quale è stato addestrato a risponere ad una serie di comandi.

Tra le funzionalità offerte c'è la ricerca dei libri che sfrutta i servizi di riconoscimento immagine per cercare un libro dalla sua copertina, o in alternativa tramite testo il quale viene ricercato su Bing e poi dati in pasto alle Google Book API per migliorare l'area di ricerca

Gli utenti del sistema possono salvare i libri nei preferiti e qui entra in gioco Azure SQL che memorizza le preferenze di ricerca e i prferiti degli utenti

Infine, App Spring di Azure espone un sito web su cui è possibile consultare le classifiche dei libri preferiti dagli utenti e i libri cercati con più frequenza


### 🔎 Tipi di risorse utilizzate 🔎
- Bot di Azure
- Servizio app
- App Spring di Azure
- Bing Search
- Language Understanding (LUIS)
- Account multi-servizi Servizi cognitivi
- Azure SQL

### 🛠 Installazione e manule d'uso 🛠

L'installazione dei servizi creati sono ritovabili nelle repo dedicate:

- [Bot Telegram (BookFinderBot)](https://github.com/BookManagerProject/BookFinderBot)
- [Sito Web (BookFinderWebSite)](https://github.com/BookManagerProject/BookFinderWebsite)

## 📸 Screenshoot del sistema 📸

### BookFinderWebSite
#### Libri più cercati
![Libri più cercati](https://github.com/BookManagerProject/.github/blob/main/image/libri_pi%C3%B9_cercati.png?raw=true)
#### Libri preferiti
![Libri preferiti](https://github.com/BookManagerProject/.github/blob/main/image/libri_preferiti.png?raw=true)
* **
### Book Finder Bot

WIP...
