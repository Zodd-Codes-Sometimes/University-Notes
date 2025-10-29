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
// Code in Cpp

#include <iostream>

int binarySearch(int arr[], int n, int target) {
    int left = 0;
    int right = n - 1;

    while (left <= right) 
    {
        int mid = left + (right - left) / 2;
        if (arr[mid] == target) { return mid;  }
        if (arr[mid] < target) { left = mid + 1; }
        else { right = mid - 1; }
    }
    return -1;
}

int main() {
    int sortedArr[] = {2, 5, 8, 12, 16, 23, 38, 56, 72, 91};
    int targetValue = 23;
    
    int arrSize = sizeof(sortedArr) / sizeof(sortedArr[0]);

    int result = binarySearch(sortedArr, arrSize, targetValue);

    std::cout << "Result: " << result << std::endl;
    
    return 0;
}
```