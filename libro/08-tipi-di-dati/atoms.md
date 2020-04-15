## Atoms

Un atom  è una costante. Non è altro che una stringa che inizia con `:` che ha come valore il suo nome.


Per esempio: 

```
iex> :apple
:apple
iex> :orange
:orange
iex> :watermelon
:watermelon
```


E gli atoms o simboli sono uguali se il loro nome è uguale. 

```
iex> :apple == :apple
true
iex> :apple == :orange
false
```

Notiamo come l'operazione `==` tra due atom uguali ritorni `true` e `false`. Questo è
quello che intendiamo quando diciamo che true e false possono essere usati come 
controlli del ciclo di esecuzione.