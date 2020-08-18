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

** kargs (Key-Value Paired argument) keyword:**

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
