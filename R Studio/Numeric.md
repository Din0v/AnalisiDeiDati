# Numeric In R
Numeric vectors 
the `numeric("Length")` creates an object Numeric and it's identical to `double` as it creates a double precision vector of specified length with each element equal to 0

i stumbled upon this doing a [[Fibonacci]] implementation in R 

```R
Fib <- numeric(20)  # we defined a numeric vector 
Fib[1] <- Fib[2] <- 1 # we se the base case that all of these cases are Equal to 1 review my notes for WHY !!!
for(i in 3:20) Fib[i] <- Fib[i-2] + Fib[i- 1] # the iteration Loop
print(Fib) # Printing it out 

# In this example we can exchange the <- with = 

```


`<-` is an [[Assignment operator]]


---
### Tags
#Rstudio
