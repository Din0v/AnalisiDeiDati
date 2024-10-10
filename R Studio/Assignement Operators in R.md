# Assignment operators 

Assign a value to a name: 

- `<-`: the operator is older and can be used anywhere to assign value to the function

- `=`: is newer it was introduced in 2001 and is only allowed at the top level ( in the complete expression typed at the command prompt )

- `<<-`: ``` x <<- value<=""code""= ```

- `->`:

- `->>`:

---
P.S. The difference in the assignment operators is clearer when you use them to set an argument in a function call 
```R
median(x = 1:10)
x
# Error; object 'x' not found 
```

in this case  `x` is declared within the scope of the function, so it does not exist in the user workspace! therefore the correct usage is as a follows 

```R 
median(<- 1:10)
x
#  [1]  1  2  3  4  5  6  7  8  9 10
```

in this case, `x` is delcared in the user workspace, so you use it after the function call has been competed. 

---
# Easy way to write <- is to: 
`alt + -` will print the assignment symbol!! 

---
### Tags
#Rstudio
#Latex 
#R_Tricks 