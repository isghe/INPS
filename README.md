// https://www.inps.it/nuovoportaleinps/modelliNuovo/assets/js/app.js

Questo è il codice sorgente di una parte del sito https://www.inps.it , in cui, in primissima analisi, si riscontrano gravissime incompetenze già a partire dalla riga 62, laddove viene definita la funzione:
```
function wait(ms) {
    var start = new Date().getTime();
    var end = start;
    while (end < start + ms) {
        end = new Date().getTime();
    }
}
```

invocata alla riga 1574:

```
                wait(1000);
```
