# pandas-cute
**pandas_cute** is a simple data analysis library based on Numpy that emulates the functionality of the pandas library .

## Functionality
pandas_cute has limited functionality but is still capable of a wide variety of data analysis tasks.

- Subset selection with the brackets
- Arithmetic and comparison operators (+, -, <, !=, etc...)
- Aggregation of columns with most of the common functions (min, max, mean, median, etc...)
- Grouping via pivot tables
- Grouping via pivot tables
- Reading in simple comma-separated value files
- Several other methods

## How To Use
 ```python
    import pandas_cute as pdc
```
## Example
```python
# create data
students = np.array(['Tom', 'Tom', 'Jack', 'Jack'])
courses = np.array(['Math', 'English', 'Math', 'English'])
scores = np.array([70, 65, 67, 91])
data = {'students': students, 'courses': courses, 'scores': scores}
#  create DataFrame
df = pdc.DataFrame(data)
```

|     | students  | courses | scores |
|  ----  | ----  | ----| ---- |
| 0  | Tom | Math | 70 |
| 1 | Tom | English | 65 | 
| 2 | Jack | Math | 67 |
| 3 | Jack | English | 91 | 


### **read_csv**()
 ```python
    df = pdc.read_csv('data/employee.csv')
    df.head()
```

### 