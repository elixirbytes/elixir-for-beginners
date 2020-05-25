# Erlang Virtual Machine (BEAM)

L'ultimo strumento di cui hai bisogno è la macchina virtuale
(Erlang Virtual Machine[^1]) su cui gira il linguaggio Elixir.[^2]

Questo è un programma che può eseguire il codice Elixir, ed è un programma che
può essere eseguito nella shell (molto simile `cd` e `ls`).

Se per esempio abbiamo del codice in un file dal nome `ciao.exs` e si è passati
alla directory in cui viene salvato il file, è possibile digitare quanto segue e
premere INVIO, per eseguire il codice:

```shell
elixir ciao.exs
```

Questo indicherà alla *macchina virtuale* di interpretare il contenuto del file
come codice *Elixir* ed eseguirlo.

Si può anche utilizzare questo comando per fare altre cose.

Probabilmente non ne avrai bisogno per ora, tuttavia ti verrà utile in futuro.

È possibile provare a digitare questi comandi nel terminale.

Ad esempio, è possibile visualizzare la versione del programma Elixir,
scrivendo:

```shell
elixir --version
```

Che visualizzerà a schermo, un testo simile (*output*)

```shell
Erlang/OTP 20 [erts-9.3.3.15] [source] [64-bit] [smp:4:4] [ds:4:4:10] [async-threads:10] [hipe] [kernel-poll:false]

Elixir 1.9.4 (compiled with Erlang/OTP 20)
```

Dove la versione Elixir è `1.9.4`, mentre la versione di Erlang/OTP è `20`.

Oppure eseguire il codice Elixir senza salvarlo in un file:

```shell
elixir -e 'IO.inspect("Ciao Elixir")'
```

Dove l'output sarà:

```shell
"Ciao Elixir"
```

[^1]: https://it.wikipedia.org/wiki/Erlang_(linguaggio_di_programmazione)

[^2]: https://it.wikipedia.org/wiki/Elixir_(linguaggio_di_programmazione)
