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
  

  Note: the inputs of the functions have the same names as the above variables. Furthermore, many functions accept variable "func" as one of their inputs, which is the function that is going to be approximated. Here it will be the sine function, and the cosine function in case of approximating the derivatine of the sine function in Q4.
  ### Functions:
  - make_fig(): makes a generic figure to be filled with a plot
  - find_coeffs(): find coefficients approximating the sine function, i.e. c's in the relation
  $sin(x) \approx \sum_p c_p \times x^p$
  - find_poly(): finds the polynomial that fits the data the best (using the formula discussed in the class)
  - plot_f_poly(): plots the approximated value for all the npoints, i.e. yy (the blue line), and the actual values (red line) of the function which is the sine function here, i.e. fstar.
  - find_plot_poly(): applys find_poly() adn plot_f_poly(), so it finds the polynomial and plots it.
  ![alt text](https://github.com/as2c/project2/blob/main/q1pmax3.png)
  
  - calc_L2error(): calculates the L2 error of the approximated points yy and the actual values fstar.
  - calc_errors(): calculate errors for all the values of pmax, from 0 to pmax_lev, and put them in an array
  - plot_L2errors(): plotting the errrors. The function accepts a variable called "lower_bound" which tells the function which errors to plot. It does not plot the errors for pmax < lower_bound. e.g. for lower_bound = 8 we will have the following plot:
  ![alt text](https://github.com/as2c/project2/blob/main/errors_from8.png)
  - find_odd_poly(): just like find_poly but only keeping odd powers, since sine function is antisymmetric
  - calc_odd_errors(): just like calc_errors in Q2 but only for odd powers
  - plot_odd_L2errors(): just like plot_L2errors function in Q2 but for odd powers
  ![alt text](https://github.com/as2c/project2/blob/main/errors_odd.png)
  - compare_poly_plots(): comparing the errors of approximating by using only the odd power polynomials (the cyan line) with approximation using all powers (the red line).
  ![alt text](https://github.com/as2c/project2/blob/main/compare_plots.png)
  - calc_D(): based on 4.a) this function calculates D matrix
  - find_d(): This function finds |d> = D |c>
  - calc_deri_D(): This function calculates the derivative from the coefficients |d> that we found.
  - plot_Dderi_vs_fprime(): Plots the derivatives calculated with D matrix and by approximating cos(x) using Q2 functions.
  ![alt text](https://github.com/as2c/project2/blob/main/plot_der_vs_fprime.png)
## Creators

Ali SaraerToosi
