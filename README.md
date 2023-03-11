# 3-card-monte

**String literals can never be updated.** A string literal variable only points to the location of the string literal in the constants section in memory. 

 To update a string, create an array holding a string literal. The string literal assignment will be stored in the constants section as always but its contents will be copied into the array. You can then update your array as much as you like.

**constants are read only i.e. you cannot update them. String literals are constants.

Delaring an array as a function argument  means the array variable is a pointer. 

If you want to set a pointer to a string literal, always use the keyword `const`. That way, if you try to update the string literal you'll get a more elaborate compile error message. 

```c
const char *cpu = "ryzen";
``` 