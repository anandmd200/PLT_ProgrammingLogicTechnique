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

