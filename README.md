### Python Programming Exercises 

Here you will find some exercises for python!

<ul>
  <li><a href="./lists/lists.ipynb">Lists</a></li>
  <li><a href="./lists/lists_solutions.ipynb">Lists Solutions</a></li>
</ul>
<ul>
  <li><a href="./functions/functions.ipynb">Functions</a></li>
  <li><a href="./functions/functions_solutions.ipynb">Functions Solutions</a></li>
</ul>
<ul>
  <li><a href="./dictionaries/dictionaries.ipynb">Dictionaries</a></li>
  <li><a href="./dictionaries/dictionaries_solutions.ipynb">Dictionaries Solutions</a></li>
</ul>

### Jupyter Shortcuts
We also have some documentation on helpful jupyter notebook shortcuts:

| Command    | Description                                        |
|------------|----------------------------------------------------|
|  dd        | Deletes current cell                               |
|  a         | Create new cell above the currently selected cell  |
|  b         | Create new cell below the currently selected cell  |
| ctrl+enter | Execute current cell and stay on current cell      |
| shift+enter| Execute current cell and move to cell below        |
| alt+enter  | Execute current cell and create new cell below     |
| m          | Change current cell to a markdown cell             |
| y          | Change current cell to a code cell                 |
| l          | Show / hide line numbers                           |
| o          | Show / hide cell output                            |
| Esc        | Enter command mode                                 |
| Enter      | Enter edit mode                                    |
| h          | Display help screen                                |


### String Formatting

#### Using `.format()` without positional arguments

```python
my_name = 'greg'
my_age = 98
print('My name is {} and my age is {}'.format(my_name, my_age))
```
returns:
```python
My name is greg and my age is 98
```

#### Using `.format()` with positional arguments
```python
my_name = 'greg'
my_age = 98
print('My name is {1} and my age is {0}'.format(my_name, my_age))
```

returns:
```python
My name is 98 and my age is greg
```

#### Using f-strings

```python
my_name = 'greg'
my_age = 98
print(f'My name is {my_name} and my age is {my_age}')
```

returns:
```python
My name is greg and my age is 98
```
