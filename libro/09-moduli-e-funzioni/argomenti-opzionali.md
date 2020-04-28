## Argomenti opzionali

Come abbiamo visto, i moduli raggruppano una serie di funzioni che hanno uno scopo comune.
Abbiamo anche visto come le funzioni abbiano la cosidetta `arity`, ovvero il numero di argomenti
accettati. Le funzioni in Erlang/Elixir si sono definite da <Nome modulo>.<nome funzione>/<arity).

Per esempio la funzione nativa per recuperare il primo elemento di una lista, 
può essere chiamata con `Kernel.hd/1` dove 1 è la lista che passiamo come argomento.

Le funzioni che definiamo nei nostri moduli non sono da meno. Ma l'`arity` presenta 
anche delle eccezioni: argomenti opzionali.

Facciamo un esempio di una funzione per la somma, la chiameremo `incrementa`. 

La funzione incrementa deve incrementare di 1 un certo numero, ma non sempre, diciamo il 99% delle volte.
Come fare questo?  

Potremmo definire due funzioni, dato che in Elixir una funzione può essere definita diverse volte 
con diverse arity/tipi di dati che accetta.

```
defmodule Sommatoria do
  def incrementa(numero) do
    numero + 1
  end

  def incrementa(numero, valore) do
    numero + valore
  end
end
```

E questo funzionerebbe bene, ma se volessimmo definirla solo una volta potremmo anche scrivere il seguente formato:

```
defmodule Sommatoria do
  def incrementa(numero, valore \\ 1) do
    numero + valore
  end
end
```

Gli argomenti opzionali sono definiti da <nome di variabile> doppi backslash // ed il valore di default.
In questo modo elixir controllerà che chiamiamo la funzione con o senza definire quel valore
ed andrà ad utilizzare quello di default se necessario.


