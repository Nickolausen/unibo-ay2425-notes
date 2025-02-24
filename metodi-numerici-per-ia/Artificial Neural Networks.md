
> Una rete non apprende in un passaggio singolo i pesi delle sinapsi

Addestramento di una rete:
- step iterativo
	- sottoinsieme dei dati di training (batch)
	- lo si fornisce alla rete
- ad ogni step iterativo occorre minimizzare l'errore
- quando tutto il dataset è stato testato, si dice che è finita un **epoca**.

### Funzioni di loss / obiettivo
- Funzione derivabile
- Segnala "quanto stiamo andando male"
	- misura l'errore rispetto all'etichetta prevista
- Minimizzare:
	- trovare il minimo della funzione

> [!info] In generale 
> Apprendere = Minimizzare la *funzione di loss*

Problemi di classificazione
- binaria
	- cane o gatto, tumore o non tumore...
	- funzione BCE (Binary Cross-Entropy)
	- $$
		BCE = -y_i \cdot \log \hat{y_i} - (1-y_i)\cdot\log(1-y_i)
	 $$
	- Se dato appartiene a classe 0, la parte $-y_i \cdot \log \hat{y_i}$ si annulla
		- sopravvive l'ultimo fattore $-\log(1-y_i)$, che restituisce un valore vicino allo 0
		- se la predizione è giusta, rimane $-\log(1) = 0$
	- Se dato appartiene a classe 1, la parte di destra scompare
		- rimane $-y_i\cdot\log\hat{y_i} \rightarrow -\log1$
	- è derivabile
- multiclasse
	- funzione CCE (Categorical Cross-Entropy)
	- $$
		CCE=-\sum_i{y_i\cdot\log\hat{y_i}}
	$$
Ricordiamo che 
- $\hat{y_i}$: i-esimo valore emesso dalla rete (predizione)
- $y_i$: etichetta associata

#### Softmax
- I valori di output di una rete non sono sempre compresi tra 0 e 1;
	- vengono prima trasformati in probabilità da una funzione apposita — in modo che la loro somma dia 100%
- funzione continua e differenziabile
- $$
	p_i = \frac{e^{a_i}}{\sum_k{e^{a_k}}}
$$
#### Architettura delle reti neurali
Le cose si complicano quando le reti devono elaborare delle immagini
- dati ad alta dimensionalità

## CNN (Convolutional Neural Network)

MLP
- MultiLayer Perceptron
- Più layer di neuroni
	- ogni neurone è collegato a tutti quelli precedenti

CNN
- reti designate per processare immagini
- idea: organizzare i neuroni in 3 dimensioni
	- una per canale di colore (R, G, B)