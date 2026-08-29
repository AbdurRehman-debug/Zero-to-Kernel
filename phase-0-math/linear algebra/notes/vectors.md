# Topic -  Vectors


## what even are they?

vectors are mathematical objects that have both magnitude and direction. They can be represented in various forms, such as arrows in a geometric space or as ordered lists of numbers (coordinates) in a coordinate system.

### row pIcture of a vector:


- The row picture of a linear system shows each individual equation as a geometric line or plane, where the final solution is the point where all these shapes cross each other.How the Row Picture WorksEach row is a rule: Every single equation in the system acts as an independent condition that the variables must satisfy.2D Space (Two variables): Each equation draws a straight line on a flat graph. The solution is the single point where the lines cross.3D Space (Three variables): Each equation draws a flat plane in three-dimensional space. The solution is the point, line, or plane where all the individual planes intersect.No solution case: If the lines or planes are parallel and never cross each other, the system has no solution


### Column Picture of a Vector:
- The column picture of a linear system looks at the equations vertically, combining vector columns to reach a target vector.Instead of looking for where lines cross, you are trying to find how much of each vector you need to mix together to arrive at your final destination.How the Column Picture WorksColumns are directions: Each variable (like \(x\) or \(y\)) controls how far you move along a specific vector column.Linear Combination: You multiply each column vector by its respective variable and add them together.

## Linear Combination of Vectors:
- A linear combination of vectors is an expression where you multiply each vector by a scalar (a real number) and then add the results together.or simply you multiply. This allows you to create new vectors from existing ones, and it's a fundamental concept in linear algebra for understanding vector spaces and transformations.



## span of a vector:
```
the span of a vector refers to the set of all possible linear combinations of that vector. In other words, if you have a vector v, the span of v includes all vectors that can be formed by multiplying v by any scalar (real number). This concept is fundamental in linear algebra, as it helps define the space that a vector occupies and how it can be combined with other vectors to form new vectors.
```

## basis of a coordinate system:
```
 A basis of a coordinate system is a set of linearly independent vectors that span the entire space. In other words, any vector in that space can be expressed as a unique linear combination of the basis vectors. The number of vectors in the basis corresponds to the dimension of the space. For example, in 2D space, a common basis is the set of unit vectors along the x-axis and y-axis, while in 3D space, a common basis is the set of unit vectors along the x-axis, y-axis, and z-axis.
```


## Row Rank:
- Row rank is the maximum number of linearly independent rows in a matrix. It tells you how many unique directions or constraints the rows provide. If the row rank equals the number of rows, all rows are independent; if it's less, some rows can be expressed as combinations of others.

## Column Rank:
- Column rank is the maximum number of linearly independent columns in a matrix. It indicates how many unique directions or dimensions the columns span. If the column rank equals the number of columns, all columns are independent; if it's less, some columns can be expressed as combinations of others.


## Rank theorem:
column rank and row rank are always equal for any matrix, a fundamental result in linear algebra known as the rank theorem. This means that the number of independent rows is the same as the number of independent columns, providing a consistent measure of the matrix's dimensionality.



## matrix Factorization and Vectors:
- Matrix factorization is a technique where a matrix is broken down into simpler, constituent matrices. A = CR, where C contains independent columns of A and R contains the combinations needed to reconstruct the original columns. This factorization helps in understanding the structure of the matrix and its column space, which is the set of all possible vectors that can be formed by linear combinations of the columns of A.
