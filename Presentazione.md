# Presentatore 1: (Dovrà anche presentare l'inizio)
    Il concetto di Variabile (Slide 3) 
    "Iniziamo il nostro viaggio cercando di capire cos'è una variabile. In JavaScript, non dovete pensare a concetti matematici astratti, ma semplicemente a una scatola di cartone. Una variabile è un contenitore fisico progettato per conservare informazioni che ci serviranno in futuro nel nostro programma. Ogni scatola ha tre elementi chiave: l'Etichetta, ovvero un nome univoco (come 'nomeUtente') per poterla ritrovare; il Contenuto, che è l'informazione vera e propria memorizzata all'interno; e infine l'Utilità, perché ci permette di salvare dati adesso per riutilizzarli in altri punti della giungla del codice." 
# Presentatore 2: 
    Dal Caos all'Ordine (Slide 4) 
    "Ma non tutte le scatole sono uguali. In passato vivevamo nel 'Caos di var': prima del 2015, questo strumento causava molti problemi, come i 'leak' di dati dove le variabili scappavano dai blocchi logici sovrascrivendo altri dati per errore, o le 'ridichiarazioni selvagge' che rendevano il debugging un incubo. Oggi usiamo la Precisione di ES6 con due strumenti specifici: let, la nuova variabile confinata nel blocco in cui nasce, e const, la 'scatola sigillata'. Una volta riempita, il valore di const è bloccato e non può essere cambiato. Il consiglio del nostro esperto Samuel è di usare sempre const, a meno che non siate certi che il valore debba cambiare." 
# Presentatore 3: 
    Ciclo di Vita della Scatola (Slide 5) 
    "Vediamo ora come nasce e come cambia una scatola attraverso il suo ciclo di vita. Tutto inizia con la Dichiarazione: usiamo let o const per dire al computer che ci serve una scatola nuova; in questa fase la scatola esiste ma è vuota, ovvero undefined. Segue l'Inizializzazione, il momento magico in cui inseriamo il primo valore, la nostra 'prima banana'. Ricordate: con const dovete farlo subito, non può restare vuota ! Infine abbiamo l'Assegnazione, dove usiamo il simbolo = per cambiare il contenuto. Potete farlo all'infinito con let, ma mai con const, perché quel valore rimane lì per sempre." 
# Presentatore 4: 
    I Tipi di Dato (Slide 6)
    "Cosa possiamo mettere dentro queste scatole? JavaScript è a tipizzazione dinamica, il che significa che la scatola capisce da sola cosa contiene senza doverlo dichiarare. Possiamo inserirci numeri interi o decimali (Number), oppure del testo racchiuso tra virgolette (String). Esistono i Boolean, che rappresentano solo due strade: true o false. Se la scatola è intenzionalmente vuota, parliamo di Undefined o Null. Infine, per le scimmie più esperte, ci sono le Strutture Complesse come gli Array (liste di dati) o gli Oggetti, che sono modelli con proprietà specifiche." 
# Presentatore 5: 
    Il Territorio dello Scope (Slide 7, 8, 9) 
    "Ora che abbiamo le scatole, dobbiamo sapere dove vivono: questo è lo Scope. Lo Scope Globale è la 'Grande Radura', la piazza principale della giungla dove tutti possono vedere e toccare le banane, ma con il rischio che qualcuno le rovini per sbaglio. Se cerchiamo privacy, entriamo nella 'Caverna della Funzione' (Scope Locale), dove le variabili esistono solo all'interno e sono invisibili a chi sta fuori. Esiste anche il 'Piccolo Cestino' (Scope di Blocco) per let e const. La regola d'oro della gerarchia è: chi sta in una stanza piccola può vedere fuori nelle stanze grandi, ma chi sta fuori non può mai guardare dentro !" 
# Presentatore 6: 
    Il Galateo del Branco (Slide 10) 
    "Per concludere, ogni buona tribù ha delle regole di stile per non far arrabbiare il browser. Usiamo il camelCase: scrivete tutto attaccato iniziando la seconda parola con la maiuscola, come 'contaBanane'. Non siate scimmie pigre: evitate nomi generici come 'x' e usate nomi descrittivi come 'utenteLoggato'. Ricordate che JavaScript è case-sensitive: 'banana' e 'BANANA' sono due scatole diverse. Infine, per le Costanti Forti, ovvero valori sacri che non cambieranno mai, scrivete tutto in MAIUSCOLO con l'underscore, come 'NUMERO_MASSIMO_SCIMMIE'. Grazie a tutti e buona sopravvivenza nel codice!"


# Presentatore 1:
	Iniziamo cercando di capire cosa sia una variabile, si può definirla una scatola,
	un contenitore il cui compito è conservare informazioni che il programma utilizzerà in futuro
	ognuna di queste scatole ha due elementi chiave,
	il nome, che ci permette di ritrovarla quando sarà necessaria e
	il contenuto, ovvero, l'informazione che andremo ad utilizzare.
	L'utilità delle variabili, è appunto quella di salvare dati, facendo si che siano
	a disposizione quando saranno necessari più avanti nel codice, dando anche 
	la possibilità in alcuni casi di modificarne il contenuto durante l'esecuzione.
# Presentatore 2:
	Non tutte le variabili si comportano allo stesso modo. In passato var causava diversi problemi,
	perché una variabile poteva restare accessibile anche fuori dal blocco in cui era stata dichiarata.
	Per questo sono stati introdotti let e const: let limita la variabile al blocco logico,
	mentre const viene usato quando il valore non deve essere modificato dal programma.
	il nostro esperto Samuel consiglia di dichiarare sempre prima con const e usare let solo quando è necessaria una modifica.

