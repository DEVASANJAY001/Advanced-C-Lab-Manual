EXP NO:2 C PROGRAM FOR PASSING STRUCTURES AS FUNCTION ARGUMENTS AND RETURNING A STRUCTURE FROM A FUNCTION
Aim:
To write a C program for passing structure as function and returning a structure from a function

Algorithm:
1.	Define structure numbers with members a and b.
2.	Declare variable n of type numbers.
3.	Prompt the user to enter values for a and b.
4.	Input values for a and b into n using scanf.
5.	Call the add function with n as an argument.
6.	Print the result returned by the add function.
7.	Return 0
 
Program:
```
#include <stdio.h>
struct Student {
    int id;
    char name[50];
    float marks;
};
void displayStudent(struct Student s) {
    printf("Student Details:\n");
    printf("ID: %d\n", s.id);
    printf("Name: %s\n", s.name);
    printf("Marks: %.2f\n", s.marks);
}
struct Student inputStudent() {
    struct Student s;
    printf("Enter student ID: ");
    scanf("%d", &s.id);
    printf("Enter student name: ");
    scanf(" %[^\n]", s.name);
    printf("Enter student marks: ");
    scanf("%f", &s.marks);
    return s;
}

int main() {
    struct Student s1;
    s1 = inputStudent();
    displayStudent(s1);

    return 0;
}
```
Output:

![image](https://github.com/user-attachments/assets/8de71488-7919-45fa-abf8-8c4c8118d4c0)

Result:
Thus, the program is verified successfully
