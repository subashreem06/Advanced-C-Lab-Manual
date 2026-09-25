## EXP NO:1 C PROGRAM FOR ARRAY OF STRUCTURE TO CHECK ELIGIBILITY FOR THE VACCINE.
2.	Declare variable e of type eligible
3.	Input age and name using scanf, store in e
4.	If e.age <= 6
-	Print "Vaccine Eligibility: No"
Else
-	Print "Vaccine Eligibility: Yes"
5.	Print details (e.age, e.n)
6.	Return 0
 
### Program:

```c
#include <stdio.h>

struct eligible {
    int age;
    char n[50];
};

int main() {
    struct eligible e;

    scanf("%d", &e.age);
    scanf("%s", e.n);
    printf("Age:%d\n", e.age);
    printf("Name:%s", e.n);
    printf("vaccine:%d\n", e.age);
    if (e.age <= 6) {
        printf("eligibility:no\n");
    } else {
        printf("eligibility:yes\n");
    }
    return 0;
}
```


### Output:

<img width="568" height="134" alt="image" src="https://github.com/user-attachments/assets/ee5bb1f8-2ef9-4a69-bd1d-8ff37e1406f7" />



### Result:
Thus, the program is verified successfully. 

---

## EXP NO:2 C PROGRAM FOR PASSING STRUCTURES AS FUNCTION ARGUMENTS AND RETURNING A STRUCTURE FROM A FUNCTION

### Aim:
To write a C program for passing structure as function and returning a structure from a function

### Algorithm:
1.	Define structure numbers with members a and b.
2.	Declare variable n of type numbers.
3.	Prompt the user to enter values for a and b.
4.	Input values for a and b into n using scanf.
5.	Call the add function with n as an argument.
6.	Print the result returned by the add function.
7.	Return 0
 
### Program:
```c
#include<stdio.h>

struct numbers{
    int a;
    int b;
}n;

int add(struct numbers n);

int main(){
    scanf("%d %d ",&n.a,&n.b);
    printf("%d",add(n));
}

int add(struct numbers n){
    return n.a+n.b;
}
```




### Output:

<img width="259" height="298" alt="image" src="https://github.com/user-attachments/assets/4272eafa-89bb-4429-bcb7-e5bbc37f25ed" />
