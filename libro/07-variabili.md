# Variabili 

*Dare nomi ai dati*

Per fare riferimento a specifici dati nei nostri programmi, usiamo le variabili.

Ogni linguaggio di programmazione che useremo permette di creare variabili.

In Elixir possiamo assegnare un nome ad alcuni dati usando l'operatore `=`, in questo
modo:

```elixir
number = 1
```

Così facendoo *assigneremo* al nome `number` il dato che è il numero
`1`. Da questo momento in poi possiamo riferirci al numero `1` con `number`.

Per esempio possiamo mostrare a schermo il numero in questo modo:

```
number = 1
IO.inspect(number)
```

Una cosa importante da notare è che la variabile non è il nummero in sè, ma solo il
nome in cui in quel "contesto" ci riferiamo al numero `1`.

Un'altra cosa importante da notare è che in Elixir, 
l'operatore `=` non "assegna" il valore `1` a `name` ma crea quello che si chiama "pattern match".

Il pattern matchin è il riconoscimento di pattern all'interno di struttura dati 
astratta. Per esempio: 

`{a, b} = {1, 2}` è un pattern che può avere un match

1. `{` corrisponde all'apertura di `{` dall'altra parte dell'`=`
2. `a` è una variabile e quindi può avere valore `1`
3. la virgola corrisponde alla virgola
4. `b` corrisponde
5. la chiusura `}` corrisponde

Elixir farà tutte queste valutazioni per noi e, nel caso di successo, 
assegnerà ad a il valore 1 ed a b il valore 2.

Questo è esattamente il principio per cui `number = 1` funziona nel nostro esempio precedente.
