[swapping two numbers: ]()
Complete the program to swap the values of two variables without using any other variable.
```cpp
#include <bits/stdc++.h>    
using namespace std;     
    
int main()    
{    
   int a,b;    
   cout<<"Enter 1st number:";    
   cin>>a;    
   cout<<"Enter 2nd number:";    
   cin>>b;    
    
    swap(a,b);
    
    cout<<a<<" "<<b;     
    return 0;    
}    
```

Output
```
Enter 1st number:6 
Enter 2nd number:5
5 6
```

[variable value: ]()
Output the ASCII code of the character?
```cpp
#include <iostream>   
#include <string>   
using namespace std;   
int main()  
 {  
     char ch;  
     int x;   
      cout<<"Enter the character:\n";  
       cin>>ch;  
      x = (int)ch;
      cout<<x<<"\n";  
   return 0;      
  }   
```

Output
```
Enter the character: A
65
```

[adding two numbers: ]()
Write a program to read two numbers and print their summation.
```cpp
#include <iostream>  
#include <string>  
using namespace std;  
int main(int argc, char* argv[])  
{ 
        int x,y;
        cin>>x;
        cin>>y;
        
        cout<<x+y;
}
```

Output
```
5
10
15
```

[initializing variables: ]()
Write a C++ program, such that whenever the program is executed, the string "Neel" and integer "18" is displayed with a space in between.
```cpp
#include <iostream> 
#include <string> 
using namespace std;
 
int main() 
{  
 string name = "Neel";
 int age = 18;
 cout<<name<<" "<<age;
 
     return 0; 
} 
```

Output
```
Neel 18
```

[greater between two variables: ]()
Print the greater between two variables
```cpp
#include <iostream>    
#include <string>    
using namespace std;    
int main(int argc, char* argv[])    
{    
   int a,b,c=0;    
   cout<<"Enter value of 1st variable: ";    
   cin>>a;    
   cout<<"Enter value of 2nd variable: ";    
   cin>>b;    
    
    if(a > b) cout << "Greater value is " << a << endl;
    else if(b > a) cout << "Greater value is " << b << endl;
    else cout << "Both are equal" << endl;
    
    return 0;
}    
```

Output
```
Enter value of 1st variable: 
Enter value of 2nd variable: 
```

[average calculation: ]()
Write a program that asks the user to enter 5 integers as input and then display their average as output. Try to write this program using only 2 variables(x,avg).
```cpp
#include <iostream>      
#include <string>      
using namespace std;      
int main(int argc, char* argv[])      
{       
        float avg=0;     
        int x;      
	for (int i = 0; i < 5; i++)      
	{    
                cout<<"Enter a number:"<<endl; 
                cin >>x;   
                
                avg += x;
	}      
	cout<<endl<<"avg= :"<< avg / 5.0 <<endl;     
        return 0;      
}     
```

Output
```
Enter a number:
5
Enter a number:
5
Enter a number:
5
Enter a number:
5
Enter a number:
5
avg= : 5
```

[a dumb calculator: ]()
Make a simple numeric calculator. It should prompt the user for three numbers. Then add the numbers together and divide by 2. Display the result. Your program must support numbers with decimals and not just integers.
```cpp
#include <iostream>
 
using namespace std;
int main()
{  
    double a,b,c;
    cin >> a >> b >> c;

    cout<<"("<<a<<" + "<<b<<" + "<<c<<")/2 is:"<<(a+b+c)/2;
}
```

Output
```
2.2
3.3
1.1
(2.2 + 3.3 + 1.1)/2 is: 3.3
```
