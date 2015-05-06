# Chapter 1

## 1.6 Exercises

1. The functional decompositional method consists of breaking down tasks into smaller tasks.
2. Functional programming is a way of describing processes as small reusable functions rather than monolithic procedural blocks.
3. C and C++ are both compiled programming languages for use in creating software.
4. Data, algorithms, and program syntax.

# Chapter 2

## 2.8 Exercises

1. The `main()` function.
2. `std::cout << "I am learning how to write programs in C.";`.
3. `std::cout << "I am learning how to write programs in C.\nMeanwhile I am learning how to write programs in C++.";`.
4. `std::cout << "I am learning how to write programs in C.\nMeanwhile I am learning how to write programs in C++.\a\a\a";`.
5. `r = PI / 2 + 1; area = PI * r * r;`.
6. The first is a post-increment, the second is a pre-increment. Post-increment returns the value and then increments the number, while pre-increment increments the number and then returns the incremented value.
7. It will output 3, 3, 4, 4, 5, 5, 6.
8. It will output 3, 4, 4, 5, 5, 6, 6.
9. `cout << "THEODOR";`.
10. The quotient 40 and it's because C performs type casting. For a more accurate result, the numbers can be coerced to float: `(float)(201) / (float)(5)`.
11. `333.3 % 5` is `3.3`.
12. `3 % 2` is `1`, quotient is 1. `1 % 4` is `1`, quotient 0. Result is `11`.

# Chapter 3

## 3.6 Exercises

```cpp
// Exercise 1.
#include <iostream>

int main() {
	int a, b;
	std::cin >> a >> b;
	std::cout << "The larger number is: " << (a > b) ? a : b;
	return 0;
}
```

```cpp
// Exercise 2.
if (a == b) {
	std::cout << "The numbers are equal!";
} else {
	std::cout << "The larger number is: " << (a > b) ? a : b;
}
```

```cpp
// Exercise 3.
#include <iostream>

int main() {
	int a;
	std::cin >> a;

	switch (a) {
		case 1:
			std::cout << "I";
		case 5:
			std::cout << "V";
		case 10:
			std::cout << "X";
		case 50:
			std::cout << "L";
		case 100:
			std::cout << "C";
		case 500:
			std::cout << "D";
		case 1000:
			std::cout << "M";
	}

	return 0;
}
```

```cpp
// Exercise 4.
#include <iostream>

int main() {
	int a;
	std::cin >> a;

	if (a < 40) {
		std::cout << "Fail";
	} else if (a < 60) {
		std::cout << "Pass";
	} else if (a < 75) {
		std::cout << "Merit";
	} else {
		std::cout << "Distinction";
	}

	return 0;
}
```

Exercise 5.

- Mon: game.
- Tue: read.
- Wed: party.
- Thu: write.
- Fri: sport.
- Sat: read.
- Sun: read.

6.a: No quotes.

6.b: No double equals.

6.c: 5.

6.d: "i != 0"

# Chapter 4

## 4.6 Exercises

```cpp
// Exercise 1.
#include <iostream>
using namespace std;

int main() {
	for (int i = 1; i <= 9; i++) {
		cout << '*';
	}

	return 0;
}
```

```cpp
// Exercise 2.
#include <iostream>
using namespace std;

int main() {
	for (int i = 1; i <= 9; i++) {
		cout << i << ' ';
	}

	return 0;
}
```

```cpp
// Exercise 3.
#include <iostream>
using namespace std;

int main() {
	for (int i = 1; i <= 9; i++) {
		cout << '*' << '\n';
	}

	return 0;
}
```

```cpp
// Exercise 4.
#include <iostream>
using namespace std;

int main() {
	for (int i = 1; i <= 9; i++) {
		cout << i << '\n';
	}

	return 0;
}
```

