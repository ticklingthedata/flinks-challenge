# 1. Linear Algebra:

## Vectors:

* Abstractly, vectors are objects that can be added together to form new vectors and that can be multiplied by scalars (i.e., numbers), also to form new vectors.

* Concretely, vectors are points in some finite-dimensional space. Although you might not think of your data as vectors, they are often a useful way to represent numeric data.

* For example, if you have the heights, weights, and ages of a large number of people, you can treat your data as three-dimensional vectors [height, weight, age].

* If two vectors v and w are the same length, their sum is just the vector whose first element is v[0] + w[0], whose second element is v[1] + w[1], and so on. (If they’re not the same length, then we’re not allowed to add them.)

* The scalar product is the result of multiplying each element of the vector by a scalar.

* the dot product of two vectors is the sum of their componentwise products.

* If w has magnitude 1, the dot product measures how far the vector v extends in the w direction. For example, if w = [1, 0], then dot(v, w) is just the first component of v. Another way of saying this is that it’s the length of the vector you’d get if you projected v onto w.

* Magnitude of a vector: square root the sum of squares.

* Disctance between 2 vectors: square root of the sum of squares of (vi-wi).

## Matrices:

* A matrix is a two-dimensional collection of numbers.
* If A is a matrix, then A[i][j] is the element in the ith row and the jth column.
* Matrix A shape: A has len(A) rows and len(A[0]) columns.
* If a matrix has n rows and k columns, we will refer to it as an n × k matrix (think of each row of an n × k matrix as a vector of length k, and each column as a vector of length n).
* A Matrix can be used to represent a dataset consisting of multiple vectors, simply by considering each vector as a row of the matrix. 
* A n × k matrix to represent a linear function that maps k-dimensional vectors to n-dimensional vectors.
* Matrices can also be used to represent binary relationships.

# 2. Statistics

## Central Tendencies:

* Mean (or average): which is just the sum of the data divided by its count.
* Median: which is the middle-most value (if the number of data points is odd) or the average of the two middle-most values (if the number of data points is even).
* Mode: or most common value(s).

## Dispersion:

* Range: which is just the difference between the largest and smallest elements.
* Variance: which is the expectation of the squared deviation of a random variable from its mean.
* Standard deviation: which is the a measure of the amount of variation or dispersion of a set of values.

## Correlation:

* Covariance: whereas variance measures how a single variable deviates from its mean, covariance measures how two variables vary in tandem from their means.
* Correlation: which divides out the standard deviations of both variables.

## Simpson’s Paradox:

* Correlations can be misleading when confounding variables are ignored.

## Some Other Correlational Caveats:

* A correlation of zero indicates that there is no linear relationship between the two variables. However, there may be other sorts of relationships.
* Correlation tells you nothing about how large the relationship is.

## Correlation and Causation:

* If x and y are strongly correlated, that might mean that x causes y, that y causes x, that each causes the other, that some third factor causes both, or nothing at all.

# 3. Probability:

Think of probability as a way of quantifying the uncertainty associated with events chosen from some universe of events.

## Dependence and Independence:

* Two events E and F are dependent if knowing something about whether E happens gives us information about whether F happens (and vice versa). Otherwise, they are independent.

* Mathematically, we say that two events E and F are independent if the probability that they both happen is the product of the probabilities that each one happens: P(E,F)=P(E)P(F)

## Conditional Probability:

Think of this as the probability that E happens, given that we know that F happens.

* If they E and F are not necessarily independent (and if the probability of F is not zero), then we define the probability of E “conditional on F” as: P(E|F)=P(E,F)/P(F)


## Bayes’s Theorem:

This of this as a way of “reversing” conditional probabilities.

* Used to know the probability of some event E conditional on some other event F occurring, when we only have information about the probability of F conditional on E occurring: 

* Concretely: P(E|F)=P(F|E)P(E)/[P(F|E)P(E)+P(F|¬E)P(¬E)]

## Random Variables:

* A random variable is a variable whose possible values have an associated probability distribution.
* The associated distribution gives the probabilities that the variable realizes each of its possible values.
* Expected value of a random variable: which is the average of its values weighted by their probabilities.