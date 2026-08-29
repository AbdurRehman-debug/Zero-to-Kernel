# Week 1 — Days 1 - 7



---

# Day 1 — Sunday , 22 August 2026
# Phase: 0A-Linear Algebra


---

## 📖 What I Studied
``` 
Vectors that what even are they?
watched 3 blue 1 browns video which stated that there are 3 primary views on a vector

watched MIT 18.06SC Linear Algebra Lecture 1: The Geometry of Linear Equations

watched MIT 18.065 The Column Space of Ax contains All Vectors Ax





```




---

## 💡 What I Understood
### From 3 Blue 1 Brown's video, I understood that there are 3 primary views on a vector:

### Physics: Vectors are arrows in space, defined by length and direction 
### Computer Science: Vectors are ordered lists of numbers, useful for modeling data 
#### Mathematics: A generalization that emphasizes the operations of addition and scalar multiplication 

And Also

### Vector Addition:
joining the tail of one vector to the head of another vector, and drawing a new vector from the tail of the first to the head of the second.

![alt text](images/image.png)


### Scalar Multiplication:
Multiplying a vector by a scalar (a real number) changes the length of the vector but not its direction. If the scalar is negative, the direction of the vector is reversed.

### From MIT 18.06 Linear Algebra Lecture 1: The Geometry of Linear Equations:


three key perspectives for understanding the equation 

#### The Row Picture: 
This focuses on viewing each equation individually as a line (in 2D) or a plane (in 3D). The solution is the point where these lines or planes intersect.


This view treats each equation as an individual line (in 2D) or plane (in 3D). You are looking for the exact single point where all these lines or planes cross each other. If you have two equations, you are finding where two lines intersect on a graph.

#### The Column Picture: 
This is highlighted as the most important perspective. It views the system as a linear combination of the columns of matrix 
 to produce the vector 

 This view is about linear combinations. Instead of focusing on lines or planes, you look at the columns of the matrix as separate vectors. The goal is to figure out how much of each column you need to add together (the "combination") to reach your target vector 
. Imagine you are trying to reach a specific destination by taking a certain number of steps in one direction, then a certain number of steps in another direction.
#### The Matrix Form: 
The algebraic way to represent the system using matrix 
, the unknown vector 
, and the right-hand side vector 


### From MIT 18.065 : The Column Space pf Ax contains All Vectors Ax: 

#### Column Space:
 it is All the vectors that can be expressed as a linear combination of the columns of a matrix. In other words the column spoace of A is the set of all possible vectors you can reach by scaling and adding together the columns of A. If you think of each column as a direction you can move in, the column space is like the entire area you can cover by moving in those directions.

 depending on the independence of the columns of A, the column space can be a line, a plane, or even fill up the entire space. If the columns are independent, you can reach more unique points in space. If they are dependent, your movement is restricted to a smaller area.

 #### rank of  matrix:
 The rank of a matrix is defined as the dimension of its column space, which corresponds to the number of independent columns in the matrix

#### Matrix Factorization (A=CR): 
A central theme of the lecture was  the decomposition of a matrix 
 into a matrix  C
 (containing independent columns of 
) and R 
 (containing the combinations needed to reconstruct the original columns)

![alt text](<images/matrix factorization.png>)


#### Fundamental Theorem:
 The lecture highlights the proof that the column rank equals the row rank, which is a fundamental theorem in linear algebra. This means that the number of independent columns in a matrix is always equal to the number of independent rows, providing a deep insight into the structure of matrices.





---


## Day 2 — Monday, August 24, 2026





### 📖 What I Studied

studied the following topics:
```
- Vectors and linear combinations specfically from professor Gilbert Strang's Book "Introduction to Linear Algebra" 5th edition, Chapter 1: Vectors and Linear Combinations Topic(1.1) and solved problem set 1.1
```

---

### 💡 What I Understood

linear combinations,dependence and independence of vectors, span of a set of vectors, and the geometric interpretation of these concepts. I also learned how to determine if a set of vectors is linearly independent or dependent by using the concept of linear combinations.




---



## Day 3 — Saturday, 29 August 2026



---

### 📖 What I Studied

```
Linear combinations, span and basis vectors from 3Blue 1 Brown's video "Linear Combinations, Span, and Basis Vectors" 
 i watched till 29:20 of MIT 18.06sc Elimination With Matrices Lecture 2: Elimination with Matrices 
```


---

### 💡 What I Understood

- From the 3Blue 1 Brown's video, I understood that linear combinations involve combining vectors using scalar multiplication and addition. The span of a set of vectors is the collection of all possible linear combinations of those vectors, which can form a subspace in the vector space. Basis vectors are a set of linearly independent vectors that span a vector space, meaning they can be used to represent any vector in that space through linear combinations. changing the basis can change the whole corrdinate sytem and the representation of vectors within that space.
also i understood about linear dependence and independence of vectors, which is crucial for determining the span and basis of a vector space. A set of vectors is linearly independent if no vector in the set can be expressed as a linear combination of the others; otherwise, they are linearly dependent. This understanding is fundamental in linear algebra and has applications in various fields, including computer graphics, data analysis, and machine learning.  ``` two dependent  vectors form a line and add zero information, 2 independent vectors form a plane, and three independent vectors form2 the entire 3D space.```



- From the MIT lecture, I learned about the process of elimination with matrices, which is a fundamental technique in solving systems of linear equations.and specificaly multiplication fo a matrix with a column vector leads to a linear combination of the columns of the matrix and mutlitplication of a matrix with a row vector leads to a linear combination of the rows of the matrix. and specifically there was guass elimination whihc is a systematic method mentioned in which we eliminate the entries below pivots(leading entries) to transform the matrix into an upper triangular form, making it easier to solve the system of equations. This process involves a series of row operations, including swapping rows, multiplying a row by a non-zero scalar, and adding or subtracting multiples of one row from another. The goal is to simplify the matrix while preserving the solutions to the system of equations. Once in upper triangular form, back substitution can be used to find the values of the variables.![alt text](images/linear%20combination%20of%20rows%20and%20columns.png)


```but the improtant thing  i learnt is the elementary row operations we typically perform are actually matrx mutliplicaton underneath and this cleared abstrcation for me and i understood that the elementary row operations can be represented as multiplication by an elementary matrix, which is a special type of matrix that performs a specific row operation when multiplied with another matrix. ```


![alt text](images/intituion1.png)
![alt text](images/page2%20intition.png)


    
---


## Week 1 Summary:

**Topics covered:**
 

**Biggest thing I learned:**

**Biggest thing still confusing me:**

