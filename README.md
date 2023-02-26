# Домашнее задание к занятию 12.1. «Базы данных»

* [Ответ к Заданию 1](#1)
* [Ответ к Заданию 2* - отсутствует](#2)


---
### Легенда

Заказчик передал вам [файл в формате Excel](https://github.com/netology-code/sdb-homeworks/blob/main/resources/hw-12-1.xlsx), в котором сформирован отчёт. 

На основе этого отчёта нужно выполнить следующие задания.

### Задание 1

Опишите не менее семи таблиц, из которых состоит база данных:

- какие данные хранятся в этих таблицах;
- какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL.

Приведите решение к следующему виду:

Сотрудники (

- идентификатор, первичный ключ, serial,
- фамилия varchar(50),
- ...
- идентификатор структурного подразделения, внешний ключ, integer).


### *<a name = "1"> Ответ к Заданию 1 </a>*

**1. Сотрудники (**
- Идентификатор сотрудника, первичный ключ, serial,
- Фамилия, varchar(20),
- Имя, varchar(20),
- Отчество, varchar(20),
- Оклад NUMERIC(10,2),
- идентификатор должности,  внешний ключ, integer,
- идентификатор структурного подразделения, внешний ключ, integer),
- Дата найма, DATE,
- идентификатор филиала, внешний ключ, integer,
- идентификатор проекта, integer

**)**

**2. Должности (**
- Идентификатор должности, первичный ключ, integer,
- Название должности, varchar(50),

**)**

**3. Структурное подразделение (**
- Идентификатор структурного подразделения, первичный ключ, integer,
- Наименование структурного подразделения, varchar(50),
- идентификатор типа структурного подразделения, внешний ключ, integer

**)**

**4. Тип структурного подразделения (**
- Идентификатор типа структурного подразделения, первичный ключ, integer,
- Наименование типа структурного подразделения, varchar(50)

**)**

**5. Филиалы (**
- Идентификатор филиала, первичный ключ, integer,
- идентификатор региона филиала, внешний ключ, integer,
- Адрес филиала внутри региона, varchar(100)

**)**

**6. Регион филиала (**
- Идентификатор региона филиала, натуральный первичный ключ, integer,
- Наименование региона филиала, varchar(100)

**)**

**7. Проекты (**
- Идентификатор проекта, первичный ключ, integer,
- Наименование проекта, varchar(100)

**)**


---

## Дополнительные задания (со звёздочкой*)
Эти задания дополнительные, то есть не обязательные к выполнению, и никак не повлияют на получение вами зачёта по этому домашнему заданию. Вы можете их выполнить, если хотите глубже шире разобраться в материале

### Задание 2*

Перечислите, какие, на ваш взгляд, в этой денормализованной таблице встречаются функциональные зависимости и какие правила вывода нужно применить, чтобы нормализовать данные.

### *<a name = "2"> Ответ к Заданию 2 - отсутствует </a>*
