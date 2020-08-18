## Python

### Magic and Dunder method in Python
 - These methods provide flexibility use python built-in function with custom object
 - Here is few magic methods, - 
 
 |Python Built-In Function| Class level method declaration | Description |
 | --- | --- | --- |
 | print{instance} | __str__(self) | This method return instance string representations. |
 | len{instance} | __len__(self) | This method return length attribute of instance. |
 | del instance| __del__(self) | This method delete instance from memory. |
 
 - Example. -
   ```python
   #class to store book information.
   class BookInformation():
       def __init__(self, bookName, bookAuthor, bookPages):
           self.bookName = bookName
           self.bookAuthor = bookAuthor
           self.bookPages = bookPages
           print('BookInformation instance created.')
   
       def __str__(self):
           return f'Name - {self.bookName} Author - {self.bookAuthor} Pages - {self.bookPages}'
       
       def __len__(self):
           return self.bookPages
       
       def __del__(self):
           print(f'Deleting book information of name - {self.bookName}')
```
