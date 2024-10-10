# sequence generator in R 

**Porre n = 5 + il proprio giorno di nascita. Creare un vettore dei multipli
di n compresi fra 1253 e 2037.**


```R 
n <- 5 + 19  # Sostituisci "27" con il tuo giorno di nascita

# Creazione del vettore dei multipli di n compresi tra 1253 e 2037
multipli <- seq(from = ceiling(1253/n) * n, to = floor(2037/n) * n, by = n)

# Stampa del vettore
print(multipli)
```


Attenzione che non ci serve l'operatore del modulo che basta fare una semplice divisione 
si usa la forma ```Ceiling``` e ```Floor``` per dentotare i limiti superiori ed inferiori. 


Leggere attentamente la documentazione :)


### Tags
#R 
#functions



