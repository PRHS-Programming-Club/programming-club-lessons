# Lesson 1: Variables and Input
### Change comes from within

Having output in our programs is nice, but it doesn't make for a very interesting program. It's really quite useless.
So, take a look at this program:

```cpp
#include <iostream> 

int main() {
	// This creates a variable named 'theAnswer' that is equal to 42
	int theAnswer = 42;

	std::cout << "The answer is " << theAnswer << "\n";

	return 0;
}
```

If you run this with Ctrl-F5, it will print 42, which is suspiciously similar to the number we wrote in the program.
What we have done here is made a *variable*, which is essentially a name that was a value. Let's look a little more closely
at that new line:

```cpp
// --- type ---   --- name ---    =   --- value ---
       int         theAnswer      =        42
```

The first part of that line is the variable's *type*. Every variable in C++ has a certain definite type which cannot change at all.
In this case, the type is `int`, which stands for 'integer', so our variable can hold--surprise!--integers.
There's a variety of different usable types, but here's a list of the common ones:

| Type          | Holds      | Examples        |
| ------------- | ---------- | --------------- |
| `int`         | Integers   | -5, 0, 125      |
| `double`      | Decimals   | 3.0, -0.254     |
| `bool`        | True/False | true, false     |
| `char`        | Symbols    | 'a', '%', '4'   |
| `std::string` | Words      | "Hello, world!" |

A note about `std::string`: you will need to add `#include <string>` at the top of your program for it to be available. All of the other types
are available by default.

```cpp
// It's my favorite
int favoriteNumber = 6;

// Just kidding, it's actually 2
favoriteNumber = 2;

std::cout << "The favorite number is " << favoriteNumber << "\n";
```

Variables, as their name implies, can vary. I changed my favorite number halfway through the program, completely getting rid of the old value and replacing it with the new one: 2.

```cpp
int favoriteNumber = 0;

std::cout << "Enter your favorite number: ";

std::cin >> favoriteNumber;

std::cout << "Your favorite number is " << favoriteNumber << "\n";
```

### Exercises
