# lab_05-task

## PROBLEM:01
*/
Write a program to check if a student has passed. If marks ≥ 50, check if marks ≥ 85,
then display “Passed with Distinction”. Otherwise, display “Just Passed”.
\*

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
