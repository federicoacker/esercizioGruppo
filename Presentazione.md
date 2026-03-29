
# Presentatore 1 (Filippo):
    Presentazione Generale
	Salve siamo il gruppo 1 e oggi tenteremo di spiegare, in maniera tale che anche un scimmia lo capisca, cosa sono le variabili e il concetto di scope in JavaScript.
	Iniziamo cercando di capire cosa sia una variabile, si puo definirla una scatola, un contenitore il cui compito è conservare informazioni che il programma utilizzerà in futuro. Ognuna di queste scatole ha due elementi chiave, il nome, che ci permette di ritrovarla quando sarà necessaria e il contenuto, ovvero, l'informazione che andremo ad utilizzare.
	L'utilità delle variabili, è appunto quella di salvare dati, facendo si che siano a disposizione quando saranno necessari più avanti nel codice, dando anche la possibilità in alcuni casi di modificarne il contenuto durante l'esecuzione.
    
# Presentatore 2 (Alessia):
	Non tutte le variabili si comportano allo stesso modo. In passato var causava diversi problemi, perchè una variabile rimaneva accessibile anche fuori dal blocco in cui era stata dichiarata.
	Per questo sono stati introdotti let e const: entrambi limitano la variabile al blocco logico, e const viene usato quando il valore non deve essere modificato dal programma.
	il nostro esperto Samuel consiglia di dichiarare sempre prima con const e usare let quando è necessaria una modifica durante lo svolgimento del programma.

# Presentatore 3 (Sara):
	Il ciclo di vita di una scim... variabile inizia con la dichiarazione, cioè il momento in cui viene creata usando const o let. Questo equivale a chiedere al computer di creare una nuova scatola.
	Successivamente avviene l’inizializzazione, con l’assegnazione del primo valore.
	Con const, queste due fasi devono coincidere.
	Infine può esserci una riassegnazione, cioè il cambiamento del valore, possibile solo nel caso di let. 

# Presentatore 4 (Francesco):
	Dentro una variabile possiamo memorizzare diversi tipi di dati. In JavaScript il tipo viene identificato automaticamente, quindi non va dichiarato esplicitamente. Possiamo avere numeri come interi e decimali, stringhe che sono testi racchiusi tra virgolette o apici, valori booleani che sono solo true o false e anche strutture più complesse come oggetti e array, inoltre ci sono valori speciali che indicano che la scatola è vuota che sono undefined e null.
	Anche se un array sembra diverso da un oggetto, in JavaScript viene comunque trattato come un oggetto speciale. Per questo typeof restituisce "object". Per distinguere correttamente un array si usa "Array.isArray()"

# Presentatore 5 (Federico):
	Ora che abbiamo le variabili, dobbiamo capire dove possono essere usate: questo è lo scope.
    Abbiamo tre tipi di scope:
    Globale,
    Locale ( o di funzione)
    e di Blocco.
    Lo scope globale rende una variabile accessibile ovunque nel programma.
	Lo scope locale, invece, ne limita la visibilità e accessibilità alla funzione in cui è stata dichiarata.
    Il vecchio var famosamente aveva scope globale o di funzione e quindi se dichiarato in un blocco era leggibile e modificabile anche al di fuori di esso.
	let e const invece rispettano lo scope di blocco, che restringe la visibilità al blocco logico in cui la variabile viene dichiarata.
	In generale, uno scope interno può vedere e modificare variabili in quello esterno, ma non il contrario.
	Ad esempio

```
let globalScimmia = "orangutan";
	if(true){
		globalScimmia = "sapiens";
	}
console.log(globalScimmia);

```		

	Ci restituirà "sapiens";
    In JavaScript capire lo scope è fondamentale, perché determina dove una variabile esiste e può essere letta o modificata.

# Presentatore 6 (Giulio):
	Per concludere, anche i nomi delle variabili hanno le loro regole di stile.
    Nei nomi delle variabili sono consentiti solo lettere, numeri, gli underscore e il simbolo del dollaro.
    Nota bene: I nomi in javascript non possono mai iniziare con un numero o utilizzare parole riservate da javascript.
    Un nome descrittivo aggiunto all'utilizzo del camelCase rende il codice più chiaro e leggibile a lettori esterni e ignari delle leggi della giungla o anche agli esperti, quindi non siate pigri e non usate nomi come x o data.	
	Inoltre JavaScript è case sensitive, quindi un nome in minuscolo e uno in maiuscolo non vengono considerati uguali.
	Per le costanti si usa spesso lo snake_case con parole in maiuscolo, ad esempio NUMERO_MASSIMO_SCIMMIE.
	Grazie per la vostra attenzione e speriamo che dopo questa breve presentazione siate passati dall'essere delle semplici scimmie ad essere delle scimmie che sanno cosa sono le variabili.
















	