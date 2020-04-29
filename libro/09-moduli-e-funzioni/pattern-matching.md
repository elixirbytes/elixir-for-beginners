## Pattern matching all'interno delle funzioni di un programma


Abbiamo visto come le funzioni all'interno dei moduli possono 
ricevere argomenti di ogni tipo, ma come operarare in modo diverso su diversi 
tipi di dati?

Come abbiamo già visto, in Elixir abbiamo il concetto di "pattern matching". Questo lo troviamo utile anche quando scriviamo le nostre funzioni. 

Per esempio il seguente modulo è valido: 

```
1  defmodule Persona do 
2    defstruct [:nome, :anni]
3    def nome(%Persona{nome: nome} = persona) do
4      nome
5    end
6  
7    def anni(%Persona{anni: anni} = persona) do
8      anni
9    end
10 end
```

E vediamo come usare il pattern matching per fare qualcosa di abbanzanza complesso: 

- abbiamo usato il pattern matchin per eseguire `%Persona{nome: nome} = persona` alla riga nummero 3
- in questo modo abbiamo "creato" una nuova variabile chiamata "nome" all'interno degli argommenti di una funzione
- abbiamo riusato il "nome" all'interno del `body` della funzione per estrarlo e farci qualcosa come valore di ritorno. 

Un modo in cui potremmo usare il pattern matching è per comunicare che il modulo Persona funziona solo con "Persona" come tipi di dati, per esempio: 

```
1  defmodule Persona do 
2    defstruct [:nome, :anni]
3    def nome(%Persona{nome: nome} = persona) do
4      nome
5    end
6
7    def nome(altri_dati) do
8      IO.inspect(altri_dati) <> "non è supportato. Usa %Persona{} con il modulo Persona invece."
9    end
10 
11    def anni(%Persona{anni: anni} = persona) do
12      anni
13    end
14 end
```

Oppure potremmmo creare funzioni che si comportano in modo diverso a seconda che ricevano una lista invece che una mappa o uno struct. Un buon esercizio sarebbe quello di provare a creare tali funzioni nella console. 
