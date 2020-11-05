# Handling_duplicate_value_using_pandas_in_python
Question: How can you handle duplicate values in a dataset for a variable in Python using pandas?
Suppose, you are given the following dataset:
df = pd.read_csv('file.csv')
This dataset has many duplicate values. You need to identify them and also remove them.

We can check duplicate value using 
DataFrame.duplicated(subset=None, keep='first')
Return boolean Series denoting duplicate rows.

Considering certain columns is optional.

Parameters
subsetcolumn label or sequence of labels, optional
Only consider certain columns for identifying duplicates, by default use all of the columns.

keep{‘first’, ‘last’, False}, default ‘first’
Determines which duplicates (if any) to mark.

first : Mark duplicates as True except for the first occurrence.

last : Mark duplicates as True except for the last occurrence.

False : Mark all duplicates as True.

Returns
Series
Boolean series for each duplicated rows.
