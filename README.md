# 2D-Array

THEORY

A multi-dimensional array can be termed as an array of arrays that stores homogeneous data in tabular form. Data in multidimensional arrays is generally stored in row-major order in the memory.

The general form of declaring N-dimensional arrays is shown below.

Syntax:


data_type array_name[size1][size2]....[sizeN];
data_type: Type of data to be stored in the array.
array_name: Name of the array.
size1, size2,…, sizeN: Size of each dimension.
Examples:

Two dimensional array: int two_d[10][20];

Three dimensional array: int three_d[10][20][30];
Size of Multidimensional Arrays:
The total number of elements that can be stored in a multidimensional array can be calculated by multiplying the size of all the dimensions.
For example:

The array int x[10][20] can store total (10*20) = 200 elements.
Similarly array int x[5][10][20] can store total (5*10*20) = 1000 elements.
To get the size of the array in bytes, we multiply the size of a single element with the total number of elements in the array.
For example:

Size of array int x[10][20] = 10 * 20 * 4  = 800 bytes.      (where int = 4 bytes)
Similarly, size of int x[5][10][20] = 5 * 10 * 20 * 4 = 4000 bytes.      (where int = 4 bytes)
The most commonly used forms of the multidimensional array are:

Two Dimensional Array
Three Dimensional Array
Two-Dimensional Array in C
A two-dimensional array or 2D array in C is the simplest form of the multidimensional array. We can visualize a two-dimensional array as an array of one-dimensional arrays arranged one over another forming a table with ‘x’ rows and ‘y’ columns where the row number ranges from 0 to (x-1) and the column number ranges from 0 to (y-1).
Declaration of Two-Dimensional Array in C
The basic form of declaring a 2D array with x rows and y columns in C is shown below.

Syntax:

data_type array_name[x][y];
where,

data_type: Type of data to be stored in each element.
array_name: name of the array
x: Number of rows.
y: Number of columns.

ALGORITHM

Take matrix input from user and display it
1.We first get the number of rows and columns from the user.

2.We then declare a 2D array (matrix) with the specified dimensions.

3.We use nested loops to iterate through the matrix and input the elements from the user.

4.Finally, we use another set of nested loops to display the matrix.

5.Compile and run this C++ program, and it will take matrix input from the user and display it on the screen.

Addition of matrix
Start

Declare variables for the number of rows and columns for the matrices (let's call them rows and cols).

Get the dimensions (rows and cols) of the matrices from the user.

Declare two 2D arrays (matrices) of size rows x cols: matrix1 and matrix2.

Input the elements of matrix1 and matrix2 from the user using nested loops.

Declare another 2D array (resultMatrix) of the same size (rows x cols) to store the result.

Perform matrix addition using nested loops:

For each element at position (i, j) in resultMatrix:
resultMatrix[i][j] = matrix1[i][j] + matrix2[i][j]
Display the resultMatrix, which contains the sum of the two matrices.

End

Multiplication of Matrix
Start

Declare variables for the number of rows and columns for the first matrix (matrix1Rows, matrix1Cols) and the second matrix (matrix2Rows, matrix2Cols).

Get the dimensions (rows and columns) of matrix1 and matrix2 from the user.

Check if matrix1Cols is equal to matrix2Rows. If not, exit the program with an error message because matrix multiplication is not possible.

Declare three 2D arrays:

matrix1 of size matrix1Rows x matrix1Cols
matrix2 of size matrix2Rows x matrix2Cols
resultMatrix of size matrix1Rows x matrix2Cols
Input the elements of matrix1 and matrix2 from the user using nested loops.

Perform matrix multiplication using three nested loops:

For each element at position (i, j) in resultMatrix:
Initialize resultMatrix[i][j] to 0.
Perform the dot product of the ith row of matrix1 and the jth column of matrix2 to calculate resultMatrix[i][j].
Display the resultMatrix, which contains the product of the two matrices.

End

Diagonal Addition
Start

Declare variables for the number of rows and columns of the matrix (rows and cols).

Get the dimensions (rows and cols) of the matrix from the user.

Declare a 2D array (matrix) of size rows x cols to store the matrix elements.

Input the elements of the matrix from the user using nested loops.

Initialize a variable (diagonalSum) to 0. This variable will store the sum of the diagonal elements.

Use a loop to iterate through the diagonal elements of the matrix:

For each element at position (i, i), add matrix[i][i] to diagonalSum.
Display the value of diagonalSum, which contains the sum of the diagonal elements.

End

Transpose of Matrix
Start

Declare variables for the number of rows and columns of the original matrix (rows and cols).

Get the dimensions (rows and cols) of the original matrix from the user.

Declare a 2D array (originalMatrix) of size rows x cols to store the original matrix elements.

Input the elements of the original matrix from the user using nested loops.

Declare a new 2D array (transposeMatrix) of size cols x rows to store the transposed matrix.

Use nested loops to copy the elements from the original matrix to the transposed matrix with swapped rows and columns:

For each element at position (i, j) in the original matrix, assign originalMatrix[i][j] to transposeMatrix[j][i].
Display the transposed matrix (transposeMatrix).

End

Campare elements of first row to the second row
Start

Declare variables for the number of rows and columns of the matrix (rows and cols).

Get the dimensions (rows and cols) of the matrix from the user.

Declare a 2D array (matrix) of size rows x cols to store the matrix elements.

Input the elements of the matrix from the user using nested loops.

Initialize a boolean variable (rowsEqual) to true. This variable will be used to track if the elements of the first row are equal to the corresponding elements of the second row.

Use a loop to compare the elements of the first row to the second row:

For each column index (i) from 0 to cols-1:
If matrix[0][i] is not equal to matrix[1][i], set rowsEqual to false and break out of the loop.
If rowsEqual is true, display a message indicating that the two rows are equal. Otherwise, display a message indicating that the two rows are not equal.

End

EXPECTED OUTPUT

Take matrix input from user and display it
enter the values in the matrix:
2
2
2
4
5
6
the given matrix is:
2 2
2 4
5 6


Addition of matrix
Enter elements of 1st matrix:
Enter element a11 : 11
Enter element a12 : 12
Enter element a21 : 4
Enter element a22 : 5

Enter elements of 2nd matrix:
Enter element b11 : 5
Enter element b12 : 5
Enter element b21 : 6
Enter element b22 : 7

Sum of two matrix is:
16  17
10  12


Multiplication of Matrix
Enter rows and columns for first matrix:  2
2
Enter rows and columns for second matrix:  2
2

Enter elements of matrix 1: Enter element a11 : 1
Enter element a12 : 1
Enter element a21 : 1
Enter element a22 : 1

Enter elements of matrix 2: Enter element b11 : 1
Enter element b12 : 1
Enter element b21 : 1
Enter element b22 : 1

Output Matrix:   2 2  2 2


Enter the number of rows and columns for matrix1: 2
2
Enter the number of rows and columns for matrix2: 2
2
Enter elements of matrix1:
2
1
2
2
Enter elements of matrix2:
2
3
1
1
Result of matrix multiplication:
5 7
6 8


Diagonal Addition
the matrix is:
1 3 4
5 6 7
8 9 1
the  transposed matrix is:
1 5 8
3 6 9
4 7 1


Transpose of Matrix
Enter elements into the matrix 
1 3 4
5 6 7
8 9 1
Sum of Left Diagonal: 8
Sum of Right Diagonal: 18

Compare elements of first row to the second row
Enter the number of rows and columns: 2
2
Enter elements of the matrix:
1 2
1 2
The elements of the first row are equal to the corresponding elements of the second row.
