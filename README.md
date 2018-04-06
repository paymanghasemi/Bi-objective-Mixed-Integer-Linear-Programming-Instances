# Bi-objective Mixed Integer Linear Programming Instances
Set of solved instances using BOMILP-MMP.cpp
# Instances
We generated two sets of instances each with 80 randomly generated instances. In both sets, 50% of all the variables are constinuous. However in mixed-integer set, there is no binary variables, i.e. half of the variables are continuous and the other half are integers. In mixed-binary set, there is no integer variables, i.e. half of the variables are continuous and the rest are binaries. The problems are as follows,

![Images](Images/problem.jpg)

Each set of instances contains 16 subclasses of instances based on the dimensions of the matrix A, where A is an M * N matrix, and each subclass contains 5 instances. To be specific, we assumed that m is in {200, 400, 800, 1600} and n=a*m where a is in {0.5, 1, 1.5, 2}. The sparsity of matrix A is 50%. The components of vector b and the entries of matrix A are randomly drawn from discrete uniform distributions [50, 200] and [1, 30], respectively. We set the vector d equal to zero. The sparsity of each row of the matrix D was also set to 50% and its components were drawn randomly from a discrete uniform distribution [1, 10].
It should be noted that, since all constraints are inequality constraints and all coefficients of matrix A are nonnegative, the feasible regions are bounded.

# instance.LP

The instances are written as CPLEX LP file as follows,

![Images](Images/instance.jpg)

where f(x) is an arbitrary function which can be removed, x1 and x2 are the objective functions respresenting the y1 and y2 of the problem, and the rest of x are the decision variables.

Real, binary, and integer decision variables are distributed randomly in the instances, and therefore, there is no pattern for separating their indexes.
# Supporting and Citing

The instances were generated as part of academic research. If you would like to help support it, please star the repository as such metrics may help us secure funding in the future. We would be grateful if you could cite:

Ghasemi Saghand, P., Charkhgard, H., Changhyun, K., A Branch-and-Bound Algorithm for a class of Mixed Integer Linear Maximum Multiplicative Programs: A Multi-objective Optimization Approach
