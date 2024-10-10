# Newton-Raphson numerical method

The Newton-Raphson method is an iterative root-finding algorithm used to approximate real roots of nonlinear equations with high degrees of accuracy.

![[Pasted image 20240226142106.png]]

```R
newton_raphson <- function(f, f_prime, x_start, tol = 1e-8, max_iter = 100) {
  # Initialize variables
  x_current <- x_start
  iter_count <- 0
  
  repeat {
    if (iter_count >= max_iter) {
      cat("Maximum number of iterations reached.\n")
      break
    }
    
    # Compute function value and derivative at current point
    y_current <- f(x_current)
    dy_current <- f_prime(x_current)
    
    # Check for zero derivative (avoids division by zero errors)
    if (abs(dy_current) < tolerable_value) {
      cat("Derivative close to zero; unable to proceed.\n")
      break
    }
    
    # Update estimate using Newton-Raphson formula
    x_next <- x_current - y_current / dy_current
    
    # Calculate absolute error and check for convergence
    abs_error <- abs(x_next - x_current)
    
    if (abs_error < tol) {
      cat(sprintf("Root found after %d iterations:\nx = %.8f\n", iter_count + 1, x_next))
      break
    }
    
    # Assign updated estimate as current estimate for next iteration
    x_current <- x_next
    iter_count <- iter_count + 1
  }
}

```

### Tags 
#Roots 