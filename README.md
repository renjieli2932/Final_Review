# Final Review Questions
MECS 4602 Final Review

***Q1. What are the conditions for a 3x3 matrix to represent a valid rotation in 3D space?***

1. It needs to be orthonormal.
2. $|R|$ = 1 ( determinant equal to 1 )
3. $R^{-1} = R^T $



***Q2. What is one advantage of representing a 3D rotation as a quaternion as opposed to a rotation matrix?***


When the number of the variables that a rotation matrix contains is big (e.g. a total of 9 variables), the matrix itself will be complicated and such much extra information is a drawback particularly for applications where storage space is a premium. But quaternion only has 4 variables.


***Q3. How is the rank of a matrix defined?***

The dimensionality of $im(A)$ is equal to the rank of $A$.

the **column rank** of a matrix is equal to the maximum number of linearly independent column vectors.

the **row rank** of a matrix is equal to the maximum number of linearly independent row vectors.

column rank = row rank = **rank(A)**


***Q4. What is the rank-nullity theorem?***

$dim(im(A)) + dim(null(A)) = n$
$rk(A) + dim(null(A)) = n$

$n$ is the number of columns of $A$.

When m>n or m=n , if matrix is full-rank , dim(null) = 0, if matrix is not full-rank, then dim(null)>0.

When m < n, matrix always has a non-0 nullspace , dimensionality is at least n-m.


***Q5. When performing Singular Value Decomposition $A=U\Sigma V^{T}$,what is the structure of the $\Sigma$ matrix and what does it tell us about the rank of $A$ ?***

1. $\Sigma \in R^{m\times n}$ is a diagonal matrix, with diagonal entries in descending order.The entries on the diagonal of $\Sigma$ are called **singular values**. It has exactly $r$ non-zero entries, where $r = rk(A)$.

2. By counting the number of non-zero singular values, we will know the rank of the matrix.


***Q6. For a full-rank matrix $A \in R^{m \times n}$ how many exact solutions does the linear system $Ax=b$ have for any $ b \in R^m $ in each of the following cases: m>n,m=n and m < n?***


<ins>***I DO NOT UNDERSTAND THE CONTENT IN THE HANDOUT!!***</ins>




***Q7. If a robot arm is operating in 3D space, what is the smallest number of joints it must have in order to have a redundancy in <ins>any</ins> configuration? Explain why that is the case.***



***Q8. How can we tell that a robot arm is in a singular configuration?***


***Q9. What are the practical implications of a robot arm being in a singular configuration?***

***Q10. How many dimensions does the configuration space of the Kuka LWR arm have?***

It has seven dimensions, for there are seven revoluted joints.

***Q11. What is the main advantage of the $A^{*}$ algorithm compared to Dijkstra's algorithm?***

$A^{*}$ algorithm uses a heuristic to estimate how long the path from a cell to the goal could be . This makes this algorithm much faster in practise.( Though in worst case, it performs as bad as Dijkstra's algorithm.)


***Q12. Which of the following algorithms guarantees that it will return the shortest possible path between the start and the goal:Dijkstra's,A,RRT,PRM?***

Dijkstra's and A star algorithm.


***Q13. If a joint trajectory as a function of time is composed exclusively of straight line segments, why is the trajectory impossible to execute on real robots?***

Linear interpolation provides continuous position , but discontinuous velocity and acceleration. 

Specifically, we want the robot to immediately stop right at the goal point. If the joint trajectory is composed exclusively of straight line segments, it means the acceleration is infinite, which is impossible to execute on real robots.


