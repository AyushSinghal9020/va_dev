# Quick Docs

Assume we have a `C++` file like 

```
#include <iostream>

int func_1(int x , int y){
    
    std::cout << "Hello World! 1";
    
    return x;
}
```
To use the function 
```
from va_dev import va_dev as vdev

obj = vdev()

lib = obj.load_lib('absolute path to the C++ file' , 'c++')

file = obj.load_func('func_1' , args = [0 , 1])

print(file)
```
```
0
```
