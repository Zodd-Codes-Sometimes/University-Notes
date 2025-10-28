# Q1: How do you find a given number in an array (assuming the number is a user-input) 

```
#include <stdio.h> 

int main() {
    
    bool A;
    int b = 35;
    int arr1[] = {22, 33, 35, 48, 52, 65}; 
    
    int length = sizeof(arr1) / sizeof(arr1[0]);
    
    for (int i = 0; i < length; i++){
        if (arr1[i] == b){
            printf("Found at location: %d\n", i);
	         A = True;
        }
    }
if (A == False){
printf("Not found.)
}
    return 0;
}
```

# Misc. (Switch-case)

```
switch (a) {
    case 21:
    case 22:
    case 23:
    case 24:
    case 25:
    case 26:
    case 27:
    case 28:
    case 29:
        printf("good.");
        break;
    default:
        printf("bad.");
        break;
}
```

# Add all the values in the array

```
#include <stdio.h> 

int main() {
    
	int sum = 0;
    int arr1[] = {22, 33, 35, 48, 52, 65}; 
    
    int length = sizeof(arr1) / sizeof(arr1[0]);
    
    for (int i = 0; i < length; i++){
	    sum = sum + arr1[i];
    }
    printf("Value is %d", sum);
    return 0;
}
```

# Binary Search Code

```
#include <iostream>


```