# lab_05-task

## PROBLEM:01
/*
Write a program to check if a student has passed. If marks ≥ 50, check if marks ≥ 85,then display “Passed with Distinction”. Otherwise, display “Just Passed”.
*/

```c
#include <stdio.h>

int main(void){
    int marks;
    printf("Enter your marks: \n");
    scanf("%d", &marks);

    if(marks >= 50){
        if(marks>= 85){
            printf("Passed with distinction\n");
        }
        else {
            printf("Just Passed\n");
        }
    }
    return 0;
}
```

## PROBLEM: 02
/*
Write a program that takes age and gender. If age ≥ 18 and gender = male, print “Adult Male”, else if female, “Adult Female”, otherwise “Minor”.
*/

```c
#include <stdio.h>
#include <string.h>

int main(void){
    int age;
    char gender[1024];

    printf("Enter your age: ");
    scanf("%d", &age);
    printf("What is your gender?: ");
    scanf(" %c", &gender);

    if(age >= 18){
        if(strcmp(gender, "male")==0 || strcmp(gender, "Male")== 0){
            printf("Adult male\n");
        }
        else{
            printf("Adult female\n");
        }
    }
    else {
        printf("Minor\n");
    }
}
```
