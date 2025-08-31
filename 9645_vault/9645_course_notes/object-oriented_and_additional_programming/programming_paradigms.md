
For your syllabus, you need to be able to:

- Know why the object-oriented paradigm is used

- Explain the term 'imperative high-level language'

- Answer theory questions in the CS04 exam about the functional programming paradigm


*It is helpful to have a wider understanding of programming paradigms - see notes and examples below.*


----

## Functional Programming

In the functional programming paradigm, functions are treated as first-class objects, meaning they can be assigned to variables, passed as arguments, and returned from other functions. Programs are built by composing pure functions, which accept arguments and return results without altering global state. These functions are stateless and must always produce the same output for the same input, with no side effects such as modifying variables outside their scope or performing I/O operations.


```python
from functools import reduce

# Pure functions
def square(x):
    return x * x

def is_even(x):
    return x % 2 == 0

def add(x, y):
    return x + y

# Functional programming pipeline
numbers = [1, 2, 3, 4, 5]
squared = map(square, numbers)
evens = filter(is_even, squared)
result = reduce(add, evens, 0)

print(result)  # Output: 20
````

---

## Imperative Programming

Imperative programming follows a step-by-step approach where each line of code explicitly tells the computer what to do in a specific sequence. This paradigm focuses on controlling the flow of execution using loops, conditionals, and state changes. Procedures within the program manipulate global or shared variables to achieve the desired results, and side effects are expected and common.

*Imperative programming can be contrasted to functional programming as shared state (i.e. global data) is a common feature.*

*Imperative programming can also be contrasted to declarative programming (see below) as a program specifically outlines the steps required to solve a problem, rather than just a description of what the results should be.*

```python
# Imperative programming example
numbers = [1, 2, 3, 4, 5]
squared = []
for number in numbers:
    squared.append(number * number)

evens = []
for number in squared:
    if number % 2 == 0:
        evens.append(number)

result = 0
for number in evens:
    result += number

print(result)  # Output: 20
````

---

## Object-Oriented Programming

Object-oriented programming organises code into objects, which are instances of classes. A class serves as a blueprint, defining properties (attributes) and methods (functions) that encapsulate related logic and data. Objects maintain their own internal state, and direct access to another object's state is discouraged. Instead, objects communicate through well-defined interfaces, promoting encapsulation and modularity.


```python
class Gadget:
    def __init__(self, name, price):
        self.name = name
        self.price = price

    def apply_discount(self, discount):
        self.price *= (1 - discount)

# Create instances
phone = Gadget("Phone", 1000)
laptop = Gadget("Laptop", 2000)

# Apply a discount
phone.apply_discount(0.1)
print(phone.price)  # Output: 900
````

## Low-Level Programming

Low-level programming involves direct manipulation of the hardware through basic instructions such as memory I/O operations and branching. This paradigm operates close to the machine, often bypassing abstractions provided by high-level languages. Programmers write code that directly interacts with registers, memory addresses, and CPU instructions, which can yield high performance but requires meticulous attention to detail.


```asm
; Assembly example (x86 NASM syntax)
section .data
    result db 0

section .text
    global _start

_start:
    mov al, 5       ; Load 5 into register AL
    add al, 10      ; Add 10 to AL
    mov [result], al ; Store result in memory

    ; Exit program
    mov eax, 60
    xor edi, edi
    syscall
````

---

# Declarative Programming

Declarative programming describes **what** the program should accomplish rather than **how** to accomplish it. It abstracts away the control flow and implementation details, allowing the programmer to focus on specifying the desired outcome. Common declarative paradigms include SQL for databases and functional-style list comprehensions in Python.


```python
# Declarative programming example with list comprehensions
numbers = [1, 2, 3, 4, 5]
result = sum(x * x for x in numbers if (x * x) % 2 == 0)
print(result)  # Output: 20
````

```SQL
SELECT amount FROM transaction WHERE amount > 10 AND suspicious_flag = TRUE
```
---

# Logic Programming

Logic programming uses a declarative approach where the programmer defines facts and rules, and the system deduces the solution by applying logical inference. Prolog is a common language for logic programming, allowing programs to solve problems by reasoning over a defined set of relationships and constraints.

```prolog
% Prolog example
even(X) :- 0 is X mod 2.
square(X, Y) :- Y is X * X.
sum([], 0).
sum([H|T], S) :- sum(T, ST), S is H + ST.

process_numbers(Numbers, Result) :-
    findall(S, (member(X, Numbers), square(X, SX), even(SX), S = SX), Squares),
    sum(Squares, Result).

% Query:
% ?- process_numbers([1, 2, 3, 4, 5], Result).
% Result = 20.
```