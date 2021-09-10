[add negative, even & odd numbers from a list: ]()
Complete the program to print the sum of negative numbers, positive even numbers, positive odd numbers from a list of numbers entered by the user. The list terminates when the number entered is zero.
```cpp
#include <iostream> 
using namespace std; 
 
int main() 
{ 
    int num,sumneg,sumeven,sumodd; 
    sumneg = sumeven = sumodd = 0;  
   
    do 
    {
      cout << "Enter a number (0 to terminate):" << endl;
      cin >> num;    
      if(num < 0) sumneg += num;
      else if(num % 2 == 0) sumeven += num;
      else sumodd += num;
    }   while (num != 0); 
 
    cout<<"\nSum of negative numbers = "<<sumneg; 
    cout<<"\nSum of positive even numbers = "<<sumeven; 
    cout<<"\nSum of positive odd numbers = "<<sumodd; 
    
    return 0; 
} 
```

Output
```
Enter a number (0 to terminate):
3
4
32
5
3
-3
-2
Sum of negative numbers = -5
Sum of positive even numbers = 36
Sum of positive odd numbers = 11
```

[palindrome number: ]()
Write a program which takes a number as input from the user and displays whether it's palindrome or not. A palindrome number is a number that remains the same when its digits are reversed.
```cpp
#include <bits/stdc++.h> 
using namespace std;

int isPalindrome (int n){
  //not checking for negative integers
  if (n < 0) return 1;
  
  //single digit numbers are always palindrome
  if (n >= 0 && n < 10) return 1;
  
  int temp = n,revN = 0;
  while (temp != 0){
    revN = revN * 10 + temp % 10;
    temp = temp / 10;
  }
 
  if (n == revN) return 1;
  else return 0;
  
}
 
int main(int argc, char* argv[]) 
{ 
     int  num;  
     cout << "Enter a number:";  
     cin >> num;  
      
     if (isPalindrome(num) == 1)  
       cout << "The number is a palindrome";  
     else  
       cout << "The number is not a palindrome";   
} 
```

Output
```
Enter a number: -121
The number is a palindrome
```

[sum of the digits of a number: ]()
Write a program to find sum of digits of a number using Do-While
```cpp
#include <iostream> 
using namespace std;  
int main() 
{ 
   int num; 
   cout<<"Enter the number: "; 
   cin>>num; 
      
   int sum = 0;
   
   while(num){
       sum += (num % 10);
       num /= 10;   
   }
   
    cout<<"\nSum of digits is: "<<sum;  
} 
```

Output
```
Enter the number: -23
Sum of digits is: -5
```

[sum of digits: ]()
Write a program which takes a number as input from the user and shows the sum of digits as output.
```cpp
#include <iostream> 
#include <string> 
using namespace std; 
int main(int argc, char* argv[]) 
{ 
   int num,sum=0; 
   cout<<"Enter a number:"; 
   cin>>num;
   
   while(num){
       sum += (num % 10);
       num /= 10;   
   }
   
  cout<<"Sum of digits:"<<sum;
     
}
```
Output
```
Enter a number:12345
Sum of digits: 15
```
[distance between 2 points: ]()
Find the distance between two points A (x1, y1) and B (x2, y2) using distance formula.
```cpp
#include <iostream>                
#include <string>                
#include <math.h>               
               
using namespace std;                
int main(int argc, char* argv[])                
{                
   	double x1,x2,y1,y2,distance;              
             
        cout <<"Enter x1:"<<endl;             
        cin>>x1;                     
        cout <<"Enter y1:"<<endl;             
        cin>>y1;             
        cout <<"Enter x2:"<<endl;             
        cin>>x2;             
        cout <<"Enter y2:"<<endl;             
        cin>>y2;                      
	
	distance = sqrt(pow((x2 - x1),2) + pow((y2 - y1),2));        
	cout<<"distance :"<<distance<<endl;                
}        
```

Output
```
Enter x1:-5
Enter x2:5
Enter y1:5
Enter y2:5
distance : 10
```
[area of triangle using Heron's formula: ]()
Calculate the area of a triangle using Heron's formula. Take the three sides of a triangle as inputs.

HERON'S FORMULA: Area= √s(s-a)(s-b)(s-c)
where s= semi-perimeter; a,b,c are sides of the triangle
```cpp
#include <iostream>   
#include<cmath>  
using namespace std;    
int main()   
{   
   int a,b,c;   
   float area;   
   cout<<"Enter the three sides :";   
   cin>>a>>b>>c;   
    
    int s = (a + b + c) / 2;
    area = sqrt(s * (s - a) * (s - b) * (s - c));
   
    cout<<"\nArea is : "<<area;  
    return 0; 
}   
```

Output
```
Enter the three sides :
4
5
6
Area is : 6.48074
```
[factorial evaluation: ]()
Find the factorial of a number n.
```cpp
#include <iostream>  
#include <string>  
using namespace std;  
int main()  
{   
    int n,fact=1; 
    cout<<"Enter the value of n: ";  
    cin>>n;
    
    if(n == 0 || n == 1) fact = 1;
    for(int i = 1; i <= n; i++) fact = fact * i;
  
    cout<<"Value of factorial is : "<<fact; 
    
    return 0;  
} 
```

Output
```
Enter the value of n: 5
Value of factorial is : 120
```
[BMI calculator: ]()
The body mass index (BMI) is commonly used by health and nutrition professionals to estimate human body fat in populations. It is computed by taking the individual's weight (mass) in kilograms and dividing it by the square of their height in meters.
```cpp
#include <bits/stdc++.h>
using namespace std;
int main()
{
   
    float height,weight,bmi;
   
	cout<<"Please Enter Your Height In Meters : ";
	cin>>height;
	cout<<"Please Enter Your Weight In Kg : ";
	cin>>weight;
	
	bmi = weight / pow(height,2);
	cout << "Your BMI is " << setprecision(1) << fixed << bmi << endl;
 
}
```

Output
```
Please Enter Your Height In Meters : 1.75
Please Enter Your Weight In Kg : 73
Your BMI is 23.8
```
[leap year finder: ]()
Complete the program to find out whether a year (entered in 4-digit integer representation) is a leap year.
```cpp
#include <iostream>   
using namespace std;  
   
int main()   
{   
   int year;   
   cout<<"\n Enter year (in 4-digits) : ";   
   cin>>year;   
   
    if((year % 4 == 0 && year % 100 != 0) || year % 400 == 0) cout << "Leap year" << endl;
    else cout << "Not a leap year" << endl;
   
    return 0;   
}   
```

Output
```
Enter year (in 4-digits) : 1932
Leap year
```
[is it a prime number?: ]()
Write a program to check whether a given number is prime or not?(n>=2)
If it is a prime number, print "Prime" else print "Not Prime" (do not print the quotes)
```cpp
#include <iostream> 
#include <string> 
using namespace std; 
int main() 
{ 
   int n; 
   cout<<"Enter the number: "; 
   cin>>n; 
   
   bool isPrime = true;
   
   // 0 and 1 are not prime numbers
    if (n == 0 || n == 1) {
        isPrime = false;
    }
    else {
        for (int i = 2; i <= n / 2; ++i) {
            if (n % i == 0) {
                isPrime = false;
                break;
            }
        }
    }
    
    if (isPrime)
        cout << "Prime" << endl;
    else
        cout << "Not Prime" << endl;
     
} 
```

Output
```
Enter the number: 5
Prime
```
[binary conversion: ]()

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
[]

```cpp

```

Output
```

```
