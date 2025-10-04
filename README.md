# lab_05-task

## PROBLEM:01

Write a program to check if a student has passed. If marks ≥ 50, check if marks ≥ 85,then display “Passed with Distinction”. Otherwise, display “Just Passed”.


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

Write a program that takes age and gender. If age ≥ 18 and gender = male, print “Adult Male”, else if female, “Adult Female”, otherwise “Minor”.


```c
#include <stdio.h>
#include <string.h>

int main(void){
    int age;
    char gender[10];

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

## PROBLEM:03

Write a program using nested switch to select a device: (1=Phone, 2=Laptop). Inside each, choose brand (Phone: 1=Samsung, 2=Apple; Laptop: 1=Dell, 2=HP).


```c
#include <stdio.h>

int main(void){
    int device, brand;

    printf("Enter device (1=Phone, 2=Laptop): \n");
    scanf("%d", &device);
    switch(device){
        case 1:
        printf("Choose brand for phone (1=Samsung, 2=Apple): \n");
        scanf("%d", &brand);
        switch(brand){
            case 1: 
            printf("You chose Samsung phone\n");
            break;
            case 2:
            printf("You chose Apple phone\n");
            break;
            default:
            printf("Invalid brand\n");
            break;
        }
        break;
        
        case 2:
        printf("Choose brand for laptop (1=HP, 2=DELL): \n");
        scanf("%d", &brand);
        switch(brand){
            case 1: 
            printf("You chose HP laptop\n");
            break;
            case 2:
            printf("You chose DELL laptop\n");
            break;
            default:
            printf("Invalid brand\n");
            break;    
        }
        break;

    }
}
```

## PROBLEM:04

A nested switch program where user enters continent (Asia, Europe) and then a country inside it (Asia → Pakistan, India; Europe → France, Germany).


```C
#include <stdio.h>


int main(void){
    int continent,country;

    printf("Enter your continent(1=Asia, 2=Europe):  \n");
    scanf("%d", &continent);
    switch(continent){
        case 1: //Asia
        printf("Enter your country(1=Pakistan, 2=India): \n");
        scanf("%d", &country);
        switch(country){
            case 1:
            printf("You entered Pakistan\n");
            break;
            case 2:
            printf("You entered India\n");
            break;
        }
        break;

        case 2: //Europe
        printf("Enter your country\n");
        scanf("%d", &country);
        switch(country){
            case 1:
            printf("You entered France\n");
            break;
            case 2:
            printf("You entered Geremany\n");
            break;
            deault:
            printf("Invalid country\n");
            break;
        }
        break;

    }
}
```

## PROBLEM:05

Write a program that checks whether a given number is divisible by both 2 and 3 using logical operators.


```c
#include <stdio.h>

int main(void){
    int num;

    printf("Enter the number: ");
    scanf("%d", &num);

    if(num % 2 == 0 && num % 3 == 0){
        printf("Number is divisible by 2 and 3\n");
    }
    else{
        printf("Number is not visible by 2 and 3\n");
    }
    return 0;
}
```

## PROBLEM:06

Demonstrate the effect of pre-increment and post-increment operators with an example.


```c
#include <stdio.h>

int main(void){
    int a,b;

    printf("Enter a: ");
    scanf("%d", &a);

    if(a>0){
        printf("Pre increment: a = %d and b = %d", a, b = ++a );
    }
    else{
        printf("Post increment: a = %d and b = %d", a,  b = a++);
    }
    return 0;
}
```

## PROBLEM:07

Use a nested ternary operator to find the smallest of three numbers.


```c
#include <stdio.h>

int main(void){
    int num1, num2, num3;

    printf("Enter number one: ");
    scanf("%d", &num1);
    printf("Enter number two: ");
    scanf("%d", &num2);
    printf("Enter number three: ");
    scanf("%d", &num3);
    
    printf("The Smallest number is: %d\n", (num1<num2)? ((num1<num3)? num1: num3): (num2<num3? num2: num3));

    return 0;
}
```

## PROBLEM:09

Write a program that checks if a number is odd or even using bitwise &.


```c
#include <stdio.h>
int main(void){
     int num;

     printf("Enter num: ");
     scanf("%d", &num);

     if(num & 1){
        printf("Number is odd\n");
     }
     else{
        printf("Number is even\n");
     }
     return 0;
}
```

## PROBLEM:10

Demonstrate bitwise left shift and right shift operators on an integer.


```c
#include <stdio.h>
int main(void){
    int a = 4;
    printf("After left shifting: a = %d\n", a<<1);
    printf("After right shifting: a = %d\n", a>>1);
    return 0;
}
```
 
