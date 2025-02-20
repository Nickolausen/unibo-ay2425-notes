### Sistema informativo
Insieme di procedure che permettono di gestire informazioni utili per un progetto aziendale.
- Competenze informatiche
- Competenze sulla vita di un'azienda

Base di dati — *database*
- Parte del sistema informativo aziendale. 
- Tutti i dati di un processo aziendale vengono - in qualche modo - memorizzati da qualche parte
- Definizione: collezione di dati di interesse per una o più applicazioni

**Modello di rappresentazione**
- ***Modello relazionale***
	- Più diffuso
	- Affrontato nel corso
	- Linguaggio di interrogazione standard: SQL

### **DBMS** (*Database Management System*)
Software che gestisce l'accesso ai dati, garantendo alcune funzionalità.

**OLTP** (Online Transactional Processing)
- oggetto di questo corso
- applicazioni in cui il modello relazionale è maggiormente diffuso
- gestione di dati "recenti"
- le operazioni più frequenti sono **ordinarie**
- elevata velocità di esecuzione
- operazioni equamente distribuite tra quelle di lettura e scrittura

**OLAP** (Online Analytical Processing)
- applicazioni a supporto delle decisioni strategiche aziendali
- grandi quantità di dati, specialmente storici
- operazioni di alto livello
- tempi di reazione lunghi
- operazioni di lettura
	- interrogo il db per estrarre informazioni statistiche
- operazioni offline
- architettura utilizzata: Datawarehouse

### Attori principali

- **DBA *(Data Base Administrator)***
	- crea gli oggetti logici necessari alle applicazioni
	- garantisce la sicurezza e l'integrità del DB
	- monitora prestazioni del DB
- **Data Base Designer**
	- colui che progetta il DB
	- ascolta l'analisi dei requisiti e concettualizza il DB di conseguenza
- **Software Engineer**
	- i primi a determinare le esigenze di un utente
- **Utenti finali**
	- Naive End User
		- NOOB dei DB
	- Sophisticated End User
		- PRO dei DB