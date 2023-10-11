"""
Pandas - Interview Question Solutions

1. What is a Pandas DataFrame?
    - A Pandas DataFrame is a two-dimensional data structure that stores data in tabular form.
    - Data is stored in rows and columns.
    - It is a human-readable way to work with data in Python.

2. What is a Pandas Series?
    - A Pandas Series is a one-dimensional array - you can think of this as one column from a DataFrame.

3. How would you make an empty DataFrame in Python?
"""
    # method 1:
    pd.DataFrame()

    # method 2: save this as a variable
    df = pd.DataFrame()

"""
4. In Pandas, how would you find the number of unique values in a column?
    - There are several ways to accomplish this:
"""
    # Method 1:
    df.value_counts(df[‘column’])

    # Method 2:
    len(pd.unique(df[‘column’])

    # Method 3:
    df[‘column’].nunique()

"""""
5. What are some benefits of using Pandas?
    - Human-readable/friendly
    - Easy manipulation of data thanks to its methods
    - Efficient on large data
    - Made for Python

6. How would you add a column to a pandas DataFrame?
"""
    # Adding empty column:
    df[‘new_col’] = np.nan

    # Adding existing list as new column:
    df[‘new_col’] = my_list

"""
7. How would you rename a column in a Pandas DataFrame?
"""
    # Method 1:
    df.rename(columns = {‘old_name’: ‘new_name’}, inplace = True)

    # Method 2:
    df.columns = [‘col1_new_name’, … ‘coln_new_name’]

"""
8. How would you convert a Pandas DataFrame to a numpy array?
"""
    # Method 1:
    df.to_numpy()

    # Method 2:
    df.values

"""
9. How would you save a Pandas DataFrame to a csv file?
"""
    df.to_csv(‘name.csv’)

"""
10. Define GroupBy in Pandas.
    - Groupby rearranges the data into various groups based on some criteria.
"""
