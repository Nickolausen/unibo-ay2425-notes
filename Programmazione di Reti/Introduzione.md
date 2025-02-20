### Comunicazione

Condivisione di informazioni
- cosa serve per condividere?
	- un mezzo di trasporto delle informazioni

Limiti degli strumenti di comunicazione naturali 
- tempo
	- le informazioni svaniscono nel tempo
	- soluzione: meccanismi di registrazione
- spazio
	- non viaggia più lontano di tanto
### Telecomunicazione

Telecomunicazione
- **tele**: lontano
- tentativo umano di trasportare l'informazione sempre più lontano
- trasporto in termini di:
	- quantità
	- qualità
### Canale di comunicazione

Chi fa il trasporto? Un canale di comunicazione
Caratteristiche:
- monodirezionale
	- l'informazione viaggia in un solo verso
- bidirezionale
	- l'informazione può viaggiare in un entrambi i versi **contemporaneamente**
- punto-a-punto
- punto-a-multipunto

È necessario trovare degli strumenti per gestire i canali, anche su larga scala.
- **RETI**

Componenti di una rete
- dispositivi terminali
	- interfacce a disposizione dell'utente
		- pc, telefono, macchine...
- collegamenti
	- oggetti fisici impiegati per realizzare i canali
	- in alcuni casi non sono fisici
		- es: WiFi
- nodi di commutazione
	- elemento cruciale della rete
	- meccanismo di riuso dei canali
		- passa dal canale punto-a-punto tra due oggetti ad un sistema più complesso

>[!info] Nota bene
>È buona norma tenere distinti i concetti di *nodo di commutazione* e *terminale*.

Topologie di rete: descrizione geometrica della rete
* composta da:
	* nodi
	* rami — archi
* descrivibile tramite un **grafo**
- diverse tipologie:
	- maglia completa
		- ogni coppia di nodi è connessa
		- $N$ nodi richiedono $\frac{N(N-1)}{2}$ collegamenti
		- PRO
			- resistente ai guasti
		- CONTRO
			- costose e complesse
	- a stella
		- PRO
			- minor costo
		- CONTRO
			- minore resistenza ai guasti
	- anello
	- bus

Nel mondo reale, le reti sono **combinazioni**: tendono ad usare le maglie nel centro e le stelle nei nodi terminali.

Rete di accesso
- parte di rete più vicina all'utente

Rete di transito / trasporto (*backbone*)
- pochi nodi di commutazione
- collegamenti ad un numero limitato ad alta capacità