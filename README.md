EX-21-POINTERS
# AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:
     #include<stdio.h>
     int main() {
         float num = 23.65;
         int *ptr = (int*)&num;
         *ptr = 25;
         printf("%d", *ptr);
         return 0;
     }
## OUTPUT:
 	
![image](https://github.com/user-attachments/assets/1267acea-d38f-4e83-a387-3db420cd3c37)











## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.
 
 


# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:
    #include<stdio.h>
       int product(int n) {
           if(n == 1) return 1;
           return n * product(n-1);
       }
       int main() {
           printf("%d", product(12));
           return 0;
       }
## OUTPUT:
![image](https://github.com/user-attachments/assets/731daee9-023d-40b3-9aed-bd62677a1fb6)

## RESULT:

Thus the program has been executed successfully.
 
 


# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each row of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each row of the matrix.
3.	Inside the loop, calculate the sum of the elements in each row.
4.	Print the sum for each row.

## PROGRAM:
    
    #include<stdio.h>
    int main() {
        int mat[3][3] = {{1,2,3},{4,5,6},{7,8,9}};
        for(int i=0; i<3; i++) {
            int sum = 0;
            for(int j=0; j<3; j++)
                sum += mat[i][j];
            printf("%d\n", sum);
        }
        return 0;
    }

## OUTPUT


 ![image](https://github.com/user-attachments/assets/058ef231-bba8-4c34-bd0d-432d60a63c6f)

 

 ## RESULT
 


# EX-24-STRINGS

## AIM:

Write C program for the below pyramid string pattern. Enter a string: PROGRAM Enter number of rows: 5 P R O G R A M P R O G R A M P R O G R A M

## ALGORITHM:

1.	Input the number of rows for the pyramid (e.g., num_rows).
2.	Initialize variables:i for the row count (starting from 1),j for the character count (starting from 1)
3.	Start a loop for i from 1 to num_rows (for each row of the pyramid).
4.	Calculate the midpoint position as midpoint = (2 * num_rows - 1) / 2.
5.	End the program.

## PROGRAM:

    #include<stdio.h>
    #include<string.h>
    int main() {
        char str[100] = "PROGRAM";
        int rows = 5, len = strlen(str), k=0;
        for(int i=1; i<=rows; i++) {
            for(int j=1; j<=i; j++) {
                printf("%c ", str[k++]);
                if(k == len) k = 0;
            }
            printf("\n");
        }
        return 0;
    }
 ## OUTPUT

 ![image](https://github.com/user-attachments/assets/f9af04d5-fd2a-4584-8762-4b13467104b9)


## RESULT

Thus the C program to String process executed successfully
 

 
.



# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM
    #include<stdio.h>
    int main() {
        int arr[6], *ptr = arr;
        for(int i=0; i<6; i++)
            scanf("%d", ptr+i);
        for(int i=0; i<6; i++)
            printf("%d ", *(ptr+i));
        return 0;
    }
## OUTPUT
![image](https://github.com/user-attachments/assets/4ea084ba-b2cc-48f3-8536-f308491d68c0)

 

## RESULT

Thus the C program to read and display an array of any 6 integer elements using pointer has been executed


