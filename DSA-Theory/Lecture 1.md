# Forms of Data:

- Numbers (Complete *(int)*, Incomplete *(float)* )
- Text (String, Character)
- Boolean (True/False, Yes/No, On/Off)
- Pointers (They store addresses to a location in memory)
- Images (Binary colour info *(RGB)* )
- Video (Number of images / Frames per second)
- Geometry (2D, 3D) 

```
// How data structures are shown (Basic Example)

Struc Employee
{
int Eid,
Str Name,
Str PhoneNo
}
```

# Pointer Concept:

```
void main(void)
{
int a = 10, b = 20, c = 30;
char d = '*', e = '$';

int *A, *B, *C;
A = &a;
B = &b;
C = &c;

*A = 90;

# Alternatively (Pointer pointing to a pointer)

int **Z;
Z = &A;

**Z = 60;

}
```


# Q1: Write code to copy Arr1 into Arr2

```
// In C

void main (void){
int arr1[] = {90, 60, 65, 85, 72, 52}
int arr2[];
	for (int i = 0; i <=5; i++){
	arr2[i]=arr1[i];
	}
}
```

# Q2: Write code to copy Arr1 into Arr2 in reverse order

```
#include <stdio.h>

int main(void) {
    int arr1[] = {90, 60, 65, 85, 72, 52};
    int arr2[6];  

    for (int i = 0; i < 6; i++) {
        arr2[i] = arr1[5 - i];  
    }
    return 0;
}

```

# Q3: Write code to find the Biggest Number in Arr1

```
#include <stdio.h>

int main(void) {
    int arr1[] = {90, 60, 65, 85, 72, 52};
    
}

```