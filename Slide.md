# Esercizio Gruppo 1: Variabili e Scope

## Slide 1

1. Le Variabili:
- Immaginate una variabile non come un concetto matematico astratto, ma come una piccola scatola di cartone. 
    - L'Etichetta (Il Nome): Ogni scatola ha un'etichetta univoca appiccicata sopra (ad esempio: "nomeUtente" o "prezzoTotale"). 
    - Il Contenuto (Il Valore): Dentro la scatola mettiamo un'informazione (un numero, un testo o una lista della spesa). 
    - L'Utilità: Usiamo queste "scatole" per memorizzare dati che ci serviranno più avanti nel programma.
2. Lo Scope:
- Se la variabile è la scatola, lo scope è la stanza in cui quella scatola si trova. Lo scope determina la "visibilità" o l'accessibilità delle informazioni. 
    - Scope Globale (La Piazza del Paese): Se mettete una scatola nella piazza principale, chiunque in città può vederla e usarne il contenuto. In JavaScript, queste sono le variabili dichiarate fuori da ogni funzione o blocco di codice. 
    - Scope Locale (La vostra Camera da Letto): Se mettete una scatola in un cassetto della vostra camera, solo chi entra in quella specifica stanza può sapere cosa c'è dentro. Se qualcuno prova a cercarla dalla cucina, non la troverà: per lui quella scatola "non esiste". 
    - La Gerarchia: Una regola d'oro è che chi sta in una "stanza piccola" (scope figlio) può vedere le scatole nelle "stanze grandi" (scope genitore), ma non viceversa.

## Slide 2
1. Breve Storia: Dal Caos all'Ordine
- Fino al 2015 (standard ES6), esisteva solo var. Questo portava a situazioni spesso frustranti per gli sviluppatori:
 - L'aneddoto del "Leak" (Perdita di dati): Con var, una variabile creata dentro un blocco if o un ciclo for non restava chiusa lì dentro, ma "scappava" fuori (non avendo block-scope), rischiando di sovrascrivere altri dati per errore.

 - Ridichiarazioni selvagge: Potevi dichiarare la stessa variabile var dieci volte nello stesso punto senza ricevere alcun errore, rendendo il debugging un incubo.
2. Le Differenze Oggi
- Dal 2015 usiamo strumenti più precisi:
    - let (La Nuova Variabile): Risolve i problemi di var. È limitata al blocco in cui nasce (block-scoped) e non permette di essere usata prima della dichiarazione o di essere ridichiarata per errore.
    - const (La Scatola Sigillata): Si comporta come let, ma con una regola extra: una volta che le dai un valore, non puoi più cambiarlo (non è riassegnabile). 
    
    - Consiglio da Senior: Usate sempre const a meno che non siate sicuri che il valore debba cambiare; renderà il vostro codice molto più prevedibile
## SLIDE 4 Assegnazione e Dichiarazione
## Slide 3 
1. JavaScript è "loosely typed" (tipizzato dinamicamente): non dobbiamo dire alla scatola cosa conterrà, lo capirà lei da sola al momento dell'assegnazione. I principali tipi sono:
    - Number: Numeri interi o decimali (es: 5 o 3.14).
    - String: Testo racchiuso tra virgolette o apici (es: "Ciao").
    - Boolean: Solo due valori possibili, true (vero) o false (falso).
    - Undefined / Null: Quando la scatola è vuota o il valore è intenzionalmente nullo.
    - Strutture complesse: Possiamo anche salvare Array (liste di dati in []) o Object (modelli di oggetti reali con proprietà).

## Slide 4: L'armadio delle Scope
1. Cos’è lo Scope? (Spiegazione per scimmie 🐒)
- Lo scope è semplicemente il territorio in cui una variabile "vive" ed è visibile.
Immaginate che ogni variabile sia una banana.
    - Se la banana è nel vostro raggio visivo, potete prenderla e mangiarla (usare il suo valore).
    - Se la banana è fuori dal vostro territorio, per voi non esiste: se provate a cercarla, la vostra "mente da scimmia" (il browser) andrà in confusione e restituirà un errore.
2. Scope Globale: La Grande Radura 🌴
    - Lo scope globale è come la piazza principale della giungla.
        - Le variabili dichiarate qui (fuori da ogni funzione o blocco) sono accessibili da chiunque e ovunque nel programma.
        - Tutti gli script e le funzioni della pagina possono vedere e usare queste variabili.
        - Attenzione: Se tutti possono toccare la stessa banana, è facile che qualcuno la rubi o la rovini per sbaglio!
3. Scope Locale: La Caverna della Funzione 🦇
    - Ogni volta che create una funzione, create una "caverna" privata.
    - Le variabili create dentro una funzione sono locali: esistono solo lì dentro.
    - Le scimmie che stanno fuori dalla caverna non possono vedere cosa succede dentro, né possono prendere le banane nascoste all'interno.
    - Una volta che la funzione ha finito il suo compito, la "caverna" sparisce e le sue banane locali vengono rimosse.
4. Scope di Blocco: Il Piccolo Cestino { } 🧺
    - Questo è il territorio più piccolo di tutti, delimitato dalle parentesi graffe { } (che troviamo ad esempio negli if o nei cicli).
    - Se usate let o const dentro queste graffe, la variabile rimane chiusa nel "cestino" e non è accessibile all'esterno.
### Slide 5 best practices per i nomi delle variabili