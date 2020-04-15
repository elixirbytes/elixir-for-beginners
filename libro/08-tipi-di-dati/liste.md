## Liste (linkate)

Le liste in Elixir si definiscono aprendo e chiudendo le parentesi quadre: `[]`. Esse possono contenere ogni genere
di dati (incluse funzioni), davvero tutto.

```
iex> [1, 2, true, 3]
[1, 2, true, 3]
iex> length [1, 2, 3]
3
```

Gli operatori ++ e -- servono a fare operazioni matematiche sulle liste.

```
iex> [1, 2, 3] ++ [4, 5, 6]
[1, 2, 3, 4, 5, 6]
iex> [1, true, 2, false, 3, true] -- [true, false]
[1, 2, 3, true]
```

Come detto in precendenza, usare operatori sulle liste non ne modifica il contenuto.
Nei precendenti esempi, ogni volta che usiamo l'operatore -- o ++, non siamo facendo
altro che creare una nuova lista con i nuovi elmenti risultanti dall'operazione.

Le liste hanno una "testa" ed una "coda". Elixir provvede anche a delle funzioni per leggere
testa e coda di una lista. Tali funzioni sono `hd` e `tl`.