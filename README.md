# Final Review Questions
MECS 4602 Final Review

***Q1. What are the conditions for a 3x3 matrix to represent a valid rotation in 3D space?***

My Answer: 

1. It needs to be orthonormal.
2. $|R|$ = 1 ( determinant equal to 1 )
3. $R^{-1} = R^T $



***Q2. What is one advantage of representing a 3D rotation as a quaternion as opposed to a rotation matrix?***

My Answer:

When the number of the variables that a rotation matrix contains is big (e.g. a total of 9 variables), the matrix itself will be complicated and such much extra information is a drawback particularly for applications where storage space is a premium. But quaternion only has 4 variables.


***Q3. How is the rank of a matrix defined?***

My Answer:

The dimensionality of $im(A)$ is equal to the rank of $A$.

the **column rank** of a matrix is equal to the maximum number of linearly independent column vectors.
the **row rank** of a matrix is equal to the maximum number of linearly independent row vectors.
column rank = row rank = **rank(A)**