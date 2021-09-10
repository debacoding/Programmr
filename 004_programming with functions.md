[factorial function: ]()
Write a function to calculate the factorial for a number. This exercise calculates it for 3 numbers in a loop.
```cpp
#include <iostream> 
#include <string> 
using namespace std; 
 
//fact() Define a factorial function
// {{ write your code here
int fact(int num){
    if(num == 0 || num == 1) return 1;
    else return num * fact(num - 1);
}    
// }}
   
int main(int argc, char* argv[]) 
{ 
   int n; 
   long int ans;
   for(int i=0;i<3;i++)
   {
        cin>>n; 
        ans=fact(n);  
        cout<<ans<<endl;
   }  
} 
```

```
Input:
2
5
7
Output :
2
120
5040
```

[sum of n numbers: ]()
Write a program that asks the user for an integer number and find the sum of all natural numbers upto that number 
i.e. 1+2+3+...+n
```cpp
#include <bits/stdc++.h>  
using namespace std; 
int main(int argc, char* argv[]) 
{ 
   int a,sum=0; 
   cout<<"Enter a number:"; 
   cin>>a; 
  
 int func(int x);
 sum=func(a);
 
 cout<<"\n"<<sum;
 
 }
 
 int func(int x){
      ///{Write your code here 

    return (x * (x + 1)) / 2;

      ///} 
      
 }
```

```
Input:
Enter a number:3
Output:
6
```

[square: ]()
Write a C++ program to print the square of all integers upto a number entered by the user, using a function.
```cpp
#include <bits/stdc++.h>  
using namespace std;  
int main(int argc, char* argv[])  
{  
   int a;  
   cout<<"Enter a number:";  
   cin>>a;  
   
    
 void square(int x); 
  
 for(int i=0;i<=a;i++)   
    square(i); 
 } 
  
 ///{Write your code here   
 
 
 void square (int x){
     cout << pow(x,2) << endl;
 }

///} 
```

```
Input:
Enter a number:3
Output:
0
1
4
9
```

[max no: ]()
Write a c++ function to find the maximum of any three numbers using multiple return statements in a function definition.
```cpp
#include <bits/stdc++.h> 
using namespace std; 
int main(int argc, char* argv[]) 
{ 
   int a,b,max,c=0; 
   cout<<"Enter three numbers:"; 
   cin>>a>>b>>c; 
 
    
 
 int maximum(int a,int b,int c);
 max=maximum(a,b,c);
 cout<<"Max: "<<max; 
 }
     ///Write your code here 
 int maximum(int a,int b,int c){
    if(a > b && a > c) return a;
    else if(b > a && b > c) return b;
    else return c;
 }
```

```
Input:
Enter three numbers: 4
5
6
Output:
Max: 6
```

[sum and product functions: ]()
Define the functions sum() and product()  to print the sum and product of 2 numbers entered by the user.
```cpp
#include <iostream>     
#include <string>     
using namespace std;     
     
//sum() and product() // define these functions   
//{{ write your code here

int sum(int x,int y){ return x + y; }
int product(int x,int y){ return x * y; }

//}}
   
    
    
int main(int argc, char* argv[])     
{     
   int a,b,answer1,answer2;     
   cout<<"Enter 1st number:";     
   cin>>a;     
   cout<<"Enter 2nd number:";     
   cin>>b;     
     
    answer1 = sum(a,b);     
    answer2 = product(a,b);    
     
    
   
     
    cout<<answer1 <<endl;
    cout<<answer2;     
}     
```

```
INPUT:
23
45
OUTPUT:
68
1035
```

[factorial: ]()
Write a C++ program that finds the factorial of a given number using a function.
```cpp
#include <bits/stdc++.h> 
using namespace std; 
int main(int argc, char* argv[]) 
{ 
   int a,mul; 
   cout<<"Enter a number:"; 
   cin>>a; 
 
 
    
 int fact(int x);
 mul=fact(a);
 cout<<mul;
 }
///{Write your code here  

int fact(int x){
    return (x == 0 || x == 1) ? 1 : x * fact(x - 1);
}
```

```
Input:
Enter a number:4
Output:
24
```

[keychains for sale: ]()
Write a program that pulls up a menu with 4 options. It should look something like...

You will need to create functions for each of the 4 menu options. Entering the number will call the correct function.
This assignment does not require you to complete ANY of the functionality except for the working menu system. There is no need for you to program the ability to add keychains, remove keychains, view orders or checkout.
The functions should be named add_keychains(), rem_keychains(), view_order() and checkout().
Each function should print a message that it has been called.
The user should be able to keep putting in choices until the checkout() function is called. When checkout() is finished, the program should end.
```cpp
#include <iostream>
#include <string>
using namespace std;
//Write your code here

void add(){ cout << "ADD KEYCHAINS" << endl; }
void rem(){ cout << "REMOVE KEYCHAINS" << endl; }
void view(){ cout << "VIEW ORDER" << endl; }
void checkout(){ cout << "CHECKOUT" << endl; }

 //
int main(int argc, char* argv[])
{
int choice=1;
cout<<"Welcome to keychain shop:\n";
    
    while(choice!=4)
    {
cout<<"1. Add Keychains to Order:\n2. Remove Keychains from Order:\n3. View Current Order:\n4. Checkout:\n";
cout<<"Please enter your choice:";
cin>>choice;
switch(choice)
{
    case 1:
    add();
    break;
    case 2:
    rem();
    break;
    case 3:
    view();
    break;
    case 4:
    checkout();
    break;
    default:
    cout<<"Wrong choice\n";
}
}
   
}

```

