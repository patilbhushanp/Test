##Python

### Functions in pythons:

**Creating function:**
```python
def function_name():
    '''
       Documentation string to explain function work
    '''
    #Function operation implementation
```

**args (Variable argument list) keywords:**

Function Decalaration:
```python
def average(*args):
    '''
       Average function. Taking number as args input and return their average
    '''
    return sum(args) / len(args)
```

Calling example, - 
```python
  print(f'Total Average for (1, 2, 3, 4, 5) is : {average((1, 2, 3, 4, 5))}')
```

**kargs (Key-Value Paired argument) keyword:**

Function Decalaration:
```python
def showStudentInformation(**kargs):
    '''
       show student information function show student name, address, marks and Percentage
    '''
    print(f'========== Student Information ==========')
    print(f'Name         : {kargs["name"]}')
    print(f'Address      : {kargs["address"]}')
    print(f'Marks        : {kargs["marks"]}')
    print(f'Percentage   : {(sum(kargs["marks"]) / len(kargs["marks"])) * 100.00}')
```

Calling example, - 
```python
  showStudentInformation({'name:'John Simth', 'address': 'Pune', 'marks':[120,140,130]})
```

**map built-in function**

- Map modifies the list with a normal logic that produces another list

```python
#Map to return square of each element of list.

# square method
def square(num):
    return num ** 2

print(map(square, [1, 2, 3, 4, 5]))
squareList = list(map(square, [1, 2, 3, 4, 5]))
print(squareList)
Output => [1, 4, 9, 16, 25]
```

**filter built-in function**

- Filter modifies the list with conditional logic that filters out some elements
```python
#Filter to find out even number from list

#is even number function
def isEvenCheck(num):
    return num ** 2

print(filter(isEvenCheck, [1, 2, 3, 4, 5, 6]))
evenList = list(filter(isEvenCheck, [1, 2, 3, 4, 5, 6]))
print(evenList)
Output => [2, 4, 6]
```
