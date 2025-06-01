# EX-11-EMI-CALCULATOR
# NAME: VINOTHKUMAR R
# REG. NO: 212224040361
## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include<math.h>
int main()
{
    float f,p,r,n;
    scanf("%f %f %f ",&p,&r,&n);
    r=r/(12*100);
    n=n*12;
    f=(p*r*pow((1+r),n))/(pow((1+r),n)-1);
    printf("Monthly EMI is= %.3f",f);
}
```

## OUTPUT

![M3 1](https://github.com/user-attachments/assets/860fd476-72e8-4f54-8f9d-e1f32aa2e907)


## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM

```
#include<stdio.h>
int main()
{
    int n,a=0,b=1,next;
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    {
        next=a+b;
        printf("%d ",a);
        a=b;
        b=next;
    }
}
```

## OUTPUT

![M3 2](https://github.com/user-attachments/assets/e932099a-1058-47c2-bda8-76a13af06675)


## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n]; 
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n - 1]);

    return 0;
}
```
## OUTPUT

![M3 3](https://github.com/user-attachments/assets/ea25e4b6-f0b6-46a4-8e1e-ead897985f77)


## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, i, count = 0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements: %d\n", count);

    return 0;
}
```

## OUTPUT

![M3  4](https://github.com/user-attachments/assets/0a69bb76-ce1a-4ced-a008-8c4945f4ec85)

## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];        
    char output[n];   
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        if (arr[i] % 2 == 0) {
            output[i] = 'E';
        } else {
            output[i] = arr[i];
        }
    }
    printf("Modified array:\n");
    for (i = 0; i < n; i++) {
        if (output[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    printf("\n");
    return 0;
}
```
## Output:
 
![M3 5](https://github.com/user-attachments/assets/89e8e530-0fc3-4be6-aa5f-80271e631ad8)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



