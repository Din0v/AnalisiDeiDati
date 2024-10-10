[Leggi](https://www.investopedia.com/terms/p/poisson-distribution.asp)

The Poisson distribution is a mathematical model that describes 
- **A number of events in a fixed interval of time**
- it often describes events that are **Rare and Random** also called **R&R**

Now, let's say you want to know the probability of a specific number of events happening in that interval. That's where the Poisson distribution comes in. It can tell you the likelihood of observing a certain number of events based on the average rate at which they occur

applications of the Poisson distribution can be in: 
1. **Traffic flow**: cars arriving at a toll booth
2. **Call center**: Nr of incoming calls 
3. **Biology**: modeling the mutation in a DNA sequence 
4. **Queuing Theory**: Nr. of customers arriving at a service center 
5. **Economics**: predicting the Nr. of defaults on given loans 

In essence, the Poisson distribution helps us make predictions about the occurrence of rare events when we have information about the average rate at which those events happen.


## Formula 
$$  Poisson[X=K] = \frac {\lambda^{-k}}{k!} e^{-\lambda}  $$

where: 
- $K$ is the number of events 
- $\lambda$ is the probability of the event (average success rate per trail )


## Approximation of a binomial distribution with a Poisson distribution 

l'approssimazione di una [[Binomial Distribution]]
- Possiamo usare questo trucco al verificarsi di due condizioni: 

1. Bassa probabilità di successo $p$ $P[success] \rightarrow 0$ 
2. presenza di un gran numero di prove $n$ $Prove \rightarrow \infty$ la semplice euristica dice che il prodotto :
   - $np \le 5$  
   - $n(1-p)\le 5$ 
devono essere più grandi di 5.

se queste condizioni sono soddisfatte il parametro di Poisson $\lambda$ è uguale a: 
$$\lambda = np$$
>[!Note] Nota Bene
>If the mean is very large, then the Poisson distribution is approximately a normal distribution.




### Tags 
#Distributions 
#Poisson

