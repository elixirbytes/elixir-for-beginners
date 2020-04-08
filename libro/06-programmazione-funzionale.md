# Programmazione funzionale (FP)

Cosa è la programmazione dei computer?

Da wikipedia:
`
La programmazione, in informatica, è l'insieme delle attività e tecniche che una o 
più persone specializzate, programmatori o sviluppatori (developer), svolgono per
creare un programma, ossia  un software da far eseguire ad un computer, 
scrivendo il relativo codice sorgente in un certo linguaggio di programmazione.
`

Di linguaggi di programmazione ne esistono davvero tanti, e di solito rispecchiano 
il modo di pensare delle persone che li hanno ideati, ed il problema che queste persone
stavano cercando di risolvere.

Ogni linguaggio cerca, a suo modo, di risolvere al meglio alcune problematiche
computazionali seguendo degli schemi. Questi possono essere più o meno flessibili
ma nessuno è perfetto, alcuni sembrano più intuitivi di altri o più familiari ma
non sempre a colpo d'occhio si è nel giusto.

Si chiama funzionale perché il suo concetto di base risiede nella funzione, 
ma nel senso matematico del termine. Le funzioni dei linguaggi procedurali o 
imperativi sono realmente delle procedure piuttosto che delle funzioni e svolgono
in questo senso delle pure direttive di calcolo. La funzione matematica invece non 
esegue calcoli ma si limita a mappare valori e viene definita infatti, 
come una: trasformazione o mappa od operatore; 

Per esempio:

`y = f(x)`

La funzione qui sopra non fa altro che applicare una trasformazione a X. Se dovessimo concretizzare
la funzione teorica qui sopra con qualcosa di più pratico potremmo scrivere: 

`f = fn x -> x + 1 end # creiamo la nostra variabile astratta`

`x = 1 # assegnamo a x il valore 1`

`y = f.(1) # <-- quindi 2`


Questa funzione chiamata `y` non fa altro che prendere un argomento di nome `x` ed aggiungerci `1`

La funzione serve a mappare i valori dati come argomenti, trasformarli all'intero della funzione stessa
chiamata `body` ed assegnarli ad una variabile (nel nostro caso `y`)

Possiamo immaginare i nostri programmi Elixir come una serie di funzioni che chiamano 
l'un l'altra fino a produrre quello che è stato inteso dal programmatore.

Quello che facciamo quando scriviamo un programma Elixir, è di 
dividere il nostro problema in piccole parti (funzioni) che trasformano
i dati fino a raggingere il risultato finale. Per questo motivo è importante
dare alle funzioni nomi che abbiano un senso, serve che indichiamo 
ai nostri colleghi quale parte del problema stiamo processando con la funzione
che abbiamo sott'occhio in quel mommento.
