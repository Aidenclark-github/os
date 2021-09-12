src 
.
├── hellofunc.c
├── hellomake
├── hellomake.c
├── makefile
└── obj
    ├── hellofunc.o
    └── hellomake.o
    
    
    
hellomake.c:

#include <hellomake.h>

int main() {
  // Call a function in another file
  myPrintHelloMake();

  return (0);
}
------

hellofunc.c:

#include <stdio.h>
#include <hellomake.h>

void myPrintHelloMake() {
  printf("Hello makefiles!\n");

  return;
}
------

hellomake.h

void myPrintHelloMake(void);
