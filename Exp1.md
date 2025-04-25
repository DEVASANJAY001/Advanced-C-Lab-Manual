EXP NO:1 C PROGRAM FOR ARRAY OF STRUCTURE TO CHECK ELIGIBILITY FOR THE VACCINE.

Aim:
To write a C program for array of structure to check eligibility for the vaccine person age above 6 years of age.

Algorithm:
1.	Declare structure eligible with age (integer) and n (character array)
2.	Declare variable e of type eligible
3.	Input age and name using scanf, store in e
4.	If e.age <= 6
-	Print "Vaccine Eligibility: No"
Else
-	Print "Vaccine Eligibility: Yes"
5.	Print details (e.age, e.n)
6.	Return 0
 
Program:
```
#include <stdio.h>

struct eligible {
    int age;
    char name[50];
};

int main() {
    struct eligible e;

    printf("Enter name: ");
    scanf("%49s", e.name);

    printf("Enter age: ");
    scanf("%d", &e.age);

    printf("\nName: %s\nAge: %d\n", e.name, e.age);
    if (e.age <= 6)
        printf("Vaccine Eligibility: No\n");
    else
        printf("Vaccine Eligibility: Yes\n");

    return 0;
}
```

Output:

![image](https://github.com/user-attachments/assets/8e1f7283-8c8b-4148-b973-b5af067f6867)

![image](https://github.com/user-attachments/assets/2a383e5d-cffe-48be-a79d-86367cd43dde)


Result:
Thus, the program is verified successfully.
