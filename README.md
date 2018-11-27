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

### Pandas Cheat Sheet

#### DataFrame Commands
| Command                                                         | Description                                                                                      |
|-----------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| df.head()                                                       | Displays first 5 rows                                                                            |
| df.tail()                                                       | Displays last 5 rows                                                                             |
| df.shape                                                        | Displays the shape of the dataframe ( rows x columns x pages )                                   |
| df.columns                                                      | Displays column header labels (can be coerced to list using list())                              |
| df.index                                                        | Displays the index ('row header') of the dataframe                                               |
| df.index.name                                                   | Displays the name of the index (None by default), settable property                              |

#### Selecting, Renaming, and Summary Commands
| Command                                                         | Description                                                                                      |
|-----------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| df['column']                                                    | Returns a single column as a `pd.Series` object                                                  |
| df[[ 'column' ]]                                                | Returns a single column as a `pd.DataFrame` object                                               |
| df[[ 'column1', 'column2' ]]                                    | Returns multiple columns as a `pd.DataFrame` object                                              |
| df.rename(columns={'old_name':'new_name'}, inplace=True)        | Overwrites column 'old_name' with column 'new_name'                                              |
| df.columns = ['new_col1', 'new_col2']                           | Overwrites a 2-column-wide DataFrame with names 'new_col1' and 'new_col2'                        |
| df.describe()                                                   | Returns descriptive statistics for numeric values in DataFrame (min, max, etc.)                  |
| df['column'].unique()                                           | Returns distinct values for 'column'                                                             |
| df['column'].nunique()                                          | Returns count of distinct, non-null values in 'column'                                           |
| df['column'].value_counts()                                     | Returns count of rows, grouped by distinct value in 'column'                                     |

#### Filtering and Sorting
| Command                                                         | Description                                                                                      |
|-----------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| df[ df['column'] < 50 ]                                         | Returns pd.Series object of 'column' where value is less than 50                                 |
| df [ ( df['column1'] < 50 ) &  ( df['column2'] == 'purple' ) ]  | Returns pd.Series object where 'column1' is less than 50 AND 'column2' has string value 'purple' |
| df.sort_values(by='column', ascending = False)                  | Returns pd.Series object, sorted by column 'column', biggest to smallest                         |

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
