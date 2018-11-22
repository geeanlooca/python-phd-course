# Introduction to Python

## Hello world

```
print('Hello World!')
```

## Data types

- float
- int
- str

Query the type of some variable:

```
type(5)
type(3.2)
```

Cast a value to the desired data type:

```
int(3.4)
float(3)
```

## Comments

Comments are preceded by a '#' sign:

```
# this piece of code will compute the area of a circle given the radius
pi = 3.1415
radius = 2.2
area = pi*(radius**2)
print('The area is {0:.2f}'.format(area) + ' while the radius is ' + str(radius))

```

## User input

```
text = input('How old are you?')
num = int(input('How old are you?'))
print(5*text)
print(5*num)
```

## Lists

```
colors = ['green', 'blue', 'red']
print(colors[0])
colors[2] = 'orange'
print(colors)
colors[-1] = 'yellow' # access the last element of the list
print(colors)
colors[-2] = 'violet' # access the second to last element of the list
print(colors)

```

```
animals = ['cat', 'dog', 'snake', 'fish', 'elephant']
print(animals[1:4]) # print elements from 1 (inclusive) to 4 (exclusive)
print(animals[0:5:2]) # print elements from 1 (inclusive) to 5 (exclusive) jumping by 2 elements
print(animals[::-1]) # print elements in reverse order


# membership
print('dog' in animals)
print(4 in [1,2,3,4])
print('ant' in 'elephant') # works with strings


# additional ops
print(len(animals))
animals.append('horse')
print(len(animals))
```

## Mutability

When assigning a variable, the content is copied => Immutable

```
x = 7
y = x
print(x, y)
x = 8
print(x, y)

y = 9
print(x, y)
```
When assigning a list it works as a C pointer. => Mutable

```
x = [1, 2, 3]
y = x
print(x, y)
x.append(4)
print(x, y)
y.append(4)
print(x, y)
x = [0, 0, 0]
print(x, y)
```


## Tuples
Tuples are immutable lists. They are lightweight are useful when used in dictionaries

```
a_tuple = ('one', 'two')
type(a_tuple)

another_tuple = ('one', )
not_a_tuple = ('one')
type(another_tuple)
type(not_a_tuple)

print([1, 'two'] == (1, 'two'))
```

## Dictionaries

```python
birth_year = {'Hamilton': 1755, 'Jefferson':1245}
birth_year_2 = dict('Hamilton': 1755, 'Jefferson'=1245)
```

## Sets

## Functions

## Lambdas
lambda functions are inline functions that don't need a function definition with def

```
animals = ['cat', 'dog', 'Fish']
print(sorted(animals)) # sorts the animals list
print(sorted(animals, key=lambda a : a.lower())) # sorts the animals list but using the lowercase item in the list as the key
```



