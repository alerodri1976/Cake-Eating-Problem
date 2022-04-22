# Cake Eating Problem
The cake eating problem is to maximize the discounted flow of utility derived from eating cake

<img src="https://render.githubusercontent.com/render/math?math=\large\max\intop_{0}^{+\infty}e^{-\rho t}u\left(c\left(t\right)\right)dt">

subject to the constraing that the total cake eaten cannot exceed the initial stock of cake

<img src="https://render.githubusercontent.com/render/math?math=\large\intop_{0}^{+\infty}c\left(t\right)dt\leq k">

## Exact Solution with CES Utility Function
If we assume that the utility function takes the form

<img src="https://render.githubusercontent.com/render/math?math=\large\\u\left(c\right)=\frac{c^{1-\sigma}-1}{1-\sigma}">

then the problem can be solved using pen and paper. The exact solution is given by

<img src="https://render.githubusercontent.com/render/math?math=\large\\v\left(k\right)=\frac{\sigma}{\rho}\frac{\left(\frac{\rho}{\sigma}k\right)^{1-\sigma}-1}{\left(1-\sigma\right)}">

and

<img src="https://render.githubusercontent.com/render/math?math=\large\\c\left(k\right)=\frac{\rho}{\sigma}k">

## Solving the Problem with Dynamic Programing
The cake eating problem can be written using the Hamilton-Jacobi-Bellman equation as

<img src="https://render.githubusercontent.com/render/math?math=\large\rho v\left(k\right)=\underset{c}{\max}\left\{ \frac{c^{1-\sigma}-1}{1-\sigma}%2B\frac{\partial v\left(k\right)}{\partial k}\frac{\partial k}{\partial t}\right\}">

where

<img src="https://render.githubusercontent.com/render/math?math=\large\frac{\partial k}{\partial t}=-c">

The first order condition is then given by

<img src="https://render.githubusercontent.com/render/math?math=\large\\c^{-\sigma}=\frac{\partial v\left(k\right)}{\partial k}">

