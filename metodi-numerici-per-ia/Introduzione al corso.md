Obiettivo del corso e ambito di studio: analisi numerica
1. Identificare un problema reale
2. Crearci un modello matematico **continuo**
3. **Discretizzare** il problema (es. da integrale a sommatoria, da derivata a rapporto incrementale) per renderlo risolubile al calcolatore
4. Implementare l'algoritmo al calcolatore
5. **Interpretare e analizzare** i risultati

Diversi possibili tipi di errori:
- errori di modello
	- 
- errori numerici
	- 
- errori nei dati
	- acquisizione e/o trasmissioni di dati
- errori di arrotondamento
	- i nostri algoritmi lavorano su numeri finiti, possono quindi propagare e amplificare un errore

### Def: Problema numerico
Descrizione chiara e non ambigua di una relazione funzionale tra dati di input e risultati desiderati di output

Problemi:
- *diretti*
	- $y = f(x)$
	- $x$ è noto, $f$ è nota; $y$ è incognita
	- conosco gli input, conosco la relazione ma non è noto l'output
	- esempio: valutazione di una funzione in un punto, calcolo di un integrale
- *inversi*
	- $y = f(x)$
	- $y$ è nota, $f$ è nota; manca $x$
	- conosco gli output, so come arrivarci ma non è noto l'insieme di input
	- esempio: risoluzione di un'equazione, risoluzione di un sistema lineare
		- $y=2$,  $f(x)=3x+1 \Rightarrow \quad 2=3x+1,\quad x=\frac{1}{3}$,
- *di identificazione*
	- $y=f(x)$
	- conosciamo $y, x$, non è nota $f$
	- esempio: interpolazione dei dati 
### Def: Algoritmo di un problema numerico
Successione ben definita di operazioni che, in un numero finito di passi, processa gli input e produce gli output.

## Introduzione all'Intelligenza Artificiale
Non è una cosa recente: come ambito di ricerca e come concetto nasce con l'informatica. 

Test di Turing: 
- prova per capire se una macchina riesce ad emulare correttamente l'intelligenza umana
- un soggetto si preoccupa di fare delle domande, che vengono risposte da due soggetti
	- una macchina
	- un uomo
- chi fa le domande non sa da dove provengono le risposte
- se la risposta umana è indistinguibile dalla risposta artificiale, allora l'IA ha raggiunto un buon livello

In generale
- tentativo di rappresentare digitalmente l'intelligenza umana
- processiamo tanti dati in poco tempo
	- i computer possono scalare nel tempo, migliorare con le tecnologie
- si compone di tante ramificazioni
	- noi: ML (*Machine Learning*), DL (*Deep Learning*)

## Machine Learning

Idea: la macchina impara da sola.
Noi: predisponiamo l'impalcatura per rendere possibile ciò.

Ci sono diversi problemi facilmente risolvibili dall'intelligenza artificiale
- Riconoscimento delle immagini
- Riconoscimento vocale
- Previsione del traffico
- Raccomandazioni sui prodotti
- Auto a guida autonoma
- Filtraggio di posta indesiderata e malware

**Apprendimento supervisionato** \[**NOI**\]
Un dataset è etichettato, quindi l'apprendimento è guidato

**Apprendimento semi-supervisionato**
Mix dei due

**Apprendimento non supervisionato**
Clustering: cercare dati simili, struttura tra i vari dati

Un dataset va diviso in 3 parti:
- **training set**
	- 80% circa dei dati raccolti in partenza
	- dati usati per l'addestramento
- **validation set**
	- impostare e aggiustare in maniera corretta i parametri del nostro modello
- **testing set**
	- rappresentativo del mondo reale su cui il nostro modello deve operare

### Task

**Classificazione e rilevamento**
Output: classe
- rilevamento spam nelle email — problema binario, 2 classi (SPAM / NO SPAM)
- riconoscimento facciale — problema multiclasse
- diagnosi medica — 
	- tumore maligno/benigno
	- problema binario (se assumo che un tumore esista già)
	- problema multiclasse se nessuna assunzione viene fatta a priori

**Regressione**
Output: numero $\in \mathbb{R}$
- problemi di stima
	- stima di un'altezza dato un peso
	- stima di un prezzo nel mercato immobiliare
	- previsione dell'energia prodotta da un sistema

**Clustering**
Apprendimento **unsupervised**
- organizzare i dati per similarità
- spesso non si sa cosa si cerca
- esempio: raggruppamento di utenti in base alle loro preferenze 

## Artificial Neural Networks
