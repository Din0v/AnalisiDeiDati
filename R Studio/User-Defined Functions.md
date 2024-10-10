# User Defined functions AKA DIY functions 
---

we can create a DIY function in R and here is an example on how: 

this is a function that gives back the square of all the numbers from a to 1 

``` R 
new.fucntion <- function(a){
	for (i in 1:a){
		b <- i^2 # as we can see b is only declaered in this scope 
		print(b)
	}
} ## the variable b doesn't exist here anymore 
```

we call the function by simply  typing it's name and following with an argument: 

```R
new.function(6)
```

## Example 2 
Factors of a Number: as we can see the function is called NumFact. 
``` R 

NumFact = function(n){
print(paste("the factors of ", n, "are: "))
for(i in 1:n){
  if ((n %% i ) == 0){
    print(i)
    }
  }
}

```


---
### Tags 
#Rstudio 
