### ITU: Tassonomia dei servizi

Ente certificato per la classificazione dei servizi.
#### Servizi interattivi
- I due soggetti coinvolti nella comunicazione interagiscono tra di loro
- Tipologie:
	- **sistemi di conversazione**
		- scambio informativo bidirezionale
		- tempo reale
		- esempio:
			- file system remoto
			- telefonia
	- **sistemi di messaggistica**
		- scambio informativo bidirezionale
		- tempo differito
		- esempio:
			- scambio informativo bidirezionale
	- **sistemi di consultazione**
		- flusso controllato dall'utente
		- esempio:
			- Web
			- YouTube

#### Servizi distributivi
- Qualcuno distribuisce l'informazione e gli altri ascoltano
- Tipologie:
	- **senza controllo di presentazione**
		- l'utente non controlla niente sul ricevimento dell'informazione
		- esempio:
			- radio
	- **con controllo di presentazione**
		- l'utente può compiere decisioni **locali**
		- esempio:
			- televideo
#### Servizi multimediali
- servizio monomediale
	- una sola tipologia di informazione
		- com'è costruito il segnale
- servizio multimediali
	- diverse tipologie di informazioni
	- es: chiamata su Teams
#### Qualità del servizio

Errori semantici: modifica il contenuto di un messaggio
Errori temporali: ritardi nel tempo

Trasparenza semantica: no errori temporali, sì errori semantici
Trasparenza temporale: no errori semantici, sì errori temporali

- È inevitabile un minimo di ritardo nella trasmissione di un messaggio.
- È più facile **recuperare errori semantici** rispetto ad **errori temporali**.

Indicatori di QoS (Quality of Service)
- Applicazioni non real-time
	- trasparenza semantica
- Applicazione real-time
	- trasparenza temporale
	- servizi isocroni
		- richiedono trasparenza temporale e corretta interpretazione delle informazioni

**Jitter**
- variazione del ritardo
- fastidioso nei video

Per compensare gli errori della comunicazione, si può intervenire:
- sulla rete
- sui terminali

Mettere insieme tanti servizi diversi sulla stessa rete è **difficile**.
- Servizi diversi = Requisiti diversi
- Problema tutt'ora irrisolto