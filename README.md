# BOMILP-instances-for-Maximum-Multiplicative-Programming
Set of solved instances using BOMILP-Branch&Bound-Maximum-Miltilplicative-Programming.cpp
# Instances
We generated two sets of instances each with 80 randomly generated instances. In both sets, 50% of all the variables are constinuous. However in mixed-integer set, there is no binary variable, i.e. half of the variables are continuous and the other half are integers. In mixed-binary set, there is no integer variables, i.e. hald of the variables are contuous and the rest are binaries. Each set of instances contains 16 subclasses of instances based on the dimensions of the matrix A, where A is an M*N matrix, and each subclass contains 5 instances. To be specific, we assumed that m is in {200, 400, 800, 1600} and n=a*m where a is in {0.5, 1, 1.5, 2}. The sparsity of matrix A is 50%. The components of vector b and the entries of matrix A are randomly drawn from discrete uniform distributions [50, 200] and [1, 30], respectively. We set the vector d equal to zero. The sparsity of each row of the matrix D was also set to 50% and its components were drawn randomly from a discrete uniform distribution [1, 10].
It should be noted that, since all constraints are inequality constraints and all coefficients of matrix A are nonnegative, the feasible regions are bounded.

# instance.LP
Each instance is written as a CPLEX LP file as follows,



# Supporting and Citing

The software in this ecosystem was developed as part of academic research. If you would like to help support it, please star the repository as such metrics may help us secure funding in the future. We would be grateful if you could cite:
