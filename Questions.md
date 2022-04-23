## CSA Questions DLC

There is a DLC :D
@author Dylan
-----
ABEDB DCDCC EDCCE DEDDD BAADC ECBAA

### MCQ 30 Questions:

### 1.

Consider the following code section:

```java
public class cls {
    public static void main(String[] args) {
        String s1 = new String("Hello, World!");
        String s2 = "Hello, World!";

        System.out.println(s1 == s2);
    }
}
```

What will be the result of executing this code segment?

```
A: true
B: false
C: nothing is printed
D: compilation error
E: runtime error
```

### 2.

In java, every class is inherited from which class?

```
A: Instance
B: Object
C: Interface
D: Class
E: Memstack
```

### 3.

Which of the following instance declaration is no accepted by the
java syntex?

```java
A.int a=(int)0.05;
B.boolean b=C>=D;
C.Object obj=new ClassA();
D.float array[]={0};
E.ArrayList<int>=new ArrayList<int>(20);
```

### 4.

Consider the following code:

```java
//Dog extends Animal, Cat extends Animal
Dog[]dogs=new Dog[10];
        Animal[]animals=dogs; //line 2
        animals[0]=new Cat();  //line 3
```

What will be the result of executing this?

```
A. Compile error at line 2
B. Compile error at line 3
C. Runtime exception at line 2
D. Runtime exception at line 3
E. The code will work fine
```

### 5.

Which of the following loop structure can not iterate the entire array?

```java
A.for(int i=0;i<array.length;i++)
B.i=0;do{i++;Object a=array[i];}while(i<array.length);
C.i=array.length;while(i>-1){i--;Object a=array[i];}
D.for(Object a:array)
E.Arrays.asList(array).forEach(o->{});
```

### 6.

which of the following is not a access control keyword in java?

```
A. public
B. private
C. protected
D. virtual
E. default
```

### 7.

Consider the following class definition:

```java
class C {
    public C() {
        System.out.print("C");
    }
}

class D extends C {
    public D() {
        System.out.print("D");
    }
}

class E extends D {
    public E() {
        super();
        System.out.print("E");
    }
}
```

what is the result of executing `new E();`?

```
A: E
B: DE
C: CDE
D: ED
E: the code encounters a compile error
```

### 8.

In many development projects, recursions are considered deprecated mainly because of
which of the following reason?

```
A. Recursion is hard to understand
B. Recursion causes waste of memory resources
C. Recursion is not supported by some java compilers
D. Infinite recursion will exceed the stack size limit of JVM
E. Using recursion as iteration would result in infinite loops
```

### 9.

Reinterpret cast is widely used in java. However, which of the following implementation
of this technique will result in a compile error?

```java
// D extends C
A.C obj=(C)new D();
B.D obj=(D)new D();
C.D obj=(D)new C();
D.C obj=new C();
  D obj2=(D)obj;
E.D obj=new D();
  C obj2=(C)obj;
```

### 10.

Consider the following code section:

```java
public class cls {
    public static void main(String[] args) {
        String s1 = new String("Hello, World!");
        String s2 = "Hello, World!";

        System.out.println("s1==s2:" + s1 == s2);
    }
}
```

What will be the result of executing this code segment?

```
A: s1==s2: true
B: s1==s2: false
C: false
D: true 
E: runtime error
```

### 11.

boolean expression `!(A || !(B && C))` is equivalent to which of the following?

```
A. A && !B || !C
B. !A && B || C
C. A && !B || C
D. A && B || !C
E. A && B && C
```

### 12.

consider the following code segment:

```java
if(A)
        if(B)System.out.println("1");
        System.out.println("2");
        else if(C)System.out.println("3");
```

For `3` to be printed, which of the following conditions must met?

```
A. A && B
B. A && !B && C
C. !A && C 
D. A && C
E. A && !B && !C
```

### 13.

Which kind of array initialization is not supported by Java?

```java
A.int[]a={1,2,3};
B.int[]a=new int[]{1,2,3};
C.int[]a=new int[];
D.int[]a=new int[3];
E.int[]a1=a; //assume a is an initialized array 
```

