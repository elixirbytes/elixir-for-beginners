## Funzioni private

Non sempre vogliamo che le nostre funzioni siano esposte al pubblico. Ci sono delle funzioni che possono 
essere utilizzate da altri moduli del nostro programma, mentre altre che sono più "private". 

Una funzione privata si dichira all'interno di un modulo esattamente come quelle pubbliche, la diffrenza
è che invece di `def`, bisogna utilizzare `defp`.

La particolarità di queste è che sono utilizzate per "semplificare" funzioni più complesse
e rendere la lettura più semplice.
