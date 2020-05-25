# Programmare significa creare

*Dare vita alle cose*

Programmare significa creare. Quando eseguiamo un programma, un piccolo universo
viene creato. Le cose prendono vita ed iniziano ad interagire tra di loro, il
tutto attraverso le regole che tu, in qualità di creatore, hai definito.

Immagina di creare un'applicazione come Twitter.

Come sviluppatore, nel linguaggio di programmazione di tua scelta, si direbbero
cose come "Ora esistono gli utenti!”, “Ora esistono i tweet", e una volta che
l'applicazione inizia ad esistere queste affermazioni prendono davvero vita.

Poi si dovrebbe andare avanti e definire che "Gli utenti possono creare tweet, e possono seguire l'uno il profilo dell'altro".

E d'ora in poi, ogni volta che vengono creati nuovi utenti nel piccolo universo
che è l'applicazione, questi avranno la possibilità di "twittarsi" e seguirsi a
vicenda.

## Breve (ed imprecisa) introduzione alla programmazione

*Programmare è metterci le mani sopra*

Un'analogia che potremmo fare è comparare la programmazione alle istruzioni
per le ricette che usiamo per cucinare.
Leggendo una ricetta, o guardando un video youtube, seguiamo le istruzioni
che un'altra persona ha preparato per cucinare un buon piatto.

Possiamo pensare alla ricetta usata in cucina, come "codice sorgente" del nostro
programma.
Il programma è il frutto del nostro lavoro con il codice sorgente, seguendo
l'analogia è il nostro buon piatto cucinato.

Il processo dello sviluppo software (quindi scrivere codice sorgente per
produrre un programma) può essere anche immaginato come un libro.

I libri, sono di diversi generi e di diversa consistenza (romanzi, saggi,
libri sui viaggi, racconti brevi, ecc)
Quando si scrive un libro (od un racconto), prima di pubblicarlo o mandarlo
in stampa, il libro percorre una serie di revisioni e quando viene approvato
dall'editore, viene pubblicato in forma digitale o stampato fisicamente.
In ogni caso c'è un "rilascio" del libro al pubblico.

Sviluppare software è simile al processo di scrittura di un libro.

Scrivere software, tuttavia, differisce dallo scrivere un libro perché lo
scrivere software non ha una vera fine!
Pensate alle varie "app" che installate sul vostro cellulare.
Esse, vengono aggiornate continuamente, per eliminare difetti di programmazione
commessi o sfuggiti ai programmatori.
Alle vostre "app" vengono anche aggiunte nuove funzionalità, ed introdurre
nuove funzionalità, molto probabilmente implicherà aggiungere nuovi difetti
nel software.

Il software non è mai perfetto, perché prodotto da persone in carne ed ossa.

Per quanto possa sembrare "strano" a chi non conosce la programmazione, chi
sviluppa software, oltre a sapere scrivere codice, deve sapere anche comunicare
e collaborare con colleghi programmatori, e deve cercare di esprimersi nel modo
più semplice possibile, evitando di approfondire i dettagli tecnici, con
colleghi che non sanno nulla di programmazione.
La comunicazione, collaborazione e l'essere pronti ad accettare i propri errori
e quelli degli altri, ascoltare e capire, sono le abilità fondamentali per
diventare un buon programmatore. 
A volte addirittura più della scrittura del codice, perché essendo aperti ci si
può evolvere ed imparare.

Scrivere codice è anche un dialogo con se stessi e con gli altri.
Parecchi programmatori pensano che leggere il codice di altri programmatori
riveli un po' della personalità del programmatore!

Oltre alla comunicazione, il compromesso, la pazienza e la curiosità, vi
aiuteranno a scrivere programmi. 
La passione ci deve essere, ma si sa. La passione a volte può affievolirsi ;)

