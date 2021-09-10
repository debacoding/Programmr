[palindrome number](http://www.programmr.com/node/38435/begin)
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
