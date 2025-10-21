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


#### [[#Pointer Concept]] - Diagram

The Diagram shows a memory stack where data is stored on basis of byte-space required.* 

![[Stack Memory _ Lec1.jpg]]
# Q1: Write code to copy Arr1 into Arr2

```
// In C

void main (void){
int arr1[] = {90, 60, 65, 85, 72, 52};
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
}

```

# Q3: Write code to find the Biggest Number in Arr1

```
#include <stdio.h>

int main(void) {
    int arr1[] = {90, 60, 65, 85, 72, 92};
    int big = arr1[0];
    for (int i= 0; i < 6; i++)
    {
	    if (big < arr1[i])
	    {
		    big = arr1[i];
		}
    }  
    printf("big = %d\n", big);
}
```

# Q4: Swap every single pair of values

```
#include <stdio.h>

int main() {
    int arr[] = { 12, 10, 78, 89, 99, 15};
    int temp;
    for (int i = 0; i < 6; i +=2)
    {
        temp = arr[i];
        arr [i] = arr[i+1];
        arr[i+1] = temp;
    }
    for(int i = 0; i < 6; i++)
        printf("arr[i] = %d\n", arr[i]);
    return 0;
}
```

# Stack pointer 

```
// Java code

Class Box {
String Arr[5];
int SP = 0; 
}

Public void push (String Name)
{
Arr[SP] = Name;
SP++;
}

public void pop()
{
SP--;
System.out.println(Arr[SP]);
}

Box b = new Box();
b.push("English");
b.push("Math");
b.push("Physics");
b.push("Chemistry");
// All of the code above will add string "Name" values to stack memory

b.pop();
b.pop();
b.pop();
b.pop();
// All lines above will 'pop out' or remove the string values from stack memory
```

## Assignment before Mids (Due in next class):

 What are the sorting techniques used in data structures? Explain briefly. 
a) Learn about and implement bubble sort on a problem (One problem with ascending order and one to make into descending order)