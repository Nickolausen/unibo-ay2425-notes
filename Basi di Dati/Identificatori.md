Obiettivo: identificare in modo univoco ogni singola istanza di entità

Ogni entità DEVE necessariamente avere almeno un identificatore

Un identificatore deve:
- essere univoco
- godere della **proprietà di minimalità**
	- non deve esistere alcun suo sottoinsieme che può funzionare come identificatore

Per definirlo:
- **identificatore interni**
	- costituito solo da attributi dell'entità in oggetto
	- es: matricola per studente, CF per persona...
- **identificatori esterni**
	- importati da altre entità
- **identificatore misto**
	- esterno + interno

Identificatore
- **semplice**
	- un singolo attributo
- **composto**
	- più attributi

Preferibile sempre scegliere **identificatori candidati** a **numeri progressivi** (*quando possibile*).

Aggiungere attributi ad un identificatore rilassa il vincolo di unicità: per esempio, se ad un identificatore costituito da due attributi ne aggiungo un terzo, basta che uno dei tre cambi che cambia l'istanza a cui si sta facendo riferimento.

>[!info] Spin-off
> In generale i dati ridondanti non vengono indicati in uno schema E/R, poiché possono essere calcolati in un secondo momento.

