# app-mwo-profile

> Stato: archiviato. Progetto del 2017, non più mantenuto. Legge i dati facendo
> scraping delle pagine del profilo su mwomercs.com, quindi con buona
> probabilità non funziona più con il sito attuale (non verificato). Resta
> online come riferimento.

Una piccola applicazione desktop per salvare le statistiche del tuo profilo di
**MechWarrior Online (MWO)**. Premi il pulsante di login, inserisci le
credenziali del tuo account MWO, e l'app legge le pagine del profilo su
mwomercs.com (dati base, mech, armi, mappe, modalità) e ti chiede dove salvare
il risultato in un file `.json`.

Fa lo stesso lavoro di [`api-mwo-profile`](https://github.com/XtremeAlex/api-mwo-profile),
ma in locale, senza passare dal servizio REST.

Da sapere, visto che è codice del 2017: il client HTTP disattiva la verifica
dei certificati TLS.

## Stack

- Java 8, interfaccia Swing (look and feel Nimbus)
- jsoup per leggere le pagine, json-simple e Gson
- Maven, packaging `jar`

## Build

```bash
mvn clean package
```

Il `jar` prodotto non dichiara la classe principale nel manifest e non include
le dipendenze: il modo più semplice per avviare l'app è lanciare
`com.xa.mwo_ui.Main` dall'IDE.

## Progetti collegati

- [`api-mwo-profile`](https://github.com/XtremeAlex/api-mwo-profile): il servizio REST
- `app-mwo-profile`: questa, l'applicazione desktop

## Licenza
Distribuito sotto licenza MIT. Vedi il file [`LICENSE`](LICENSE). Ogni riuso deve mantenere l'attribuzione all'autore.

## Contatti

Andrei Alexandru Dabija (XtremeAlex) · [alexdabi92@gmail.com](mailto:alexdabi92@gmail.com) · [2ad.bubume.it](https://2ad.bubume.it/) · [LinkedIn](https://www.linkedin.com/in/andrei-alexandru-dabija/) · [github.com/XtremeAlex](https://github.com/XtremeAlex)
