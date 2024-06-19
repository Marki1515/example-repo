
public class IdentityMatrix {
Defines a public class named IdentityMatrix.

Main Method:

public static void main(String[] args) {
The main method, which is the entry point of the program.

Comment Block:

/*
 * We want to print shape
 *   1 2 3
 *   _____
 *1| 1 0 0   row = 1, column =1
 *2| 0 1 0   row = 2, column = 2
 *3| 0 0 1   row = 3, column = 3
 */
This comment block explains the desired output format of an identity matrix.

Random Object:

Random rnd = new Random();
Creates an instance of the Random class, named rnd, which will be used to generate random numbers.

Size of the Square Matrix:

int sqaureSize;
sqaureSize = rnd.nextInt(5) + 2;
Declares an integer variable sqaureSize and assigns it a random value between 2 and 6 (inclusive). rnd.nextInt(5) generates a random number between 0 and 4, and adding 2 ensures the minimum size is 2.

Outer Loop:


for(int i = 0; i < sqaureSize; i++) {
This loop iterates over each row of the matrix. i represents the current row index.

Inner Loop:


for(int j = 0; j < sqaureSize; j++) {
This nested loop iterates over each column of the matrix. j represents the current column index.

Condition to Print Elements:


if(i == j) {
    System.out.print("1");
} else {
    System.out.print("0");
}
This condition checks if the current row index i is equal to the current column index j. If true, it prints 1 (for the diagonal element), otherwise, it prints 0.

New Line After Each Row:


System.out.println();
After completing each row, this statement prints a newline character to move to the next line.

Example Output
If the random size generated is 4, the output might look like:

yaml
1000
0100
0010
0001
The output represents a 4x4 identity matrix. Each diagonal element (where row index equals column index) is 1, and all other elements are 0.
