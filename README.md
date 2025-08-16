 # ascii 
if i want to add number in string ,i would to add the number and caracter of 0 '0'
- example {
string str=" ";
str = 1 + '0'
}
# modulas
if i want to print the last digit in the integer i would to use 'modulas' = '%'
- example {
- int num= 1994;
- cout<<num % 10;
- }

## 1. Ceiling Function (`ceil`)
If I want to round up a number to the nearest integer, I can use `ceil()`.  
### Example:
```cpp
#include <iostream>
#include <cmath>
using namespace std;
int main() {
    double num = 6.2;
    cout << ceil(num); // Output: 7
    return 0;
}
______________________________________________________________________________________________________________________________________________________________________________
#long long
If I need to handle very large numbers, I should use long long instead of int to avoid overflow.
long long n, m, a;
cin >> n >> m >> a;
long long tiles = (n + a - 1) / a * ((m + a - 1) / a);
cout << tiles;
#checking if integer
double num = 4.0;
if (num == (int)num) {
    cout << "Integer";
} else {
    cout << "Not an integer";
}
______________________________________________________________________________________________________________________________________________________________________________
# unordered_map
if i have an string and the string is join a name and integer i can use unordered_map
- example
#include <iostream>
#include <unordered_map>
using namespace std;

int main() {
    unordered_map<string, int> faces = {
        {"Tetrahedron", 4},
        {"Cube", 6},
        {"Octahedron", 8},
        {"Dodecahedron", 12},
        {"Icosahedron", 20}
    };

    cout << faces["Cube"]; // Output: 6
    return 0;
}
______________________________________________________________________________________________________________________________________________________________________________
# gcd
the library is algorithm
this function is used to get the biggest common dinomanator
- example
if(__gcd(a,b)==1)
______________________________________________________________________________________________________________________________________________________________________________
# sort
the library is algorithm
this function is used to arrange the number from smaller to greater or from greater to smaller
- example
sort(num,num+n);
______________________________________________________________________________________________________________________________________________________________________________# min
The main function of min in C++ is to return the smaller of two values. It is a standard utility function defined in the <algorithm> header.
- example
int x = 5, y = 8;
int m = min(x, y);  // m = 5
___________________________________________________________________________________________________________________________________________________________________
## Queue مع Pair في C++

- `queue` هو حاوية بتنظم العناصر بنظام **FIFO (First In, First Out)**.
- تقدر تخزن **زوج من القيم (pair)** جوه queue بسهولة.

### مثال عملي
```cpp
#include <iostream>
#include <queue>
using namespace std;

int main() {
    queue<pair<int,int>> q;

    q.push({5, 1});   // (value=5, index=1)
    q.push({10, 2});  // (value=10, index=2)
    q.push({15, 3});  // (value=15, index=3)

    cout << "Front: (" 
         << q.front().first << ", " 
         << q.front().second << ")" << endl;

    q.pop(); // مسح أول عنصر

    cout << "New Front: (" 
         << q.front().first << ", " 
         << q.front().second << ")" << endl;

    return 0;
}

