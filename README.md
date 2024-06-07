# Random Variable Generation (RVG)

This project repository contains the implementation and results of simulations for three distributions: Beta(5,1), Student's t-distribution with 2 degrees of freedom, and Gamma(2,2). Each distribution was chosen to demonstrate different methods of random variable generation and their applications in statistical analysis.

## Project Overview

### 1. Inverse CDF Method
Used for the Beta(5,1) distribution

**Key Steps:**
- Generate a uniform random number u
- Transform u using the inverse CDF $F^{-1}(u) = u^{1/5}$

### 2. Transformation of Random Variables
Applied to generate samples from a Student's t-distribution by transforming variables from standard normal and chi-squared distributions

**Key Steps:**
- Generate z from N(0, 1) and vfrom $\chi^2(2)$
- Compute $T = \frac{Z}{\sqrt{V/2}}$

### 3. Accept-Rejection Method
Implemented to sample from Gamma(2,2) using Gamma(2,1) as a proposal distribution

**Key Steps:**
- Generate a candidate sample from Gamma(2,1)
- Accept or reject the sample based on the calculated acceptance criterion

## Repository Files

- **RVG.Rmd**: Contains all the code for generating the random variables
- **RVG.pdf**: Knitted pdf of the rmd file