### 14.

Consider the following code segment:

```java
double a,b;
        a=0.0/0; //line 1
        b=3.0/0; //line 2
```

What are the result of executing this code segment?

```java
A.a=0.0,b=0.0
B.a=0.0,b=Infinity
C.a=Nan,b=Infinity
D.an exception will be thrown at line 1
E.an exception will be thrown at line 2
```

### 15.

Which of the following is not an OOP concept in Java?

```java
A.Encapsulation
B.Inheritance
C.Polymorphism
D.Abstraction
E.Compilation
```

### 16.

What will be the output of the following code segment?

```java
class Output {
    public static void main(String args[]) {
        int arr[] = {1, 2, 3, 4, 5};
        for (int i = arr.length; i < arr.length - 2; i--)
            System.out.print(arr[i] + " ");
    }
}
```

```java
A. 1 2
B. 4 5
C.ArrayIndexOutOfBoundsException
D.No observable output
E.Compilation error
```

### 17.

What is the result of executing the following code segment?

```java
public static String loops(String insert){
        String result=insert;
        result+=loops(insert.subString(1));
        return result;
        }

//call in main():
        System.out.println(loops("Howard"));
```

```java
A.Howardowardwardardrdd
B.HowardHowarHowaHowHoH
C.Howardwardrd
D.java.lang.StringIndexOutOfBoundsException
E.java.lang.StackOverflowException
```

### 18.

Multiple inheritance means:

```
A. A class can inherite from more than one class
B. a class extends more than one subclasses
C. a class can inherite a subclass
D. A and B
E. None of the above
```

### 19.

```java
class A {
    private void method1() {
        System.out.println("A.method1");
    }
}

class B extends A {
    @Override
    private void method1() {
        super.method1();
        System.out.println("B.method1");
    }
}

class C extends B {
    @Override
    private void method1() {
        super.method1();
        System.out.println("C.method1");
    }

    public void callMethod1() {
        method1();
    }
}
```

which of the following statements is true when `callMethod1()` is executed?

```
A. A.method1 will be called first
B. C.method1 will be called first
C. The code ends up in a infinite loop
D. The code does not compile
E. The code would encounter a runtime exception
```

### 20.

```java
//sort an array using insertion sort
public double[] insertionSort(double[] in){

for(int i=1;i<in.length;i++){
    double temp=in[i];  //l1
    int j=i-1;
    while(j>=0 && in[j]>temp){  //l2
        in[j+1]=in[j];          //l3
        j++;                    //l4
        in[j+1]=temp;          
    }
    return in;                  //l5
} 
```
The code is malfunctioning, what mighht be the possible cause?
```
A. l1 shoule be in[i-1];
B. l2 shoule be  while(j>0 && in[j]>temp);
C. l3 shoule be in[j+1] = temp;
D. l4 shoule be j--;
E. l5 shoule be return return new double[]{in}; 
```

### 21.

```java
//sourt a double array using merge sort
public double[] mergeSort(double[] in){
    if(in.length<2)
        return in;
    int mid = in.length/2;
    double[] left = new double[mid];
    double[] right = new double[in.length-mid];
    for(int i=0;i<mid;i++)
        left[i]=in[i];
    for(int i=mid;i<in.length;i++)
        right[i-mid]=in[i];
    left = mergeSort(left);
    right = mergeSort(right);
    return merge(left,right);
}
```
how many times is `merge()` called sorting an array of size 1000?

```
A. 31
B. 999
C. 208
D. 13
E. 55
```

### 22.

In java, an initialized variable is a:
```
A. Instance
B. Enumeration
C. Class
D. Pointer
E. Reference
```

### 23.

Consider the following code segment:

```java
class A{
    public int member;
}

//call in main():
A a = new A();
A a1 = a;
a1.member = 30;
System.out.println(a.member);
```
What is the output of executing this?
```
A. 30
B. 0
C. NullPointerException
D. Nan
E. Random number, as uninitialized variables will point to 
   a random address in memory and pick up what ever left there.
```

