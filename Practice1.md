## Data type & variable practice 

```c++ 
  #include <iostream>
  using namespace std;
  
  int main() {
      
      int mynumber;
      double myfloatnumber;
      
      mynumber = 2001;
      
      myfloatnumber = 999;
      
      bool flag = false;
      
      cout<<sizeof(myfloatnumber)<<endl;
      cout<<sizeof(mynumber)<<endl;
      
      cout<<"The value of flag : " << flag <<"and the size occupied : " << sizeof(flag) << endl;;
      
      // the value of flag: 0 and the size occupied : 1  
      
      cout<<"My integer number is : "<<mynumber <<endl <<"My floating number is : "<< myfloatnumber;
      return 0;
  }
```

## Operators: 

- **Arithmatic**
  ```c++
  #include <iostream>
  using namespace std;
  
  int main() {
      
      // Arithmatic operator
      
      int num1 = 10;
      int num2 = 20;
      int num3 = 14;
      
      // int ans = ((((num1 + num2) - num3) * 4 ) / 2) % 5;
      
      int ans = num1 + num2;
      ans = ans - num3;
      ans = ans * 4;
      ans = ans / 2;
      ans = ans % 5;
      cout<<"Ans is : "<< ans << endl;
      return 0;
  }
  ```

- **Relational**: 

```c++
  #include <iostream>
  using namespace std;
  
  int main() {
      
      // Realtional operator
      
      int num1 = 10;
      int num2 = 20;
      
      if(num1 > num2){
          cout<<"num1 is grater!!"<<endl;
      }
      
      if(num1 != num2 ){
          cout<<"number 1 is equal to number 2"<<endl;
      }

      if(num1 <= num2 ) {
          cout<<"num2 is grater"<<endl;
          int a = 10;
          int b = 20;
          cout<<"The sum of two number is : " << a+b <<endl;
      }
      return 0;
  }

```

## Global & local variable with scope

```c++
#include <iostream>
using namespace std;

int Global_Value = 9999999999; // global variable 

int main() {
	{
	    int a = 10; // global variable for its chield;
	    cout<<a<<endl;
	    {
	       cout<<a<<endl; 
	       {
	           {
	               {
	                   int b = 20;
	                   cout<<a<<endl;
	               }
	               
	           }
	       }
	    }
	}
	
	return 0;
}
```
## largest of 2 number 

```c++
#include <iostream>
using namespace std;

// logical operators (and = && , or = ||, not = !)

int main()
{
    int a = 10;
    int b = 20;

    int ans = (a > b) ? a : b;

    if (a > b)
    {
        ans = a;
    }
    else
    {
        ans = b;
    }

    cout << "the larest number : " << ans << endl;

    return 0;
}
```
## largest of three number

```c++
#include <iostream>
using namespace std;

// logical operators (and = && , or = ||, not = !)

int main()
{

    int num1;
    int num2;
    int num3;

    cout << "Enter num1 num2 num3: " << endl;
    cin >> num1 >> num2 >> num3;

    if ((num1 > num2) && (num1 > num3))
    {
        cout << "num1 is grater: " << num1 << endl;
    }
    else if ((num2 > num1) && (num2 > num3))
    {
        cout << "num2 is gater: " << num2 << endl;
    }
    else if ((num3 > num1) && (num3 > num2))
    {
        cout << "num3 is grater: " << num3 << endl;
    }
    else
    {
        cout << "All numbers are equal" << endl;
    }

    string ans = ((num1 > num2) && (num1 > num3)) ? "num1 is grater" : (num2 > num1) && (num2 > num3) ? "number 2 is grater "
                                                                   : ((num3 > num1) && (num3 > num2)) ? "num3 is grater"
                                                                                                      : "All number are equal";

    cout << endl
         << endl;

    cout << ans << endl;

    return 0;
}

```
## String to lowercase and or case practice

```c++
#include <bits/stdc++.h>
#include <cstring>
using namespace std;

// logical operators (and = && , or = ||, not = !)

int main()
{
    string day;
    cout << "Enter the name of day: " << endl;
    cin >> day;

    transform(day.begin(), day.end(), day.begin(), ::tolower);

    cout << day << endl;

    if (day == "monday" || day == "friday")
    {
        cout << "Ring the alram" << endl;
    }
    else
    {
        cout << "stop the alarm" << endl;
    }
}

```
## Assignment Operator: 

```c++
#include <bits/stdc++.h>
#include <cstring>
using namespace std;

// logical operators (and = && , or = ||, not = !)

int main()
{
    int a = 10;
    a += 1; // 11
    cout << a << endl;

    a -= 2; // 9
    cout << a << endl;

    a *= 2; // 18
    cout << a << endl;

    a /= 2; // 9
    cout << a << endl;

    a %= 2; // 1
    cout << a << endl;

    return 0;
}

```

