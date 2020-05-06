## Condizioni e controllo dei flussi

In un qualsiasi linguaggio di programmazione possiammo trovare codice come il seguente: 

```
# sorgente https://nickjanetakis.com/blog/refactoring-elixir-code-if-cond-and-pattern-matching
def initials(name) do
  if name == nil or name == "" do
    "?"
  else
    if String.contains?(name, " ") do
      split_name = name |> String.split(" ")

      first_letter = split_name |> List.first() |> String.slice(0, 1)
      last_letter = split_name |> List.last() |> String.slice(0, 1)

      "#{first_letter}#{last_letter}"
    else
      name |> String.slice(0, 1)
    end
  end
end
```

Ma in Elixir abbiamo la comodità di concetti come "cond", vediamo come usarlo
per migliorare la leggibilità del nostro codice: 

```
def initials(name) do
  cond do
    name == nil or name == "" ->
      "?"
    String.contains?(name, " ") ->
      split_name = name |> String.split(" ")

      first_letter = split_name |> List.first() |> String.slice(0, 1)
      last_letter = split_name |> List.last() |> String.slice(0, 1)

      "#{first_letter}#{last_letter}"
    true ->
      name |> String.slice(0, 1)
  end
end
```

In questo case abbiamo estratto le 3 condizioni a cui la nostra 
logica fa riferimento.


Ma nella scorsa lezione abbiamo visto come possiamo usare il `pattern matching` 
per valutare diverse condizioni, quindi potremmo usarle: 

```
  def initials(name) when name in [nil, ""], do: "?"

  def initials(name) do
    split_name = name |> String.split(" ")

    first_letter = split_name |> List.first() |> String.slice(0, 1)
    last_letter = split_name |> List.last() |> String.slice(0, 1)

    case Enum.count(split_name) do
      1 ->
        first_letter

      _ ->
        "#{first_letter}#{last_letter}"
    end
  end
```

Il codice a questo punto diventa più conciso e molto semplice da leggere.


## Extra su if/else/unless: 

Come in molti altri linguaggi di programmazione 
possiamo usare anche `unless` per indicare il caso in cui 
una condizione è negata.

Per esempio: 

```
if true do
 1 + 2
end
```

Potrebbe diventare:
```
unless false do
 "Non vedremo mai questa stringa"
end
```

Ed entrambe potrebbero essere abbrevate utilizzando i `do`:



```
if true, do: 1 + 2
```

Potrebbe diventare:

```
unless false, do: "Non vedremo mai questa stringa"
```

e possiamo ovviamente usare anche `else` poiché stiamo 
usando le __keywordlists__ come argomenti per if/else: 

`if false, do: :this, else: :that`

Possiamo riferirci alla documentazione elixir per altri esempi: https://elixir-lang.org/getting-started/case-cond-and-if.html
