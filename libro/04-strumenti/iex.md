# REPL

Elixir è un linguaggio con una sintassi molto simile a quella di Ruby che però, 
contrariamente appunto a Ruby, sfrutta la potenza della BEAM, ovvero la virtual machine di Erlang,
e dell’ecosistema OTP per costruire ed eseguire applicazioni per la maggior parte di rete, 
a bassa latenza, distribuite, fault-tolerant.

Oltre ad essere un vero gioiellino per le web application 
ed in generale la programmazione distribuita, la sintassi funzionale impura Ruby-like 
lo rende in realtà un meraviglioso giocattolino general purpose, che diventa adatto per 
costruire qualsiasi tipo di programma, anche un CLI tool o altro.

Il sito ufficiale del linguaggio è elixir-lang.github.io.

Setup
Il setup dell’ambiente è abbastanza facile. Su macOS:

$ brew install elixir
Su Linux leggermente meno, ma dipende dalla distribuzione che usiamo. In genere abbiamo il pacchetto elixir nei repository della nostra distribuzione. Per Arch Linux è sufficiente un:

# pacman -S elixir
Ubuntu e Debian per esempio prevedono che venga usato il repository di pacchetti di Erlang Solutions:

$ wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb
$ sudo dpkg -i erlang-solutions_1.0_all.deb
$ sudo apt-get update
$ sudo apt-get install esl-erlang elixir
In caso di necessità comunque, informazioni aggiornate possono essere trovate sulla pagina ufficiale.

REPL
Ora che abbiamo il nostro setup possiamo divertirci con il REPL.

A Read–Eval–Print Loop (REPL), also known as an interactive toplevel or language shell, 
is a simple, interactive computer programming environment that takes single user 
inputs (i.e. single expressions), evaluates them, and returns the result to the user; 
a program written in a REPL environment is executed piecewise. 
The term is most usually used to refer to programming interfaces similar to the 
classic Lisp machine interactive environment. Common examples include command line
shells and similar environments for programming languages, and is particularly 
characteristic of scripting languages.

Tip: moltissimi altri linguaggi hanno un REPL incluso nell’ambiente di sviluppo,
come Python (python), JavaScript (node o la stessa console di Chrome), 
Ruby (irb), Haskell (ghci).

Il nostro REPL nello specifico si chiama iex. 
Lanciandolo nel terminale ci dà un po’ di informazioni utili, 

dopodiché sta a noi cominciare a fabbricare i nostri elixir:

22:02:51 › iex

Interactive Elixir (1.5.3) - press Ctrl+C to exit (type h() ENTER for help)
iex(1)>

Ci siamo.

Hello world

Il percorso di apprendimento di un nuovo linguaggio comincia sempre con un hello world.

iex(1)> IO.puts("hello world!")
hello world!
:ok
iex(2)>

