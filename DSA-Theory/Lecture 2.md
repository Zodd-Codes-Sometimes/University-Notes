# Q1: Make it so the first value is deleted

```
=== Algorithm ===

arr [0] = Arr [1];
arr [1] = Arr [2];
arr [2] = Arr [3];
arr [3] = Arr [4];
arr [4] = Arr [5];
arr [5] = Arr [6];
arr [6] = Arr [7];
arr [7] = 0;
```

```
void main(void) {
    int ar[] = {12, 17, 15, 18, 21, 20, 35};
    for (int i = 0; i < arr.length; i++) {
        if (i == arr.length) {
            arr[i] = 0;
            break;
        }
        arr[i] = arr[i + 1];
    }
}

```
# Q2: Write the same array in a reverse order

```
=== Algorithm ===

arr [0] = Arr [7];
arr [1] = Arr [6];
arr [2] = Arr [5];
arr [3]= Arr [3];
arr [5] = Arr [2];
arr [6] = Arr [1];
arr [7] = Arr [0];

```

```
void main(void) {
    int ar[] = {12, 17, 15, 18, 21, 20, 35};

    for (int i = 0; i < arr.length; i++) {
        arr1[i] = arr1[7 - i];
    }
}
```

# Q3: Find the biggest number in the array

```
void main(void) {
    int arr[] = {12, 17, 15, 18, 21, 20, 35};
    int n = sizeof(arr) / sizeof(arr[0]);
    int max = arr[0];  // assume first element is the largest

    for (int i = 1; i < n; i++) {
        if (arr[i] > max) {
            max = arr[i];
        }
    }

    printf("The largest number in the array is: %d\n", max);
}
```
