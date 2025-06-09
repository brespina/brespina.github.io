+++
title = "intro to python"
sort_by = "weight"
weight=1
description="introductory python course for the elders"

+++

### welcome

{% note(center=true, header="welcome!") %}
this course is a passion project, growing up i admired sal khan (and still do) for creating khan academy.

i plan to make more courses, they will always be free, i will never ask for your email or other personal information.

education should be free. i often say this. and i vehemently believe it.

so here is my contribution
{% end %}

### preface

{% note(center=true, header="my advice") %}
i am so glad you are here to learn more about programming.

my goal is to write this course as if i am teaching my own parents/family elders, some of whom only recently discovered `ctrl + f`.

try to stay away from chatgpt or other large language models, unless it's for detailed studying. you are here on this page for a reason.

don't allow chatgpt to do your learning for you. either use chatgpt to enhance your studies, or wait until after the course for further exploration.

don't be afraid of error messages. most of my learning and education comes from error messages.

error messages are the single greatest learning tool that is at your disposal. use them!

doing this, you will learn much faster and have more of an understanding of programming in general.

never stop asking "what happens when i do this instead?" or "what if i leave this part out?" etc etc.

try to break things. have fun.
{% end %}

### expectations

{% note(center=true, header="what can you expect out of this course") %}
backstory: one of my favorite professors, Dr. Gooch, taught in an unconventional way. he didn't believe in exams. 

instead we had one big project, broken up into checkpoints, that tested our comprehension of the material. 

each checkpoint built on top of the last. 

when you stop and think about what is computer science, you begin to question why aren't most classes taught this way?

we will be doing the same thing here.

by the end we will have a project that manages 

{% end %}

### 0. environment setup and why python?

<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/gn-yd-6cvyg?si=kjd9slowiacu9w8k"
    title="youtube video player"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
</iframe>

{% note(center=true, header="why python?") %}
python is a fantastic language to start learning as a beginner as its syntax is similar to english moreso than other languages. on top of that python is an extremely popular and powerful language that is used in many facets of software, for instance, data science, artificial intelligence, web design, etc etc. i often hear the phrase: "python is the swiss army knife of programming languages." and i wholeheartedly agree.
{% end %}

{% note(center=true, header="setup") %}
first, we need to set up a couple things.

- [download and install python](https://www.python.org/downloads)
  the latest stable version is fine, but anything over python 3+ is perfect

i am doing this on a windows 10 machine. so we may need a bit more set up. (may have to add to path)

i know that python comes with a shell called idle that can run python code snippets. i am aware there are websites where you can write python code and it will run it.

but we are taking a real step into the development world. having your own environment makes development personal. caring about your environment setup is fun.

it's time to install an integrated development environment (ide). i will simply be using vscode as it's the most popular.

- [download and install vscode](https://code.visualstudio.com/download)

- [python vscode extension download](https://marketplace.visualstudio.com/items?itemname=ms-python.python)

```c,linenos
int main() {
    printf("hello world");

    return 0;
}
```

{% end %}

---

### 1. hello, world

<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/uamuz6ultfu?si=gclvw8h4g8atlx5j"
    title="youtube video player"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
</iframe>

{% note(center=true, header="hello, world!") %}
now that we have everything set up it is time to write our first program: the "hello world" program.
all the program does, is prints a string of text to the terminal.

this is a long passed down tradition that people do when learning how to program. this can be found in the famous 1978 book: _the c programming language_ by brian kernighan and dennis ritchie.

don't worry we won't be learning c.

hello, world function in python:

```py, linenos
print("hello, world")
```

see how simple it looks?
in python all we do is use the built in function `print()` and put a "string" of text inside of it.

{% end %}

---

### 2. data types and variables

<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/yhrybimnmz0?si=b720-b-wbncpej1r"
    title="youtube video player"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
</iframe>

{% note(center=true header="data types") %}
a data type is simply telling us what kind of information something is. knowing what type of data something is, lets us know what we can or can't do with it.

starting with the basics, we have four basic data types:

- **integer**: (keyword: int) an integer is simply any whole number, positive, negative, or zero
- **float**: (keyword: float) a float is any number with decimal places. postive, negative, or zero
- **string**: (keyword: str) a string is a string of characters, or anything encapsulated inside double quotes ("test") or single quotes ('test')
- **boolean**: (keyword: bool) a boolean only ever true (1) or false (0), it's like a light switch.

```py
int: -123, 0, 32131, 8
float: -12.01, 0.0, 31.30000
str: "hello world", "", "3", "-23", "false", 'true', '', '12.01'
bool: true, false
```

{% end %}

{% note(center=true, header="variables") %}

## **a variable** is something that holds a piece of data. we define a name, then assign a value to that name.

naming a variable has some rules like: cannot use spaces, cannot start with a number, and only has letters, numbers after start, or underscores. capitalization does matter.
e.g.

```txt
valid_name: seven_eleven, i, x, iter, test2
invalid: 7eleven, h^k, 2test
```

## **assignment**

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
x = x + 1
print(x)  # 4 is printed
```

this is why the equals sign, `=` is better to be thought of as "assignment."

in math this equation: `x=x+1` is impossible. but in computer science, this is completely valid statement.
in `x=x+y`
all we are doing is reassigning the variable x to the sum of the current value of x and 1
so our print(x) function will print out the integer: 4

in python, we do not need to declare the data type a variable like in other languages.
python will imply the type of the data based on what we are assigning the variable.

```py
# note: the # sign is a special character that denotes a comment.
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

### 3. operators and user input

{% note(center=true, header="operators") %}

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

we will dive deeper into these in the next section but i wanted to let you know they exist.

{% end %}

{% note(center=true, header="user input") %}

## user inputs

now is where the fun begins.

personally this is where i began to love programming. with user inputs, coding now can become a conversation.

our silly little characters typed on a keyboard can now interact with us!

to ask for the user's input all we have to do is this:

```py
input()
```

this is a valid input function call. however, it is quite confusing to the user. the program will wait for user's input, but since there is no message, the user will not know what to do!

let's fix this by clarifying what we want our input to be.

```py
input("Please input an integer")  # pop quiz! what is an integer?
```

we use the built-in `input()` function and place our question inside the double quotes.

in your IDE, try out this small program and test out variations on different data types!

i am going to test you a little bit with what we have learned thus far.

```py
print("hello there, i sell water bottles")
x = input("how many water bottles would you like?")
print("you would like this many water bottles: ", x)  # bit of a different print function usage but see what it does!
```

{% end %}

### 4. conditional statements (multiple conditions/nested)

---

### 5. loops

---

### 6. lists and tuples

---

### 7. revisting loops, iteration by item

---

### 8. string methods

---

### 9. slicing operator

---

### 10. dictionaries

---

### 11. functions

---

### 12. file handling

---

### 13. error handling

---

### 14. list methods

---

### 15. modular programming

---

### 16. scope

---

### 17. classes and objects

---

```

```

```

```
