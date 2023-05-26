# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
 ## Algorithm:

 ## Step 1:
 Create a class operator
 ## Step 2:
 Pass values through the constructor
 ## Step 3:
 Return the bool operator, (==) and (!=)
 ## Step 4:
 Create a object to store the return object
 ## Step 5:
 Print the program.
 
 
 
 ## Program:
 ```
 NAME : POOJITHASETTY
 REG_NO : 212221240050

using System;
namespace overload
{
   class example
   {
       int n;
       public example(int a)
       {
           this.n = a;
           Console.Write("This is a parameterized Constructor");
           Console.WriteLine(" value is = " + this.n);
       }
       public example()
       {
           this.n = 10;
           Console.WriteLine("Default Constructor value is = " + this.n);
       }
       public static bool operator ==(example e1, example e2)
       {
           return e1.Equals(e2);
       }
       public static bool operator !=(example e1, example e2)
       {
           return !e1.Equals(e2);
       }
       static void Main(string[] args)
       {
           example e1 = new example(10);
           example e4 = new example();
           example e2 = e4;
           if (e2 == e4)
           {
               Console.WriteLine("Both are equal");
           }
           else
           {
               Console.WriteLine("Both are not equal");
           }
       }
   }
}
```

 
 
 ## Output:
 ![output](out.png)
 
 ## Result:
 Thus the C# program to find the volume of a box using operator overloading is implemented successfully.
