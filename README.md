# Cake Eating Problem

The cake eating problem is to maximize the discounted flow of utility derived from eating cake

<img src="https://render.githubusercontent.com/render/math?math=\large\max\intop_{0}^{+\infty}e^{-\rho t}u\left(c\left(t\right)\right)dt">

subject to the constraing that the total cake eaten cannot exceed the initial stock of cake

<img src="https://render.githubusercontent.com/render/math?math=\large\intop_{0}^{+\infty}c\left(t\right)dt\leq K">

## Exact Solution with CES Utility Function

If we assume that the utility function takes the form

<img src="https://render.githubusercontent.com/render/math?math=\large\\u\left(c\right)=\frac{c^{1-\sigma}-1}{1-\sigma}">

then the problem can be solved using pen and paper. The exact solution is given by

<img src="https://render.githubusercontent.com/render/math?math=\large\\V\left(K\right)=\frac{\sigma}{\rho}\frac{\left(\frac{\rho}{\sigma}K\right)^{1-\sigma}-1}{\left(1-\sigma\right)}">

and

<img src="https://render.githubusercontent.com/render/math?math=\large\\c\left(K\right)=\frac{\rho}{\sigma}K">
