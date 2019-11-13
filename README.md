# MMP_Instance_Generator
An executive program to generate instances for Minimum Multiplicative Programming (MMP) problems. This problem can be formulated as follows:

$ min_{x,y} {prod(y); y = Cx+d , Ax>=b, y>=0, x in {R^n_R, Z^n_Z, B^n_B} } $, where n = n_R + n_Z + n_B is the number of variables in different types including real, integer, and binary. 

By runningthe following command in command window, forut matrices of parameters will be generated.
"./MMP_Instance_Generator p m n ASparcity CSparcity n_R n_Z n_B"

Inputs:
p => the number of multiplicative terms or objectives,
m => the number of constraints,
n => the number of variables,
ASparcity => the sparcity of matrix A in the problem,
CSparcity => the sparcity of matric C in the problem,
n_R => the number of real variables,
n_Z => the number of integer variables,
n_B => the number of binary variables.

Outputs:
The outputs will be generated in the form of text files with the following names;
A => matrix A or coefficient matrix in the problem,
b => vecotr b or right-hand side values in the problem,
C => matrix C or objective coefficients in the problem, 
d => vector d or fixed values of linear terms in the problem. 
VariableDef => a vector with three values determining the number of variables from each type. 


