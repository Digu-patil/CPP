# endl

```
//Code 1 = 
#include<iostream>
int main()
{
    std::cout <<"Hello";
    std::cout <<"World";
    return 0;
}
```
- Output of this code is "HelloWorld"
- Note that this output on the terminal happend without and space or newline

```
//Code 2= Added a new line with "\n" 
#include<iostream>
int main()
{
    std::cout <<"Hello\n";
    std::cout <<"World";
    return 0;
}
```
- Output is "Hello" in one line and "World" in 2nd line

```
#include<iostream>
int main()
{
    std::cout <<"Hello" << std::endl;
    std::cout <<"World" << std::endl;
    return 0;
}
```
- Output using endl here is same as using "\n"
- This is becauase endl add a new line and move the cursor to the start of the 2nd line.
- But it does one more important thing - It flushes the output right away and does not wait for the entire program to run
- endl ensures that the outout that the program has generated so far, is printed, instead of waiting in the memory to be written.

>Note - endl is a manipulator that functions like a object.



Key Differences
|endl                       | \n                                         |
|---------------------------|--------------------------------------------|
|Flushes the output direclty| Waits for the entire program to be executed|
|Does not take any memorey  | Takes 1 byte of memoery|