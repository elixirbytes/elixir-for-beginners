## Moduli e funzioni 

Ora che abbiamo visto a cosa servono i tipi di dati, structs e quali dati abbiamo a disposizione, vediamo
quali strumenti abbiamo per manipolarli. 

In Elixir raggruppiamo le funzioni all'interno di moduli. Un modulo può essere creato
usando la macro `defmodule` (che è di per sè una funzione, ma un pò speciale e che vedremo in seguito).


```
iex> defmodule Matematica do
...>   def somma(a, b) do
...>     a + b
...>   end
...> end

iex> Matematica.somma(1, 2)
3
```

Il più delle volte i moduli sono creati uno per file, in questo modo usarli e modificarl irisulterà più semplice.
Per esempio, il nostro modulo `matematica` potrebbe essere chiamato `matematica.ex`. 

All'interno dei moduli, che poi sono le "scatole" che contengono funzioni 
relative ad uno stesso argomento o operazione di business, troviamo la possibilità
di creare funzioni con la dicitura `def`.

Nell'esempio precendente, la "somma" era eseguita dalla funzione di nome `somma`


```
iex> defmodule Matematica do
...>   def somma(a, b) do <<<--------la nostra funzione 
...>     a + b            <<<--------------------------
...>   end                <<<--------------------------
...> end

iex> Matematica.somma(1, 2)
3
```

Le funzioni appartenenti ai moduli possono essere usate in diversi modi. Un modo è
quello di invocarle come descritto in precendenza con "Modulo.funzione(argomenti)", 
un altro è quello in cui "catturiamo" la funzione stessa e la riusiamo come una variabile.

Abbiamo già visto che possiamo assegnare alle variabili qualsiasi tipo di dati,
adesso possiamo vedere come possiamo assegnare loro anche delle funzioni.

Per esempio: 


```
iex> defmodule Matematica do
...>   def somma(a, b) do <<<--------la nostra funzione 
...>     a + b            <<<--------------------------
...>   end                <<<--------------------------
...> end

iex> Matematica.somma(1, 2)
3
```

Ha un equivalente: 

```
iex> defmodule Matematica do
...>   def somma(a, b) do <<<--------la nostra funzione 
...>     a + b            <<<--------------------------
...>   end                <<<--------------------------
...> end

iex> funzione_somma = &Matematica.somma/2
iex> funzione_somma.(1, 2)
3
```

Possiamo catturare delle funzioni con l'uso di `&` e `/numero_di_argomenti`. Dato che la nostra
funzione "somma" accetta e richiede due argomenti possiamo chiamarla con `&Matematica.somma/2`




