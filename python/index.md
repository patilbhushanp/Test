## Python

### Object Oriented Programming

**Class creation syntax**

```python
# Class name and usage
class ClassName():

  # class level attribute
  classLevelAttribute = ''

  # Constructor declaration
  def __init__(self, param1, param2):
    #instance attribute param1 initialization
    self.param1 = param1
    #instance attribute param2 initialization
    self.param2 = param2
  
  #Method declaration
  def method(self):
    //some operation
    print(f'Instance Parameter 1  : {self.param1}')
    print(f'Class Level Parameter : {ClassName.classLevelAttribute}')
```
