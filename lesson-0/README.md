# Lesson 0: Program Structure and Output 
### Hello, world!

When you create a basic program in Visual Studio, it will likely have one file
that looks something like this (and as a side note, anything that begins with `//` is
a 'comment', which is not part of the program and only for explanation):

```cpp
int main() {
	// The program begins here


	// The program ends at the line below
	return 0;
}
```

The function `main` is where all C++ programs start. When `main` finishes running,
the program finishes running. If you click the run button at the top, then... you may see a screen pop up briefly
and then disappear. This is normal! The program started at the top, and then stopped when it reached `return 0;`,
which in this case is the end of the program. 

```cpp
// This tells the program that it should use all the stuff in 'iostream'
// 'iostream' includes a variety of things for printing and reading text
#include <iostream>

int main() {
	// The program still starts here

	// This line prints out a message.
	std::cout << "Hello, world!\n";

	// And the program still ends here
	return 0;
}
```

This is a more interesting program--it actually does something! Press Ctrl-F5 to try it out.
You should see the message appear on the screen.

### Exercises

Try removing the `\n` at the end of the middle line, see what it does!