```
1. Add Keychains to Order
2. Remove Keychains from Order
3. View Current Order
4. Checkout
Please enter your choice:1
ADD KEYCHAINS
1. Add Keychains to Order
2. Remove Keychains from Order
3. View Current Order
4. Checkout
Please enter your choice:3
VIEW ORDER
1. Add Keychains to Order
2. Remove Keychains from Order
3. View Current Order
4. Checkout
Please enter your choice:4
CHECKOUT
```

[area calculator: ]()
Write a program to calculate the area of four different geometric shapes: triangles, squares, rectangles, and circles. You must use functions. Your program should present a menu for the user to choose which shape to calculate, then ask them for the appropriate values (length, width, radius, etc.). Then it should pass those values to the appropriate function and display the resulting area.

Notice that you must not input the values inside the functions, and you must not display the values inside the functions. All input and output must be in the main(), and values must be passed to the functions and returned from them.
```cpp
#include <iostream>
#include <string>
using namespace std;
///Write your code here
double area_triangle(double base,double height){
    return (base * height) / 2;
}

double area_rectangle(double length,double width){
    return length * width;
}

double area_square(double side){
    return side * side;
}

double area_circle(double radius){
    return 3.14 * radius * radius;
}

///}
int main(int argc, char* argv[])
{
	int x;
    cout<<"Shape Area Calculator:\n";
	cout<<"1) Triangle 2) Rectangle 3) Square 4) Circle:\n";
    cout<<"Which shape:";
	cin>>x;
		switch(x){
		case 1:
			double b,h;
			cout<<"Height:";cin>>h;cout<<"Base:";cin>>b;
			cout<<"The area is "<<area_triangle(b,h);
			break;
		case 2:
			double l,w;
			cout<<"Length:";cin>>l;cout<<"Width:";cin>>w;
			cout<<"The area is "<<area_rectangle(l,w);
			break;
		case 3:
			double s;
			cout<<"Side:";cin>>s;
			cout<<"The area is "<<area_square(s);
			break;
		case 4:
			double r;
			cout<<"Radius:";cin>>r;
			cout<<"The area is "<<area_circle(r);
			break;
        default:
            cout<<"Invalid Option";
		}
        
		
}
```

```
Shape Area Calculator:
 
1) Triangle 2) Rectangle 3) Square 4) Circle:

Which shape:1

Base:5

Height:6

The area is 15
```

[greatest common divisor: ]()
Take two numbers from user and pass them to function which will return their GCD.
```cpp
#include <bits/stdc++.h>
using namespace std;
 //Write code{

int GCD(int a,int b){
    if(a == 0) return b;
    else return GCD(b % a,a);
}    

 //}


int main()
{
    int x, y;
    cout<<"Enter value of x:";
	cin >> x;
    cout<<"Enter value of y:";    
	cin >> y;

	cout <<"The GCD of "<<x<<" and "<<y<<" is "<<GCD(x, y);  

	return 0;
}
```

```
Enter value of x:2
Enter value of y:3
The GCD of 2 and 3 is 1
```

[keychains for sale, for real this time: ]()
Create a menu driven program having menu like this

1. Add Keychains to Order
2. Remove Keychains from Order
3. View Current Order
4. Checkout
You will need 2 new variables in main, one to store the current number of keychains, and one to store the price per keychain.
The price should be $10 per keychain.
add_keychains() will need to be passed one int, and have a return type of int. It will ask the user for the number of keychains to add to the order, and then return the new number of keychains.
remove_keychains() will need to be passed one int, and have a return type of int. It will ask the user for the number of keychains to remove from the order, and then return the new number of keychains.
view_order() will need to be passed two ints, and have a return type of void. It will display, on three different lines, the number of keychains in the order, the price per keychain, and the total cost of the order.
checkout() will need to be passed two ints, and have a return type of void. It will ask the user for his/her name in order to deliver them correctly, display the order information, and then thank the user, by name, for ordering.
```cpp

```

```
Ye Olde Keychain Shoppe

1. Add Keychains to Order
2. Remove Keychains from Order
3. View Current Order
4. Checkout
Please enter your choice:1
You have 0 keychains. How many to add?:3
You now have 3 keychains.
1. Add Keychains to Order
2. Remove Keychains from Order
3. View Current Order
4. Checkout
Please enter your choice:2
You have 3 keychains. How many to remove?:1
You now have 2 keychains.
1. Add Keychains to Order
2. Remove Keychains from Order
3. View Current Order
4. Checkout
Please enter your choice:3
You have 2 keychains.
Keychains cost $10 each.
Total cost is $20.
1. Add Keychains to Order
2. Remove Keychains from Order
3. View Current Order
4. Checkout
Please enter your choice:4
What is your name?:Biff
Each keychain costs 10$ so total is 20$
Thank you for your order Biff!
```
