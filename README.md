# Experiment-2
## Aim:
The aim of this program is to determine and print the size of various data types in bytes using the sizeof operator in C++.

## Theory:
Data Types and Variables:

Variables a, b, c, d, e, f, g, h, and i are declared to represent different data types (char, int, short int, long int, float, double, long double, bool, wchar_t respectively).

## Sizeof Operator:

The sizeof operator is used to determine the size of each variable in bytes. Each size is printed using std::cout along with appropriate labels.

## Code
### Storage Class
#include<iostream>
using namespace std;

extern int extern_variable =30;


int main()
{
    auto a = 8;
    register int registered_variable = 100;
    static int s = 7;
    cout << "The local variable: "<< a << std::endl;
    cout <<"The variable in register: "<<registered_variable<<endl;
    std::cout<<"External variable: "<<extern_variable<<endl;
    s = 10;
    cout<<"The static variable: "<<s<<endl;

}

/* Output of the following code 

The local variable: 8
The variable in register: 100
External variable: 30
The static variable: 10
*/

### Finding the sizes of primitive datatypes 
#include <iostream>
using namespace std;

int main() 
{
    char a = 's';
    cout << "The size of a character is: "<< sizeof(a) << endl;
    int b = 123456;
    cout << "The size of an integer is: "<< sizeof(b) << endl;
    short int c = 1233;
    cout << "The size of a short integer is: "<< sizeof(c) << endl;
    long int d = 12739482;
    cout << "The size of a long integer is: "<< sizeof(d) << endl;
    long long int e = 122388728;
    cout << "The size of a long long integer is: "<< sizeof(e) << endl;
    float f = 27168.5;
    cout << "The sie of a float is: " << sizeof(f) << endl;
    double g = 84273923.89877;
    cout <<"The size of a double floating point is: "<< sizeof(g) << endl;
    long double h = 8742980.789793;
    cout<< "The size of long double floating point is: "<<sizeof(h) << endl;
    cout<< "The size of a wide character is: "<<sizeof(wchar_t) << endl;
    return 0;
}


/*output

The size of a character is: 1
The size of an integer is: 4
The size of a short integer is: 2
The size of a long integer is: 4
The size of a long long integer is: 8
The sie of a float is: 4
The size of a double floating point is: 8
The size of long double floating point is: 16
The size of a wide character is: 2


*/
## Conclusion:
This program effectively illustrates how to use the sizeof operator to obtain the size of various data types in bytes in C++. The sizes are printed to the console, showing the memory allocation for each type on the specific environment where the program is compiled and executed. The output confirms the standard sizes of these data types on most typical systems, providing valuable information for understanding memory usage and data representation in C++ programming.
