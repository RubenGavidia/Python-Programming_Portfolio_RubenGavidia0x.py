# Python-Programming_Portfolio_RubenGavidia0x.py
Python-Programming_Portfolio_RubenGavidia0x.py

![image](https://user-images.githubusercontent.com/35381213/140606509-50395f62-4a6e-4078-8ef0-930c28be162d.png)

Natural Language Processing:

Computer Science Thinking:

Object Oriented Programming:

Files:

Exception Handling:

Array Oriented Programming:



List Comprehension:'

```
>>> cubes = [ (x, x**3) for x in range(1,6)]
>>> cubes
[(1, 1), (2, 8), (3, 27), (4, 64), (5, 125)]

multiples = [item for item in range(1,30) if item%3 == 0]
>>> multiples
[ 3, 6, 9, 12, 15, 18, 21, 24, 27]

```
Generator Expresion:
```
list(x ** 3 for x in [10, 3, 7, 1, 9, 4, 2] if x % 2 == 0)
[1000, 64, 8]

```

Set Comprehension:

```
In [1]: numbers = [1, 2, 2, 3, 4, 5, 6, 6, 7, 8, 9, 10, 10]
In [2]: evens = {item for item in numbers if item % 2 == 0}
In [3]: evens
Out[3]: {2, 4, 6, 8, 10}
```

Dictionary Comprehension:
```
grades = {'Sue': [98, 87, 94], 'Bob': [84, 95, 91]}
grades2 = {k: sum(v) / len(v) for k, v in grades.items()}
grades2
{'Sue': 93.0, 'Bob': 90.0}
{ number:number ** 3 for number in range(1,5)}
{1: 1, 2: 8, 3: 27, 4: 64}
```
Functions:
```
import random

def mult(x,y):
    if a == x*y:
        return random.choice(["Nice work!","Very good!","Keep up the good work!"])
    elif a != x*y:
        return random.choice(["No. Please try again.","Wrong. Try once more.","No. Keep trying."])

def mult2(i,k):
    if b == i*k:
        return random.choice(["Nice work!","Very good!","Keep up the good work!"])
    elif b != i*k:
        return random.choice(["No. Please try again.","Wrong. Try once more.","No. Keep trying."])
    
x = random.randrange(1, 10)
y = random.randrange(1, 10)
i = random.randrange(1, 100)
k = random.randrange(1, 100)

difficult = int(input("Guess my number between 1 and 1000 with the fewest guesses \n Please Select the Difficult ENTER: 1 or 2:"))

if difficult == 1:
    a = int(input(f"How much is {x} times {y}: "))
    print(mult(x,y))
    
elif difficult == 2:
    b = int(input(f"How amuch is {i} times {k}: "))
    print(mult2(i,k))
   
    
```

```
import random

aux  = 1
y = random.randrange(1, 1001)

while(aux == 1):
    x = int(input("enter the x value: "))
    if x > y:
        print("Too High. Try again.")
    elif x < y:
        print("Too Low. Try again.")
    elif x == y:
        print("Congratulations. You guessed the number!")
        aux = aux + 1

```

