# Chapter 1. Getting Started

## Exercise 1.6

> Explain whether the following program fragment is legal

It's illegal.

**`[Error] expected primary-expression before '<<' token`**

Fixed it: remove the spare simicolons.

```cpp
std::cout << "The sum of " << v1
          << " and " << v2
          << " is " << v1 + v2 << std::endl;
```

## Exercise 1.8

> Indicate which, if any, of the following output statements are legal:

```cpp
std::cout << "/*";
std::cout << "*/";
std::cout << /* "*/" */;
std::cout << /* "*/" /* "/*" */;
```

> After you’ve predicted what will happen, test your answers by compiling a program with each of these statements. Correct any errors you encounter.

Correction:
```cpp
std::cout << "/*";
std::cout << "*/";
std::cout << /* "*/" */";
std::cout << /* "*/" /* "/*" */;
```