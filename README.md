# project2
Numerical Methods Course - Project2
=========

## Table of contents

- [About](#about)
- [Documentation](#documentation)
- [Creators](#creators)


## About

Approximating the sine function using polynomials is discussed. The L2-norm of errors of approximation are calculated and plotted. Further, the derivative is calculated using the two methods outlined in the questions (written by E. Schnetter).


## Documentation
You can use the functions as outlined in the comments written throughout the code. Here is a brief outline of the functions and important variables:

### Variables:
  - f(x): function to define, here it is the sine function
  - min, max: minimum and maximum for the interval for which we are approximating the function f(x)
  - pmax: maximum order of polynomials used
  - npoints: number of points sampled from the interval [min, max]
  
### Functions:
  - make_fig(): makes a generic figure to be filled with a plot
  - find_coeffs(): find coefficients approximating the sine function, i.e. c's in the relation
  $sin(x) \approx \sum_p c_p \times x^p$


## Creators

Ali SaraerToosi