### 24. 

The boolean function `!((A && !B) || !C)` is equivalent to:

```
A. A && (B || !C)
B. A || (!B && C)
C. A && (!B || C)
D. !(A && C) || (B && C)
E. (A || B) && (B || !C)
```

### 25.

Which variable name is invalid in java syntax?
```java
A. int _a;
B. int 变量;
C. int for;
D. int x1;
E. int DATA;
```

### 26.

Consider the following code segment:

```java
//find the difference in the max and min element of an array:
public int findDifference(int[] in){
    int min = in[0];
    int max = in[0];
    for(int i=1;i<in.length;i++){
        if(in[i]<min){
            min=in[i];
            continue;
        }
        else if(in[i]>max)
            max = in[i];
    }
    return max-min;
}
```
Which of the array inputs will cause the code to malfunction?
```
A. {6,0,2,4,5}
B. {7,7,3,4,2}
C. {1,9,9,5,5}
D. {3,0,1,2,2}
E. The code works properly for any given input
```

### 27.

When an overridden method is called from within a subclass, it will always refer to the version of that method defined by the
```
A. superclass
B. subclass
C. D and E
D. Depends on the method definition
E. Depends on the method type
```

### 28.

The correct order of the hierarchy in a Java program is
```
A. public class, private class, variables, methods
B. package, class, methods and variables
C. class, package, methods, variables
D. public class, public variables, private class, private variables, methods
E. public class, private methods and variables, private class, methods
```

### 29. 

```java
class A{
    int a;
    public A(int a){
        this.a = a;
    }
}
```
Which code correctly instantialte an object of type A?
```
A. A a = new A(10);
B. A a = new A();
C. A a = new A;
D. A a = 10;
E. None of the above
```

### 30.

```java
double[][] mat = new double[3];
for(int i=0;i<3;i++)
    mat[i] = new double[i];
```
Which of the following codes can safely print all elements of the matrix?
```
A. for(int i=0;i<3;i++)
     for(int j=0;j<i;j++)
        System.out.println(mat[i][j]);
        
B. for(int i=0;i<3;i++)
     for(int j=0;j<3;j++)
        System.out.println(mat[i][j]);
        
C. for(double[] j : mat)
       for(double i : j)
           System.out.println(j[i]);
```

## FREE RESPONSE QUESTIONS:

### 1.

Conwey's game of life is a famous experiment in simulating the 
formation of complex systems. In a 2 dimensional grid containing 
live cells (value = 1) and dead cells (value = 0), the following 
rules applies every generation:
```
    1. Any live cell with fewer than two live neighbours dies, 
       as if caused by underpopulation.
    2. Any live cell with two or three live neighbours lives on 
       to the next generation.
    3. Any live cell with more than three live neighbours dies, 
       as if by overpopulation.
    4. Any dead cell with exactly three live neighbours becomes a 
       live cell, as if by reproduction.
```

Complete the code for running the game of life a round:

```java
/**
 * Precondition: The grid constains only 1s and 0s.
 * grid of int[m][n] : m > 3 and n > 3
 */
public static int[][] round(int[][] input);
```

### 2.

A binary tree is a tree in which each node has at most two children. This is
a data structure optimized for binary searches.

Each Node of the tree contains following information:

```
1. int data: the data stored in the node (int in this case)
2. Node left: the left child of the node (with value stored less than or equal this node)
3. Node right: the right child of the node (with value stored greater than this node)
4. method: public int getData(): returns the data stored in the node
5. method: public Node search(int x): returns itself with data equal to x,
                         or call the left child search() with data < c and 
                         right child search() with data > x
```
Construct the Node class:
    
### 3.

In the field of algorithmic neural networks, the softmax function is a useful activation
function that cast any input array into a probability density distribution.

The softmax function is defined as:
```
    softmax(arr[]) = (e^xi / (sum of e^x for x in arr[])) for xi in arr[]
```

complete the code for the softmax function:

```java
public static double[] softmax(double[] arr);
```
