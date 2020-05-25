# REPL (Read Eval Print Loop)

Elixir è un linguaggio con una sintassi molto simile a quella di Ruby che però,
contrariamente a Ruby, sfrutta la potenza della BEAM, ovvero la virtual machine
di Erlang, e dell’ecosistema OTP per costruire ed eseguire applicazioni per la
maggior parte di rete, a bassa latenza, distribuite, fault-tolerant.

Elixir, è un linguaggio particolarmente adatto ai sistemi "soft real-time",
cioè quei sistemi che devono gestire contemporeneamente ed efficentemente molti
compiti (task/processi).

Ad esempio, pensate a quante cose possa fare un sito web articolato, come un
e-commerce. Seguirvi lungo tutto il vostro percorso di acquisto, aggiornare le
vostre raccomandazioni in tempo reale (come YouTube), oppure mandare notifiche
nel caso ci sia una novita' di interesse in accordo ai vostri gusti personali,
etc

La BEAM, e di conseguenza Elixir, inoltre è adatta a qualsiasi applicazione di
coordinazione di processi.
Ad esempio, la BEAM ha gestito e gestisce reti telefoniche, reti digitali,
programmi collaborativi.
Approfondiremo i campi applicativi di Elixir, proseguendo il corso.

Il sito ufficiale del linguaggio è https://elixir-lang.org/

- Installazione (MacOSX)
Per installare Elixir su MacOSX, e' fortemente consigliato installare `brew`

```bash
$ brew install elixir
```

- Installazione (Linux)

## Distribuzioni basate su Debian (Ubuntu, Linux Mint, etc)

Il modo piu' diretto per installare Erlang/OTP ed Elixir e' usare i pacchetti di
Erlang Solutions (una societa' di consulenza che organizza conferenze sul mondo
della BEAM e fornisce supporto alle startup e alle ditte che usano Erlang /
Elixir)

```bash
$ wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb
$ sudo dpkg -i erlang-solutions_1.0_all.deb
$ sudo apt-get update
$ sudo apt-get install esl-erlang elixir
```

## Arch Linux

```bash
pacman -S elixir
```


## Windows

Nessuno di noi usa Windows, pero' potete trovare le istruzioni sul sito
ufficiale di Elixir:

https://elixir-lang.org/install.html#windows

In caso di necessità comunque, informazioni aggiornate possono essere trovate
sulla pagina ufficiale.

## REPL (Read Eval Print Loop)

Ora che abbiamo il nostro setup possiamo inizare a giocare con il REPL.

```
A Read–Eval–Print Loop (REPL), also known as an interactive toplevel or language
shell, is a simple, interactive computer programming environment that takes
single user inputs (i.e. single expressions), evaluates them, and returns the
result to the user; a program written in a REPL environment is executed
piecewise. The term is most usually used to refer to programming interfaces
similar to the classic Lisp machine interactive environment. Common examples
include command line shells and similar environments for programming languages,
and is particularly characteristic of scripting languages.
```

Suggerimento: moltissimi altri linguaggi hanno un REPL incluso nell’ambiente di
sviluppo, come:

* Python -- python/ipython
* JavaScript -- nodejs, o anche la console del vostro browser (Firefox, Chrome, ecc)
* Ruby -- irb
* Haskell -- ghci

Il nostro REPL nello specifico si chiama `iex`.
Scrivendo `iex` nel terminale ed eseguendo il comando premendo il tasto invio:

```shell
$ iex

Interactive Elixir (1.5.3) - press Ctrl+C to exit (type h() ENTER for help)
iex(1)>
```

Ci siamo.

Hello world!

Il percorso di apprendimento di un nuovo linguaggio comincia sempre con un hello world.

```elixir
iex(1)> IO.puts("Hello world!")
"Hello world!
:ok
iex(2)>
```
