# Experiment 16
# Aim
To study and implement Exception Handling

# Apparatus 
VS code 

# Theory
An exception is an unexpected problem that arises during the execution of a program our program terminates suddenly with some errors/issues. Exception occurs during the running of the program (runtime).
1. try in C++
* The try keyword represents a block of code that may throw an exception placed inside the try block.
* It’s followed by one or more catch blocks. If an exception occurs, try block throws that exception.

2. catch in C++
* The catch statement represents a block of code that is executed when a particular exception is thrown from the try block.
* The code to handle the exception is written inside the catch block.

3. throw in C++
* An exception in C++ can be thrown using the throw keyword.
* When a program encounters a throw statement, then it immediately terminates the current function and starts finding a matching catch block to handle the thrown exception.

# Codes 
~~~
#include <iostream>
using namespace std;

int main()
{
    float n1,n2, ans;
    cout<<"enter the numbers 1 and 2: ";
    cin>>n1>>n2;
    try
    {
        if(n2==0)
        {
            throw n2;
        }
        else
        {
            ans = n1/n2;
            cout<<"answer = "<<ans<<endl;
        }
    }

    catch( float num)
    {
        cout<<"ERROR: division by "<<num<<endl;
    }
}
~~~
![image](https://github.com/user-attachments/assets/011272ae-9c3b-4d6a-99d3-0354f9e816b1)

code 2:
~~~
#include <iostream>
using namespace std;

int main()
{
    int age;
    cout<<"enter age: ";
    cin>>age;
    try
    {
        if (age<18)
        {
            throw age;
        }
        else
        {
            cout<<"age: "<<age<<"\nAPPROVED"<<endl;
        }
    }
    catch(int a)
    {
        cout<<"\nERROR: Underage ("<<age<<")"<<endl;
    }
}
~~~
![image](https://github.com/user-attachments/assets/d288657f-545b-431c-b529-a2e53fd65b63)
