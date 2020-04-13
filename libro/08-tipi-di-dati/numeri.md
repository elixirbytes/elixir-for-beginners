## Numeri

I numeri sono forse il tipo di dati più semplice ed immediato di cui parlare. Non sono
altro che quello che tutti abbiamo imparato a scuola: numeri interi e numberi con la virgola. 

Si rappresentano esattamente come lo faremmo in qualsiasi altro contesto: `10`, `10.0` etc.


Quello che è importante ricordare è che operazioni matematiche con i numeri sono sempre più accurate
usando nummeri interi piuttosto che decimali. In ogni linguaggio di programmazione, i nummeri non sono 
necessariamente "esatti" ma piuttosto delle approssimazioni (molto molto corrette). E quindi quando lavoriamo 
con numeri molto piccoli o molto grandi è bene prestare particolare attenzione ai nostri programmi perché 
i risultati potrebbero essere soprendenti.

## Problemi noti

Ci sono alcuni problemi molto noti con i numeri con la virgola e l'aritmetica a causa del fatto che la maggior parte delle frazioni decimali non possono essere rappresentate e la maggior parte delle operazioni non sono esatte, ma si basano su approssimazioni. Tali problemi non sono specifiche di Elixir, sono una proprietà del modo in cui la rappresentazione dei numeri decimali stessi.


- Il numero rappresentabile più vicino a 0,1 è 0,1000000014
- Il numero rappresentabile più vicino a 0,01 è 0,009999997
- L'esecuzione di 0,1 x 0,1 dovrebbe restituire 0,01, ma poiché 0,1 è in realtà 0,1000000014, il risultato è 0,010000000000000002 e poiché questo non è il numero rappresentabile più vicino a 0,01, si otterrà il risultato errato per questa operazione

Ci sono anche altri problemi noti come l'arrotondamento ma per adesso il nostro focus non è questo,
tuttavia è bene sapere che ci sono delle limitazioni in tutti i programmi.