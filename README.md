[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
# Housing in Mexico

## Description
In this project, I'll work with a dataset with 21,000 properties for sale in Mexico to determine whether sale prices are influenced more by property size or location.


**Table of contents**
- [About the Project](#about-the-project)
- [Language](#language)
- [Library](#library)
- [Getting started](#getting-started)
- [Rum Project](#rum-project)
- [References](#references)
- [Author](#author)

## Language
- Python  3.9.12
- SQL

## Library
- Faker   18.7.0
- Pandas  2.0.1
- Sqlite  

## Getting started
- [Import the library](#import-the-library)
- [Building the database](#building-the-database)
- [Create the tables](#create-the-tables)
- [Normalize the database](#normalize-the-database)
- [Check the database](#check-the-database)

### Import the library
```python
from faker import Faker
import pandas as pd
import sqlite3

# create a instance of the faker class and set a seed to have the same behaviour
fake = Faker()
fake.seed_instance(121)
```
### Building the database
```python
# set a cursor to the database
# whether the database doesn't exist sqlite create it.
conn = sqlite3.connect('db_test.db')
cursor = conn.cursor()
``` 

## Rum Project
```bash
# Clone the reposotiry 
git clone https://github.com/IgorTraspadini/Sintectical_SQL_database.git

# Import
requirements.txt

# Run the project
python sintectical_db.py
```

## References 
- [Faker Documentation](https://faker.readthedocs.io/en/master/)
- [Database normalization](https://en.wikipedia.org/wiki/Database_normalization)

## Author
[Igor Traspadini](https://www.linkedin.com/in/igor-chieppe-traspadini/?locale=en_US)

## License
- This application is covered under: 
[MIT License](https://choosealicense.com/licenses/mit)
