[operator(+): ]()
Your Task is to read the three values of the sides of a triangle and print the result of their summations.
```cpp
#include <iostream>  
#include <string>  
using namespace std;  
int main(int argc, char* argv[])  
{  
   float a,x,b,c=0;  
   cout<<"Enter 1st number:";  
   cin>>a;  
   cout<<"Enter 2nd number:";  
   cin>>b;  
   cout<<"Enter 3rd number:"; 
   cin>>x; 
    
   c = a + b + x;

   cout<<c;  
}  
```

Output
```
Enter 1st number:
3.2
Enter 2nd number:
5.3
Enter 3rd number:
10.9
19.4  
```

[area & perimeter of circle: ]()
Complete the program taking input choice (1 or 2).

If choice is 1, print the are of a circle otherwise print the perimeter of circle.
```cpp
#include <iostream> 
using namespace std;
 
int main() 
{ 
   int choice;
   float radius; 
    
   cout<<"\n Enter choice :"; 
   cin>>choice; 
   cout<<"\n Enter radius of cirle :";
   cin>>radius; 
   
   switch(choice){
       case 1:{
           cout << "Area = " << 3.14 * radius * radius << endl;
           break;
       }
       case 2:{
           cout << "Perimeter = " << 2 * 3.14 * radius << endl;
           break;
       }
   }
 
   return 0; 
} 
```

Output
```
 1. Area of circle
 2. Perimeter of circle
 Enter choice : 1
 Enter radius of cirle : 10
 Area = 314
```

[even 3 multiples: ]()
Write a program to see whether a number is an even multiple of 3
```cpp
#include<iostream>

using namespace std;

int main()
{
    int a;
    cin>>a;
    
    
    if(a % 3 == 0 && a % 2 == 0) cout << "yes"<< endl; 
    else cout << "no" << endl;

    return 0;
}
```

Output
```
9
no
```

[salary estimation based on experience: ]()
Take input of experience and age of a person.

If the person is experienced and his age is equal to or more than 35 the slary of the person is 6000. Otherwise, if the person is experienced and his age is equal to or more than 28 but less than 35, then the salary should be 4800.For experienced person below 28 yr of age the salary should be 3000 and for inexperienced person the salary should be 2000.
```cpp
#include <iostream>      
using namespace std;     
int main()     
{     
   int salary, exp, age;     
   cout<<"\n Is the person experienced ? Enter 1 for yes, 0 for no : ";     
   cin>>exp;     
   cout<<"\n Enter age of the person : ";   
   cin>>age;   
      
    if(exp == 1 && age >= 35) salary = 6000;
    else if(exp == 1 && age >= 28 && age < 35) salary = 4800;
    else if(exp == 1 && age < 28) salary = 3000;
    else if(exp == 0) salary = 2000;
   
    
   cout<<"\n The salary of the person is "<<salary; 
       
   return 0;     
}     
```

Output
```
Is the person experienced ? Enter 1 for yes, 0 for no : 1
Enter age of the person : 26
The salary of the person is 3000
```

[modulus of variables: ]()
Print the remainder of a/b (first number/second number).
```cpp
#include <iostream>  
#include <string>  
using namespace std;  
int main(int argc, char* argv[])  
{  
   int a,b,c=0;  
   cout<<"Enter 1st number:\n";  
   cin>>a;  
   cout<<"Enter 2nd number:\n";  
   cin>>b;  
   c = a % b;
    cout<<"Remainder is:"<<c;  
    return 0;  
}  
```

Output
```
Enter 1st number:
10
Enter 2nd number:
5
Remainder is:0
```

[pre ans post increment operator: ]()
Write a program to print the resultant value after adding a++(post-increment) and ++a(pre-increment).
```cpp
#include <iostream>          
#include <string>          
using namespace std;          
int main(int argc, char* argv[])          
{          
   int a,b=0;          
   cout<<"Enter value of a: ";          
   cin>>a;          
            
    b = a++;
    b += a;
    
       cout<<"Addition is: "<<b;   
            
}    
```

Output
```
Enter value of a: 12
Addition is: 25
```

[ternary operator: ]()
Print the greater value between two variables by only using ternary operators(?:). If equal is just prints that value.
```cpp
#include <iostream>  
#include <string>  
using namespace std;  
int main(int argc, char* argv[])  
{  
   int a,b,c=0;  
   cout<<"Enter 1st number:";  
   cin>>a;  
   cout<<"Enter 2nd number:";  
   cin>>b;  
  
  c = (a > b) ? a : b;
  
    cout<<"Greater value is:"<<c;  
}  
```

Output
```
Enter 1st number:5
Enter 2nd number:1
Greater value is:5
```

[basic operators: ]()
Write a program that evaluates the following things for two int numbers:

Sum,Diff,Product,Quotient,Remainder,Increment first no, Decrement Second no.,takes a third num- Checks if first no is greater than second then assign third no 1. If not, assign third no 0 (use conditional operator for last task)
```cpp
#include <iostream>  
#include <string>  
using namespace std;  
int main(int argc, char* argv[])  
{  
   int num1,num2,sum,diff,product,quotient,remainder,num3=0; 
   cout<<"Enter 1st number: ";  
   cin>>num1;  
   cout<<"Enter 2nd number: ";  
   cin>>num2;  
  
  sum = num1 + num2;
  diff = num1 - num2;
  product = num1 * num2;
  quotient = num1 / num2;
  remainder = num1 % num2;
  num1 += 1;
  num2 -= 1;
  if(num1 > num2) num3 = 1;
  else num3 = 0;
    
  cout<<"" << sum; 
  cout<<"\n" << diff; 
  cout<<"\n" << product;  
  cout<<"\n" << quotient; 
  cout<<"\n" << remainder; 
   cout<<"\n" << num1; 
   cout<<"\n" << num2; 
   cout<<"\n" << num3; 
   
 return 0; 
  
}  
```

Output
```
Enter 1st number:
20
Enter 2nd number:
10

30
10
200
2
0
21
9
1
```

[size of integer value: ]()
Find the size in bytes of the type used to store the value input by the user?
```cpp
#include<iostream>  
  
using namespace std;  
  
int main()  
 {       
    int a,b;            
    cout<<"Enter the element:\n";  
    cin>>a;  
      
    b = sizeof(a);
    cout<<"The value is:"<<b<<"\n";  
       
 } 
```

Output
```
Enter the element:3
The value is:4
```
