##  Mappe (di dati)

Le mappe, in modo simile alle liste, possono contenere ogni tipo di dati
ma sono create aprendo "%{" e chiudendole con "}".

Esempio: 

` %{nome: "Lorenzo", cognome: "Sinisi"}  `

Possiamo accedere ai valori all'interno delle mappe in questo modo:

```
iex(3)> persona = %{nome: "Lorenzo", cognome: "Sinisi"}
%{cognome: "Sinisi", nome: "Lorenzo"}
iex(4)> persona.nome
"Lorenzo"
iex(5)>
```

