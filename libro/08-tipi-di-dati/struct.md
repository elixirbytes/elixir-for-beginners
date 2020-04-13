##  Structs (mappe con un nome)

Gli structs sono fondamentalmente delle mappe con un nome, possono contenere ogni tipo di dati
ma sono create aprendo "%", aggiungendo un nome, e chiudendole con "}".

Esempio: 

` %Persona{nome: "Lorenzo", cognome: "Sinisi"}  `

Possiamo accedere ai valori all'interno degli structs in questo modo:

```
iex(1)> defmodule Persona do
...(1)>   defstruct [:nome, :cognome]
...(1)> end
{:module, Persona,
 <<70, 79, 82, 49, 0, 0, 6, 188, 66, 69, 65, 77, 65, 116, 85, 56, 0, 0, 0, 184,
   0, 0, 0, 18, 14, 69, 108, 105, 120, 105, 114, 46, 80, 101, 114, 115, 111,
   110, 97, 8, 95, 95, 105, 110, 102, 111, 95, ...>>,
 %Persona{cognome: nil, nome: nil}}
iex(2)> %Persona{nome: "lorenzo", cognome: "sinisi"}
%Persona{cognome: "sinisi", nome: "lorenzo"}
iex(3)>
```


Essendo gli struct dei dati che non sono comuni a tutti i programmi Elixir, il programmatore
ha bisogno di definirli all'interno del proprio programma con "defstruct". E per questo serve anche 
creare loro un "modulo" (che vedremo nei prossimi capitoli).

