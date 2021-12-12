# Python-Programming_Portfolio_RubenGavidia0x.py
Python-Programming_Portfolio_RubenGavidia0x.py

![image](https://user-images.githubusercontent.com/35381213/140606509-50395f62-4a6e-4078-8ef0-930c28be162d.png)

Natural Language Processing:

Computer Science Thinking:

Object Oriented Programming:

Files:

Exception Handling:

Strings and Regular Expressions ( regex )

Array Oriented Programming:

```
1 (IPython Session) Given the following 
 dictionary;

temps = {'Mon': [68, 89], 'Tue': 
       [71, 93], 'Wed': [66, 82],
       'Thu': [75, 97], 'Fri': [62, 79]}

perform the following tasks:

a) Convert the dictionary into 
the DataFrame named temperatures 
with 'Low' and 'High' as 
the indices, then display 
the DataFrame .

tempsdf = pd.DataFrame(data = temps,index=['Low','High'])
tempsdf

Mon	Tue	Wed	Thu	Fri
Low	68	71	66	75	62
High	89	93	82	97	79

b) Use the column names to 
select only the columns 
for 'Mon' through 'Wed' .

# tempsdf.T.iloc[0:3] I am not use column names 
tempsdf.T.loc['Mon':'Wed'].T 

In [5]: temperatures.loc[:, 'Mon':'Wed'] # (b)
Out[5]:
Mon Tue Wed
Low 68 71 66
High 89 93 82

c) Use the row index 'Low' 
to select only the low 
temperatures for each day.

# tempsdf.iloc[0,:] 
tempsdf.loc['Low',:]

Mon    68
Tue    71
Wed    66
Thu    75
Fri    62
Name: Low, dtype: int64

d) Set the floating-point 
precision to 2, then 
calculate the average 
temperature for
each day.

pd.set_option('precision', 2)
tempsdf.mean()

Mon    78.5
Tue    82.0
Wed    74.0
Thu    86.0
Fri    70.5
dtype: float64


e) Calculate the average low 
 and high temperatures.

tempsdf.mean(axis=1)
Low     68.4
High    88.0
dtype: float64

```

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

