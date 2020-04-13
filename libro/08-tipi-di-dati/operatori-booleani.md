## Operatori booleani

Elixir supporta `true` e `false` come operatori booleani:

```
iex> true
true
iex> true == false
false
```

Elixir ha anche delle funzioni "built-in" per lavorare con gli operatori booleani:

```
iex> is_boolean(true)
true
iex> is_boolean(1)
false
```

Tali operatori sono usati di solito per avere delle condizioni nei nostri programmi e per prendere delle decisioni
in base alle quali eseguire "questo" o "quel" codice.