Inoltre, resiste ancora, in qualche modo, uno stereotipo dei programmatori con
il con gli occhiali rotti, solitari ed introversi, propagandato dai giornali ed
altre fonti di informazione.
Tuttavia i programmatori oggi, pur sembrando ad un non addetto ai lavori
"strani", sono persone come le altre (mi includo pure io!) con le loro passioni,
debolezze e qualità.
Troverete programmatori introversi, estroversi (a volte un po' troppo! ;)),
diplomatici. Tutte le sfumature dell'umanità sono presenti. Garantito!

Tornando a noi, all'inizio abbiamo affermato che la programmazione è creazione.
In aggiunta, la programmazione è anche espressione umana. 
I programmatori possono anche dedicarsi esplicitamente all'arte ed ad altri
campi non necessariamente "seri" (notare le virgolette)

# Codice e Arte

Vi sono movimenti di "live coding" (programmazione dal vivo) in cui questi
artisti, davanti ad un pubblico, compongono e manipolano musica scrivendo
codice. Spesso, oltre alla musica, associano anche forme visuali sincronizzate
con la musica prodotta durante l'esibizione dal vivo.

# Programmazione etica

La programmazione, oltre ad essere uno strumento per finanze, commercio
elettronico ed altre diavolerie orientate all'incremento di capitale, è anche
uno strumento per aiutare persone, mettendole in contatto o fornendo loro
strumenti per collaborare assieme.

In particolare il movimento del Software Libero (conosciuto da molti come "Open
Source"), è alla base della filosofia di Internet ed è anche la sua base
tecnologica. 
Purtroppo, in questo periodo storico, Internet, è diventata chiusa, simile ai
Silos di grano. 
Avete mai pensato di voler trasferire i dati della vostra "app" che traccia le
vostre corse e le vostre tempistiche da una "app" ad un'altra?
Oggigiorno nella maggior parte dei casi questo non è possibile.

Internet è nata ed esiste grazie ai protocolli aperti, i formati
interscambiabili e la collaborazione mondiale dei programmatori.
Senza questa "etica" Internet ed il mondo sarebbe più povero (di conoscenza) e
questo libro non sarebbe mai nato, molto probabilmente.

Quindi potresti essere tu uno dei futuri programmatori a continuare questa tradizione
per migliorare la società!


# Passiamo ad Elixir

Per questo corso abbiamo scelto il linguaggio di programmazione Elixir, perché è
basato su una tecnologia chiamata "virtual machine" o macchina virtuale in
Italiano, che è stata progettata per fornire degli strumenti di resilienza
(fault tolerance o letteralmente resistenza ai guasti/errori).
Il che la rende molto speciale ed unica.
Gli autori non conoscono un altro sistema al mondo che fornisca nativamente
strumenti per essere resiliente ed ispezionare un sistema in produzione in tempo
reale -- dal vivo.

# BEAM Virtual Machine (Macchina Virtuale)

Elixir "gira" su una virtual machine.
La virtual machine, chiamata BEAM può ospitare diversi linguaggi di
programmazione che seguono la filosofia della fault tolerance.
Il linguaggio "padre" della BEAM è Erlang, creato da Joe Armstrong e Robert
Virding.

Erlang è stato progettato per servire reti telefoniche. Uno dei requisiti
fondamentali, era quello di non poter fare cadere la rete telefonica se ci
fosse stato un errore nel sistema, pena multe salatissime e telefonate non
servite!
Questa progettazione (design) fornisce strumenti al programmatore che
permettono di creare, idealmente sistemi, che "si curano da soli"
(auto-healing)
Se siete curiosi di avere qualche cenno su Erlang, seguite questo link:
[Erlang](https://it.wikipedia.org/wiki/Erlang_(linguaggio_di_programmazione))

# Cos'è Elixir quindi?

È un linguaggio di programmazione che sposa la filosofia di Erlang e gira
sulla BEAM (la macchina virtuale) Potreste immaginare il linguaggio di
programmazione Elixir, come il figlio di Erlang.

Elixir è stato creato da José Valim, per rendere piu' accessibili ai
programmatori più giovani e non, l'ecosistema di Erlang.
Elixir, è più simile a linguaggi di programmazione che sono attualmente
popolari.

Se siete curiosi di avere qualche cenno su Elixir, seguite questo link:
[Elixir](https://it.wikipedia.org/wiki/Elixir_(linguaggio_di_programmazione))

Link utili:

https://elixirschool.com/it/ (progetto collaborativo e volontario in varie
lingue per imparare Elixir -- questo e' il link in Italiano)

https://elixir-lang.org/ (sito ufficiale, in Inglese)

https://elixir-lang.org/install.html (istruzioni di installazione per
Windows, Linux e MacOSX di Erlang ed Elixir -- funzionano assieme)