```cpp
// Exercise 5.
#include <iostream>
using namespace std;

int main() {
	for (int i = 1; i <= 9; i++) {
		for (int j = 1; j <= 9; j++) {
			cout << '*';
		}
		cout << '\n';
	}

	return 0;
}
```

```cpp
// Exercise 6.
#include <iostream>
using namespace std;

int main() {
	for (int i = 1; i <= 9; i++) {
		for (int j = 1; j <= 9; j++) {
			cout << i;
		}
		cout << '\n';
	}

	return 0;
}
```

```cpp
// Exercise 7.
#include <iostream>
using namespace std;

int main() {
	for (int i = 1; i <= 9; i++) {
		for (int j = 1; j <= i; j++) {
			cout << '*';
		}
		cout << '\n';
	}

	return 0;
}
```

```cpp
// Exercise 8.
#include <iostream>
using namespace std;

int main() {
	for (int i = 1; i <= 9; i++) {
		for (int j = 1; j <= i; j++) {
			cout << i;
		}
		cout << '\n';
	}

	return 0;
}
```

```cpp
// Exercise 9.
#include <iostream>
using namespace std;

int main() {
	int mid = 5;
	for (int i = 0; i < mid; i++) {
		for (int j = 1; j <= 9; j++) {
			int lo = mid - i;
			int hi = mid + i;
			if (j >= lo || j <= hi) {
				cout << '*';
			} else {
				cout << ' ';
			}
			cout << i;
		}
		cout << '\n';
	}

	return 0;
}
```

```cpp
// Exercise 10.
#include <iostream>
using namespace std;

int main() {
	int mid = 5;
	for (int i = 0; i < mid; i++) {
		for (int j = 1; j <= 9; j++) {
			int lo = mid - i;
			int hi = mid + i;
			if (j >= lo || j <= hi) {
				cout << i;
			} else {
				cout << ' ';
			}
			cout << i;
		}
		cout << '\n';
	}

	return 0;
}
```

```cpp
// Exercise 11.
#include <iostream>
using namespace std;

int main() {
	int sum = 0;
	for (int i = 100; i < 1000; i += 2) {
		sum += i;
	}
	cout << sum;

	return 0;
}
```

# Chapter 5

## 5.6 Exercises

```cpp
// Exercise 1.
#include <iostream>
using namespace std;

int main() {
  double a;
  cin >> a;
  cout << PI / 180 * a << endl;

  return 0;
}
```

```cpp
// Exercise 2.
#include <iostream>
#include <cmath>
using namespace std;

int main() {
  double a;
  cin >> a;
  cout << sin(a) << endl;
  cout << cos(a) << endl;

  return 0;
}
```

```cpp
// Exercise 3.
#include <iostream>
#include <cmath>
using namespace std;

int main() {
  double a;
  cin >> a;
  cout << tan(a) << endl;

  return 0;
}
```

For exercise 4, the program will output 232.053 and then 232.

# Chapter 6

## 6.10 Exercises

Q1: a[3] is the null terminator.

```cpp
// Exercise 2.
#include <iostream>
using namespace std;

int main() {
  int sum = 0;
  for (int i = 1; i <= 100; i++) {
    sum += i;
  }
  cout << sum;

  return 0;
}
```

```cpp
// Exercise 3, 4, 5, 6.
#include <iostream>
using namespace std;

void ConvertToBinary(int n) {
  if (n / 2 != 0) {
    ConvertToBinary(n / 2);
  }
  printf("%d", n % 2);
}

int main() {
  int a = 4;
  ConvertToBinary(a);

  return 0;
}
```

# Chapter 7

## 7.6 Exercises

Q1: The first is a pointer declaration, the second a dereference.

# Chapter 8

## 8.10 Exercises

```cpp
// Exercise 1.
#include <iostream>
#include <string>
using namespace std;

string readName() {
  string buf;
  cin >> buf;
  return buf;
}

int main() {
  string name = readName();

  cout << name << endl;

  return 0;
}
```

