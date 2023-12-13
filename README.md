Writing and Running C Code in Google Colab:
Writing C Code:
You can create a C file using the %%writefile magic command followed by the file name and your C code. Let's create a simple C program that prints "Hello, world!".


%%writefile hello.c

#include <stdio.h>

int main() {
    printf("Hello, world!\n");
    return 0;
}
This code creates a file named hello.c containing the C code.

Compiling and Running C Code:
After writing the C code, compile it using the !gcc command (the C compiler in this case) and then execute the generated executable.


!gcc hello.c -o hello_c
!./hello_c
The first command (!gcc hello.c -o hello_c) compiles the C code into an executable named hello_c. The second command (!./hello_c) executes the compiled program.

Writing and Running C++ Code in Google Colab:
Writing C++ Code:
Similarly, you can create a C++ file using the %%writefile magic command followed by the file name and your C++ code. Let's create a simple C++ program that prints "Hello, world!".

%%writefile hello.cpp

#include <iostream>
using namespace std;

int main() {
    cout << "Hello, world!" << endl;
    return 0;
}
This code creates a file named hello.cpp containing the C++ code.

Compiling and Running C++ Code:
Unlike C, C++ code needs to be compiled with the !g++ command (the C++ compiler) and then executed.


!g++ hello.cpp -o hello_cpp
!./hello_cpp
The first command (!g++ hello.cpp -o hello_cpp) compiles the C++ code into an executable named hello_cpp. The second command (!./hello_cpp) executes the compiled program.

Important Notes:
Ensure that the necessary compiler (gcc for C and g++ for C++) is available in the Colab environment. Typically, Colab has these compilers pre-installed.
Adjust the file names and compilation commands accordingly if you're working with different file names or multiple source files.
You can also add flags like -std=c++11 to specify the C++ version or other necessary flags for compilation.
