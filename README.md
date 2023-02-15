# Newton-Method-in-Optimization
### Newton's Method
The central problem of optimization is the minimization of functions. Let us first consider the case of univariate functions, i.e., functions of a single real variable. Given a twice differentiable function 'f', we seek to solve the optimization problem:

![image](https://user-images.githubusercontent.com/125180530/219141222-0f180129-ac9f-413e-b3f2-8e7b832c4704.png)

In each step of the solution, the method follows these two structures:

* Locally approximate function as quadratic

* Minimize this quadratic function

![image](https://user-images.githubusercontent.com/125180530/219141754-1950910d-7f14-45e1-a4e6-81ffcfad8496.png)

Newton's method approximates a function using second-order Taylor series expansion:

![image](https://user-images.githubusercontent.com/125180530/219142015-d881ab7f-be60-461e-a057-cea7d348b07e.png)

### Comparison between Gradient Descent and Newton's Method
A comparison of gradient descent (green) and Newton's method (red) for minimizing a function (with small step sizes). Newton's method uses curvature information (i.e. the second derivative) to take a more direct route.

![image](https://user-images.githubusercontent.com/125180530/219142794-4aa4b019-08b6-442d-9056-f9bd29167961.png)

Now consider the following non-convex function:

![image](https://user-images.githubusercontent.com/125180530/219143106-881fa570-2daa-4152-b2d0-ed43e92b13cf.png)

Assume the initial point (1,3). We have found the minimum of the function. 

![image](https://user-images.githubusercontent.com/125180530/219145091-d0fb8e1e-a59e-46b7-b7bb-2237b18dc12f.png)

![image](https://user-images.githubusercontent.com/125180530/219145160-34726774-271d-423c-862f-9a2c15684d70.png)

For all points in the following intervals and for step size = 0.5 we found the minimums and calculate their distance from the actual minimum value which is -36.4. Then, we classify the distances into three classes: close, far, and farther. The plot of the calculated points can be observed in the code file. 

As the minimum point is located in x1 = 0.13 and x2 = 4.26, we expect the points that have nearer x1 and x2 values to be in the 'close' class. We can conclude the same thing from the plot. Almost all the points near x1 = 0.13 and x2 = 4.26 are red which are in the 'close' class and then we can see blue points that are illustrating the points in the 'far' class and finally we can see yellow points of the 'farther' class that are also farther from the minimum point.
