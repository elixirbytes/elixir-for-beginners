## Stringhe (Testo)

Le stringhe, per semplicità, non sono altro che testo. Si creano aggiungendo le doppie virgolette
all'inizio e alla fine del testo: "Ciao", "Casa", "Qualcosa che abbia anche spazi", etc.

Bisogna stare attenti a non confondere le stringhe con le doppie e single virgolette. 

In Elixir le stringhe con le doppie virgolette sono effettivamente trattate come testo, mentre 
le stringhe tra virgolette singole sono visualizzate esattamente come una normale stringa 
ma sono in realtà delle liste di caratteri. Sono dei dati diversi che possono confondere e creare bug. 

Vedremo meglio come si differenziano nel paragrafo sulle liste. Quello che ci serve sapere per ora è
che se vogliamo rappresentare del testo, il nostro modo di farlo è ``""``.