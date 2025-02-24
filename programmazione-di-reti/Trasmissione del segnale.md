Regola generale: più complessa l'informazione, più larga la banda.

### Transizione logico/digitale

- **ADC** (*Analogic to Digital Conversion*)
	- il segnale digitale viene rappresentato in forma binaria, utilizzando i bit 0/1
- **DAC** (*Digital to Analogic Conversion*)
	- il segnale analogico è una funzione del tempo

### Analogico to Digitale

Processo che prende senso quando è reversibile
1. **Campionamento**
	- **misuro** periodicamente il segnale e ci associo dei numeri
	- occorre trovare un corretto $T_s$: *periodo di campionamento*
	- possibili problemi:
		- **over-sampling**
			- campiono più di quanto necessario
			- overhead di memoria
		- **sub-sampling**
			- campiono meno del necessario
			- troppa perdita di informazione
	- **Teorema di Shannon-Nyquist**
		- per non perdere informazione (quindi mantenere l'irreversibilità del processo), devo avere che
			- $f_s \geq 2f_M$, dove $f_M \coloneqq$ *frequenza massima del segnale*
			- Tempo di campionamento minimo: $$T_s = \frac{1}{f_s} \lt \frac{1}{2f_M}$$
2. **Quantizzazione**
	- trasformazione dei campioni in sequenze binarie
	- un maggior numero di bit a disposizione permette una maggiore precisione nella rappresentazione dei campioni

### Perché passare al digitale?

1. **Integrazione**
	- formato di informazione unificato
2. **Computazione**
	- I segnali possono essere elaborati da calcolatori digitali
	- **Modifica**
	- **Compressione**
	- **Cifratura**
		- Riservatezza, autenticazione