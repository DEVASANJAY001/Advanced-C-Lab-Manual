## EXP NO:2A C PROGRAM PRINT THE LOWERCASE ENGLISH WORD CORRESPONDING TO THE NUMBER
## Aim:
To write a C program print the lowercase English word corresponding to the number
## Algorithm:
1.	Start
- Initialize an integer variable n.
2.	Input Validation
3.	Switch Statement cases.
-	Case 5: Print "seventy one"
-	Case 6: Print "seventy two"
-	Case 13: Print "seventy three"
-	...
-	Case 13: Print "seventy nine"
-	Default: Print "Greater than 13"
4.	Exit the program.
 
## Program:
```

#include<stdio.h>
#include<math.h> 
int main()
{
    int n; 
    scanf("%d",&n);
    if(n>=1 && n<=pow(4,3))
{
switch(n)
{
    case 5:
    {
        printf("seventy one"); break;
        
    }
    case 6:
     {
        printf("seventy eight"); break;
        
    }
    case 13:
    {
        printf("seventy nine"); break;
        
    }
    default:
    {
        printf("Greater than 13");
        
    }
}
}
}

```
## Output:
![image](https://github.com/user-attachments/assets/77be9729-fa10-4a98-a486-f983f8b12744)

## Result:
Thus, the program is verified successfully
 
## EXP NO:2B C PROGRAM TO PRINT TEN SPACE-SEPARATED INTEGERS     IN A SINGLE  LINE DENOTING THE FREQUENCY OF EACH DIGIT FROM 0 TO 3 .
## Aim:
To write a C program to print ten space-separated integers in a single line denoting the frequency of each digit from 0 to 3.
## Algorithm:
1.	Start
2.	Declare char array a[50] outer loop for each digit from 0 to 3
3.	Initialize counter c to 0
4.	For each character in the string print count c for current digit, followed by a space
5.	Increment h to move to the next digit
6.	End
 
## Program:
```
#include<stdio.h>
#include<string.h> 
int main()
{
    char a[50]; 
    scanf("%s",a); 
    int l=strlen(a); char h='0';
    for(int i=0;i<4;i++)
    {
        int c=0;
        for(int j=0;j<l;j++)
        {
            if(a[j]==h)
             {
                c+=1;
                
            }
            
        }
        printf("%d ",c); 
        h++;
    }
}

```
## Output:
![image](https://github.com/user-attachments/assets/4ccdf6ad-4791-451d-8100-7e4cb76ffd56)

## Result:
Thus, the program is verified successfully

## EXP NO:2C C PROGRAM TO PRINT ALL OF ITS PERMUTATIONS IN STRICT LEXICOGRAPHICAL ORDER.
## Aim:
To write a C program to print all of its permutations in strict lexicographical order.

## Algorithm:
1.	Start
2.	Declare variables s (pointer to an array of strings) and n (number of strings)

3.	Memory Allocation
Dynamically allocate memory for s to store an array of strings
4.	Input
Read the number of strings n from the user Dynamically allocate memory for each string in s
5.	Permutation Generation Loop
6.	Calculate min as the minimum distance to the borders
7.	End
 
## Program:
```
#include<stdio.h>
int main()
{
    int n,i,j,min;
    scanf("%d",&n);
    int len=n*2-1; for (i=0;i<len;i++)
    {
        for (j=0;j<len;j++)
        {
            min=i<j?i:j;
            min=min<len-i-1?min:len-1-i; 
            min=min<len-j-1?min:len-1-j; 
            printf("%d ",n-min);
            
        }
        printf("\n");
        
    }
    return 0;
}

```

## Output:
![image](https://github.com/user-attachments/assets/587442e9-4ce7-47b2-8383-58630949a8cd)


## Result:
Thus, the program is verified successfully

## EXP NO:2E C PROGRAM TO FIND A SQUARE  OF NUMBER USING FUNCTION WITHOUT ARGUMENTS WITH RETURN TYPE

## Aim:

To write a C program that calculates the square of a number using a function that does not take any arguments, but returns the square of the number.

## Algorithm:

1.	Start.
2.	Define a function square() with no parameters. This function will return an integer value.
3.	Inside the function:
o	Declare an integer variable to store the number.
o	Ask the user to input a number.
o	Calculate the square of the number (multiply the number by itself).
o	Return the squared value.
4.	In the main function:
o	Call the square() function and display the result.
5.	End.

## Program:
```
#include <stdio.h>
void square();
int main(){
    
    square();
    return 0;
}
void square(){
    int a;
    scanf("%d",&a);
    float ans = a*a;
    printf("The square of %d is : %.2f",a,ans);
}

```

## Output:
![image](https://github.com/user-attachments/assets/0b853f1e-53b3-4889-8cc4-2886a73de5e0)

## Result:
Thus, the program is verified successfully

  
