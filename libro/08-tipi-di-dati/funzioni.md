## Funzioni anonime

Elixir permette di raggruppare del codice all'interno di scatole chiamate funzioni
con cui possiamo passare del codice come fosse una stringa o un atom.

Le funzioni anonime si creano in questo modo: 

```
iex> add = fn a, b -> a + b end
#Function<12.71889879/2 in :erl_eval.expr/5>
iex> add.(1, 2)
3
iex> is_function(add)
true
```

Iniziano con `fn`, sono seguite dagli `argomenti` che indicano il codice da eseguire con `->` e si
chiudono con `end`.


Il numero degli argomenti di una funzione ne definisce il cosidetto "arity". L'arity non è 
altro che la quantificazione di quanti valori la funzione ha bisogno per funzionare.

Per esempio: 

```
# controlliamo se la funzione add accetta due argomenti
iex> is_function(add, 2)
true
# controlliamo che ne accetti solo uno
iex> is_function(add, 1)
false
```

Ed in questo modo possiamo distriminare le funzioni nei nostri programmi.

