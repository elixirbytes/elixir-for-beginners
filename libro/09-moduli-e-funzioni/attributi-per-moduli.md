## Moduli e attributi


Abbiamo visto come i moduli servano a contenere una lista di funzioni e a ritrovarle
quando ne abbiammo bisogno. Ma i moduli possono contenere anche altre informazioni utili
ai programmi che stiamo creando. Uno di questi dati, e l'abbiamo già visto, è lo structs. 
Mentre altri dati, quelli che di solito non cambiano durante la fase di vita di un programma, 
sono gli attibuti. In altri programmi sono chiamate costanti, proprio perché particolarmente immutabili. 

Un attributo si definisce con la chiocciola, seguita dal nome, seguita da dati.


```
defmodule Triangolo do 
  @angoli 3
end
```

Nell'esempio appena visto vediamo come definire l'attributo @angoli per il modulo Triangolo. 

Potremmo usarlo nel seguente modo all'interno di una funzione: 




```
defmodule Triangolo do 
  @angoli 3

  def communica_angoli do
    "Il triangolo ha #{@angoli} angoli."
  end
end
```

  
