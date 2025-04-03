
![pandas](https://github.com/user-attachments/assets/4f7c8730-4337-4634-9718-e29f2ea5700e)

# Pandas-practice
A hands-on repository designed to help users practice and master pandas, one of Python's most powerful libraries for data manipulation and analysis. This collection features detailed examples of pandas functions and methods, applied in various contexts, making it ideal for learners and professionals alike

# Pandas Functions & Methods Guide

## Overview
This document provides a categorized reference of commonly used **Pandas functions and methods** for data manipulation and analysis. Pandas is a powerful Python library for data handling, offering tools for reading, processing, analyzing, and visualizing structured data.

---

## Table of Contents
- [Data Creation](#data-creation)
- [Data Inspection](#data-inspection)
- [Data Selection and Filtering](#data-selection-and-filtering)
- [Data Cleaning](#data-cleaning)
- [Data Transformation](#data-transformation)
- [Aggregation and Statistics](#aggregation-and-statistics)
- [Group Operations](#group-operations)
- [Merging and Joining](#merging-and-joining)
- [Visualization](#visualization)
- [Date and Time Handling](#date-and-time-handling)
- [File Export](#file-export)

---

## Data Creation
```python
import pandas as pd
pd.Series()
pd.DataFrame()
pd.read_csv('file.csv')
pd.read_excel('file.xlsx')
pd.read_json('file.json')
pd.read_sql(query, connection)
pd.read_html('url_or_html')
pd.DataFrame.from_dict(dictionary)
```

---

## Data Inspection
```python
df.head(n)
df.tail(n)
df.info()
df.describe()
df.shape
df.columns
df.dtypes
df.index
```

---

## Data Selection and Filtering
```python
df.loc[row_label, col_label]
df.iloc[row_position, col_position]
df.at[row_label, col_label]
df.iat[row_position, col_position]
df.query('column > value')
df[df['column'].isin([value1, value2])]
```

---

## Data Cleaning
```python
df.dropna()
df.fillna(value)
df.replace(old_value, new_value)
df.drop(columns=['column_name'])
df.duplicated()
df.drop_duplicates()
```

---

## Data Transformation
```python
df.apply(function)
df['column'].map(function)
df.astype('data_type')
df.rename(columns={'old': 'new'})
df.sort_values(by='column')
df.sort_index()
```

---

## Aggregation and Statistics
```python
df.mean()
df.median()
df.sum()
df.count()
df.min(), df.max()
df.std()
df.corr()
df['column'].value_counts()
```

---

## Group Operations
```python
df.groupby('column').mean()
df.agg(['sum', 'mean'])
pd.pivot_table(df, values='column', index='index_column', columns='column2')
pd.crosstab(df['column1'], df['column2'])
```

---

## Merging and Joining
```python
pd.concat([df1, df2])
pd.merge(df1, df2, on='key')
df1.join(df2, on='key')
df1.append(df2, ignore_index=True)
```

---

## Visualization
```python
df.plot()
df.hist()
df.boxplot()
```

---

## Date and Time Handling
```python
df['date_column'] = pd.to_datetime(df['date_column'])
df['date_column'].dt.year, df['date_column'].dt.month
df.resample('M').sum()
```

---

## File Export
```python
df.to_csv('output.csv')
df.to_excel('output.xlsx')
df.to_json('output.json')
df.to_sql('table_name', connection, if_exists='replace')
```

---

## Contribution
If you find this guide helpful, feel free to contribute by adding more functions or improving descriptions. Fork this repository, make changes, and submit a pull request. 😊

---

## License
This project is licensed under the MIT License.

---

## Conclusion
This guide provides a quick reference for essential Pandas functions and methods. Mastering these will help streamline your data analysis workflows. Happy coding! 🚀


