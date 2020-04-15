## Tuples

Elixir usa le parentesi graffe per rappresentare liste di valori accessibili via index. 
Nei comuni programmi Elixir, le tuple sono usate generalmente per contenere un numero limitato di valori (dai tre in giù)
in modo che sia più semplice fare operazioni di confronto tra due tuples. 

`{:ok, valore}`, `{:error, valore}` sono tuples che vedrete molto spesso nei programi elixir, 
è questo non è altro che un modo per rappresentare il fatto che la variabile "valore" sia
stata generata da una operazione che ha avuto successo o meno.

Le tuples sono molto efficienti se bisogna accedere a dei valori al loro interno riferendoci 
ad una posizione, indice preciso. Le tuples sono efficienti in questo senso poiché 
i loro valori in memoria sono salvati in modo ravvicinato.

Possiamo accedere ai valori all'interno delle tuple in diversi modi, con pattern matching oppure attraverso il 
loro indice (essendo questo metodo molto efficiente)