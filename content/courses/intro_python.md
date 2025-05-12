+++
title = "intro to python"
sort_by = "weight"
weight=1
description="introductory python course for the elders"

+++

### 0. Environment Setup and Why Python?

<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/Gn-yD-6cvYg?si=kjd9SloWIacU9w8K"
    title="YouTube video player"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
</iframe>

{% note(center=true, header="Why Python?") %}
Python is a fantastic language to start learning as a beginner as its syntax is similar to english moreso than other languages. On top of that python is an extremely popular and powerful language that is used in many facets of software, for instance, data science, artificial intelligence, web design, etc etc. I often hear the phrase: "Python is the swiss army knife of programming languages." and i wholeheartedly agree.
{% end %}

{% note(center=true, header="Setup") %}
First, we need to set up a couple things.

- [Download and Install Python](https://www.python.org/downloads)
  The latest stable version is fine, but anything over python 3+ is perfect

i am doing this on a windows 10 machine. so we may need a bit more set up. (may have to add to PATH)

i know that python comes with a shell called IDLE that can run python code snippets. i am aware there are websites where you can write python code and it will run it.

but we are taking a real step into the development world. having your own environment makes development personal. caring about your environment setup is fun.

it's time to install an Integrated Development Environment (IDE). I will simply be using Vscode as it's the most popular.

- [Download and install VScode](https://code.visualstudio.com/download)

- [Python VScode Extension download](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

```c,linenos
int main() {
    printf("hello world");

    return 0;
}
```

{% end %}

---

### 1. Hello, World

<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/UAmUz6UlTfU?si=GCLvW8H4G8AtLX5J"
    title="YouTube video player"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
</iframe>

{% note(center=true, header="Hello, World!") %}
now that we have everything set up it is time to write our first program: the "hello world" program.
all the program does, is prints a string of text to the terminal.

this is a long passed down tradition that people do when learning how to program. this can be found in the famous 1978 book: _The C Programming Language_ by Brian Kernighan and Dennis Ritchie.

don't worry we won't be learning c.

Hello, World function in python:

```py, linenos
print("hello, world")
```

see how simple it looks?
in python all we do is use the built in function `print()` and put a "string" of text inside of it.

{% end %}

---

### 2. Data Types and Variables

<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/yHryBiMnmz0?si=b720-b-WBNCpEJ1r"
    title="YouTube video player"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
</iframe>

{% note(center=true header="Data Types") %}
A Data Type is simply telling us what kind of information something is. knowing what type of data something is, lets us know what we can or can't do with it.

starting with the basics, we have four basic Data Types:

- **integer**: (keyword: int) an integer is simply any whole number, positive, negative, or zero
- **float**: (keyword: float) a float is any number with decimal places. postive, negative, or zero
- **string**: (keyword: str) a string is a string of characters, or anything encapsulated inside double quotes ("test") or single quotes ('test')
- **boolean**: (keyword: bool) a boolean only ever True (1) or False (0), it's like a light switch.

```py
int: -123, 0, 32131, 8
float: -12.01, 0.0, 31.30000
str: "hello world", "", "3", "-23", "False", 'True', '', '12.01'
bool: True, False
```

{% end %}

{% note(center=true, header="Variables") %}
**A Variable** is something that holds a piece of data. we define a name, then assign a value to that name.
naming a variable has some rules like: cannot use spaces, cannot start with a number, and only has letters, numbers after start, or underscores. Capitalization does matter.
e.g.

```txt
valid_name: seven_eleven, i, x, iter, test2
invalid: 7eleven, h^k, 2test
```

it's tempting to see the equals sign and immediately think back to math, however all this is doing is assigning value.
you can think of it more as an arrow

```txt
bwandii = 3

is more like this

bwandii <- 3

assigning the value 3 to the variable: bwandii an integer value, 3
```

the reason why i make this distinction is because you can have a statement like this:

```py
x = 3
y = 2
x = x + y
print(x)
```

in math this equation is impossible. but in computer science, this is completely valid statement.
in `x=x+y`
all we are doing is reassigning the variable x to the sum of the current value of x and current value of y
so our print(x) function will print out the integer: 5

in python, we do not need to declare the data type a variable like in other languages.
python will imply the type of the data based on what we are assigning the variable.

```py
# NOTE: the # sign is a special character that denotes a comment.
#       a comment is not read by the interpreter so we can place notes for ourselves)

my_variable = "hello" # str
print(my_variable)
# output: hello

my_variable = 3 # int
print(my_variable)
# output: 3

xyz = my_variable # what data type would xyz be?
print(xyz)
# output: 3
```

{% end %}

### 3. Operators and User Input

{% note(center=true, header="Operators") %}

```py
+  # addition
-  # subtraction
*  # multiplication
/  # division
** # exponential
// # integer division (truncation)
%  # modulus (remainder of division)
```

example:

```py
x = 2
y = 4

z = x - y   # z is -2
z = z + y   # z is 2

m = 5 * 2   # m is 10
m = 5 * 2.0 # m is 10.0  <- what data type is this one?

a = z * y   # a is 8
b = a ** z  # b is 64


b = a / 5   # b is 1.6
b = a // 5  # b is 1
c = a % 5   # c is 3
```

logical operators:

```py
and, or, not
```

{% end %}

{% note(center=true, header="User Input") %}

{% end %}

### 4. Conditional Statements (multiple conditions/nested)

---

### 5. Loops

---

### 6. Lists and Tuples

---

### 7. Revisting Loops, iteration by item

---

### 8. String Methods

---

### 9. Slicing Operator

---

### 10. Dictionaries

---

### 11. Functions

---

### 12. File Handling

---

### 13. Error Handling

---

### 14. List Methods

---

### 15. Modular Programming

---

### 16. Scope

---

### 17. Classes and Objects

---

```

```
