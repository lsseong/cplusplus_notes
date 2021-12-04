# cplusplus_notes

int x{0} vs int x = 9 - https://stackoverflow.com/questions/20603403/c11-variable-initialization-and-declaration



The first const refers to stored int value (i.e. cannot change value), the second const refers to int address (i.e. cannot change address)
```
int x = 0;
int y = 0;

cont int* const ptr = &x;
*ptr = 9; // not allowed
x = 10; // ok
ptr = &y // not allowed


int* const ptrB = &x
*ptrB = 10; // ok
ptrB = &x; // not allowed

```
