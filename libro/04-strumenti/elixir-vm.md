- Erlang Virtual Machine (BEAM)

L'ultimo strumento di cui hai bisogno è la macchina virtuale
(Erlang Virtual Machine [1]) su cui gira il linguaggio Elixir. [2]

Questo è un programma che può eseguire il codice Elixir, ed è un programma che
può essere eseguito nella shell (molto simile 'cd' e 'ls').

Se per esempio abbiamo del codice in un file dal nome `ciao.exs` e si è passati
alla directory in cui viene salvato il file, è possibile digitare quanto segue e
premere INVIO, per eseguire il codice:

```
elixir ciao.exs
```

Questo indicherà alla *macchina virtuale* di interpretare il contenuto del file
come codice *Elixir*ed eseguirlo.

Si può anche utilizzare questo comando per fare altre cose.

Probabilmente non ne avrai bisogno per ora, tuttavia ti verra' utile in futuro.

È possibile provare a digitare questi comandi nel terminale.

Ad esempio, è possibile visualizzare la versione del programma Elixir:

```
elixir --version
```

Oppure eseguire il codice Elixir senza salvarlo in un file:

```
elixir -e "IO.inspect('Ciao Elixir')"
```

 [1]: https://it.wikipedia.org/wiki/Erlang_(linguaggio_di_programmazione)
 [2]: https://it.wikipedia.org/wiki/Elixir_(linguaggio_di_programmazione)
