Загрузка данных в базу данных



1. Вариант 1: добавить пустой столбец в файл (что-бы у полей в файле и полей в БД был идентичный порядок)

2. Вариант 2: грузить из dataframe а не из файла

https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_sql.html
```python
df = ... загрузить данные в df...
df.to_sql("sessions", if_exists="replace")
```
