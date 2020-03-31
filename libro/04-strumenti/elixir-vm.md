- Elixir VM 

L'ultimo strumento di cui hai bisogno è una macchina virtuale Elixir. Questo è un programma che può eseguire il codice Elixir, 
ed è un programma che può essere eseguito nella shell (molto simile 'cd' e 'ls').

Se per esempio abbiamo del codice in un file dal nome 'ciao.ex' e si è passati alla directory in cui viene salvato il file, 
è possibile digitare quanto segue e premere INVIO, per eseguire il codice:

```
elisir ciao.ex
```

Questo indicherà alla 'macchina virtuale' 'elixir' di interpretare il contenuto del file 'ciao.ex' come codice Elixir ed eseguirlo.

Si può anche utilizzare questo metodo per fare altre cose. 

Probabilmente non ne avrai bisogno per ora, ma pensiamo che faccia bene saperlo. 

È possibile provare a digitare questi comandi nel terminale.

Ad esempio, è possibile stampare la versione del programma Elixir:

```
elisir --version
```

Oppure eseguire il codice Elixir senza memorizzarlo in un file:

```
elixir -e "IO.inspect('Ciao Elixir')"
```
