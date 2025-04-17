Notes for Machine Learning Foundations: Linear Algebra

CHP 1: Introduction to Linear Algebra:

• Defining Linear Algebra: 
  - Algebra: A branch of mathematics that uses mathematical statements to describe relationships between things that may vary.
  - Linear Algebra: A branch of mathematics that lets you concisely describe coordinates and interactions of planes in higher dimensions and perform operations on them.
  -  A.K.A., Linear Algebra is the study of vectors and linear functions.

• Main Building Blocks and Areas:
  - Systems of linear equations, vectors and matrices, linear transformations, determinants, and vector spaces (the study of vectors and linear functions).

• Machine Learning: (Also taught in Intro to Artificial Intelligence: 4.2.)
  - Dealing with vectors and matrices.
  - Large data sets and matrices.
  - Split data set into training and testing data set.
• Applications of Linear Algebra in ML:
  1. Data set and data files: data set is either a matrix or vector.

  2. Images and photographs.

  3. Data preparation: Dimensionality reduction or one hot encoding.

  3.1. Dimensionality Reduction:
    - Data sets are represented as matrices.
    - Use matrix factorization methods to reduce it into its constituent parts.
    - Example below:

        a11 |  a12  | a13
        a21 |  a22  | a23
    A = a31 |  a32  | a33
         .  |   .   |  . 
         .  |   .   |  .
         .  |   .   |  .
        an1 |  an2  | an3


  3.2. One Hot Encoding: 
    - Used when working with categorical data.
    - Example: Class labels for classification problems, or categorical input variables (below).
    - (It's common to encode categorical variables to make them easier to work with).

     |Color|        | Red |Green| Blue |
     | Red |        |  1  |  0  |   0  |      
     |Green| -----> |  0  |  1  |   0  |
     |Blue |        |  0  |  0  |   1  |
     |Green|        |  0  |  1  |   0  |


  4. Linear Regression:
    - The most common way of solving linear regression is via a least square optimization (matrix factorization method):
    - Example below:

             3   0 (circled by blue) 
       A =  -4   2 (circled by red)
             3  -5 (circled by green)


  5. Regularization:
    - Used to prevent the model from overfitting.
    - Overfitting: used when a model is too close a fit for the available data to the point that it does not perform well w/ any new or outside data.
    - In a nutshell, overfitting is used to encourage a model to minimize the size of coefficients while it's being fit on data.

      VALUES                                                                      
        ↑
        |        
        |         _*_    _*_   _*_    _*_
        |       */   \ /   \  /   \  /   │
        |      *└---┐* *    *     *  *┌---┘*                 ■
        |     *┌----┘*               *└----┐*          *┌----┘*
        |     *└-┐*                    *┌--┘*         *└---┐*
        |   *┌--┘*                     *└---┐*      *┌----┘*                        
        |   *└-┐*                       *┌--┘*     *└---┐* 
        |  *┌--┘*                       *└---┐*  *┌-----┘*
        |  *└-┐*                         *┌--┘*  *└-┐*
        |*■---┘*                         *└--┐ ┌----┘* 
        |                                     *
        |-------------------------------------> TIME         
                       OVERFITTED MODEL                                                  
        
      VALUES
        ↑                                                                   
        |                                                          
        |         *  *  *  *  *  *  *                                         
        |        * ⎾ -  -  -  -  -  ⏋*                            
        |       * / *  *  *  *  *  * \ *              ■                   
        |      * │ *                * | *         *  / *                          
        |     * / *                  * \ *      *  / *              
        |    * | *                    * | *     * | *              
        |   * / *                      * \ *   * / *                 
        |  * │ *                        * │| *  * │ *                 
        | * / *                          * \ * * / *               
        |* ■┘*                             *  ⏘  *      
        |                                     *
        |-------------------------------------> TIME                     
                                                                              
                    GOOD FIT / ROBUST MODEL                                         


  6. Principal Component Analysis: Method for automatically reducing the number of columns of a dataset:
    - Used in Machine Learning to create a projection of high-dimensional data for visualizations and training models.
    - The core of PCA methods is the matrix factorization method.
    - Example:

            ⎾  3  0  4  !6  (blue colored)
        A = | -4  2  2   !2  (red colored)
            ⎿  3 -5  4  !2  (green colored)


  7. Latent Semantic Analysis (LSA): A form of data preparation used in natural language processing, a subfield of ML for working with text data.
    - i.e.: Keyword Categorization
      - Documents are usually represented as large matrices of word occurrences. Then, apply matrix factorization of methods to them in order to be able to 
        easily compare, query, and use them as basis for the ML model.


  8. Recommender Systems: Predictive modeling problems involving product recommendations.
    - i.e.: Amazon Shopping:
      - Used each time you buy something on Amazon and you get recommendations of products based on your previous purchases.


  9. Deep Learning: Specific subfield of ML:
    - Scaled up to multiple dimensions, deep learning methods work w/ vectors, matrices, and tensors of inputs and coefficients

| Question 1/3: What are the main building blocks of linear algebra? 
|A: systems of linear equations, vectors and matrices, linear transformations, determinants, and vector spaces
|
| Question 2/3: Modeling data with many features is challenging and it's hard to know which features of data are relevant and  
|               which are not. One of the methods for automatically reducing the number of columns of a dataset is _____.
|A: Principal Component Analysis
|
| Question 3/3: _____ is a form of data preparation used in natural language processing, a subfield of ML for working with text data.
|A: Latent Semantic Analysis


CHP 2: Vectors Basics:

• Introduction to Vectors:

  - Difference between Scalar and Vector:
    - Scalar: A number, denoted with a lowercase symbol, such as a or b. For example, weight/200 lbs, temperature/55 Fahrenheit, and blood pressure/120 by 80.
    - Vectors: Lowercase bolded Roman letters, an arrow printed on top (→α). By definition, a vector is an ordered list of numbers, for example, α = [8 4 5 2 7]
      - Vector Characteristics: 
        - Dimensionality: It's called the length or the shape of the vector in Python.
          - The number of elements in the vector: α = [1 9 5 8 7 2 4 3 6], which in this case, the dimensionality is 9
 
                                                                                     |1|
        - Orientation: Column orientation (tall) or row orientation (flat/wide): b = |2|  or c = [1 2 3]
                                                                                     |3| 

      - Examples of Vectors:           |1|
        - x is a 3D column vector: x = |2|  
                                       |3|
         
        - y is a 2D column vector: y = |1|
                                       |2|

        - z is a 3D row vector: z = [1 2 3]

        - If you use vectors for storing data, orientation usually doesn't matter. But when performing arithmetic operations it's extremely important,
          since the wrong orientation leads to unexpected results or even errors.
      
      - By convention, vectors are column-oriented*. If they're row-oriented, then they are written with v^t which indicates the transpose operation 
        which converts a column vector into a row vector**.
             |1|
        *v = |2|        
             |3|
             |4|

        **v^t = [1 2 3 4]

        - If we want to represent the vector graphically, see below:

       y ↑ 
         |
         |       α
         |----------------┒← Head
         |              ↗ ┆                            - →V is the vector, and in our case, α and b are scalars denoting the magnitude of →v in
         |            ̷    ┆                              in horizontal and vertical directions. The algebraic interpretation of a vector is an 
         |    →     ̷      ┆                              ordered list of numbers. The geometric interpretation of a vector is a line that has 
         |    v   ̷        ┆  b                           specific length and direction also called an angle. It's computed relative to the 
         |      ̷          ┆                              positive X-axis.
         |    ̷            ┆                              
         |  ̷              ┆                            - The two points of a vector are called the tail, where the vector starts, and the head 
         |̷                ┆                              that has the tipo of the arrow tip, where it ends.
  Tail → ┕--------------------------------→
                                          x

        - Vector Representation: We can represent vectors in Python using several data types. The simplest way to represent a vector is with a list.
          - vectorAsList = [1,2,3,4,5]
            - However, as many linear algebra operations don't work on Python list we can create vectors as NumPy arrays called ND arrays. See below.
       
          - vectorasArray = np.array([1,2,3,4,5])
            - This array above is an orientationless array, meaning it's neither a row nor a column vector. In NumPy, we indicate orientation with brackets. See below.
       
          - rowVector = np.array([[1,2,3,4,5] ])
            - The outer brackets group all elements together in one object as an additional set of brackets indicates a row.
      
          - columnVector = np.array([[1],[2],[3],[4],[5]])
            - In the case above, we see it has only one column and five rows. 


• Vector Arithmetic:

    * Add notes here*




























Unicode characters used in this file: https://www.rapidtables.com/code/text/unicode-characters.html










         









