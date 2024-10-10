# Oscillatore di Van der Pol 
la relazione sua con le equazioni differenziali 

```R 
library(deSolve)
library(ggplot2)

# Definizione delle equazioni differenziali per l'Oscillatore di Van der Pol
vanderpol <- function(t, y, params) {
  x <- y[1]
  dx <- y[2]
  mu <- params$mu
  dx1 <- dx
  dx2 <- mu * (1 - x^2) * dx - x
  return(list(c(dx1, dx2)))
}

# Set dei parametri
params <- list(mu = 1)

# Condizioni iniziali
initial_state <- c(x = 0.1, dx = 0)

# Intervallo temporale
times <- seq(0, 30, by = 0.01)

# Risoluzione dell'ODE
sol <- ode(y = initial_state, times = times, func = vanderpol, parms = params)

# Creazione del grafico
plot_data <- data.frame(sol)
ggplot(data = plot_data, aes(x = time, y = x)) +
  geom_line() +
  labs(x = "Tempo", y = "x") +
  theme_minimal()

```

questo (forse) è un a rappresentazione della sua equazione visualizata in R 
![[Pasted image 20230524202145.png]]

se vede L'attenuazione 



---
## Tags
#Equazioni_Differenziali 
#ds