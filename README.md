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

´´´
>>> cubes = [ (x, x**3) for x in range(1,6)]
>>> cubes
[(1, 1), (2, 8), (3, 27), (4, 64), (5, 125)]

list= [item for item in range(1,30) if item%3 == 0]
>>> list
[ 3, 6, 9, 12, 15, 18, 21, 24, 27]

´´´

Set Comprehension:

Dictionary Comprehension:

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

