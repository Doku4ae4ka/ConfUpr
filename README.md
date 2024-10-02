# Практическое занятие №1. Введение, основы работы в командной строке

П.Н. Советов, РТУ МИРЭА

Научиться выполнять простые действия с файлами и каталогами в Linux из командной строки. Сравнить работу в командной строке Windows и Linux.

## Задача 1

grep '.*' /etc/passwd | cut -d: -f1 | sort

<img width="638" alt="Снимок экрана 2024-10-02 в 14 40 29" src="https://github.com/user-attachments/assets/d47996f7-ea6e-4895-8999-625605164720">


## Задача 2

awk '{print $2, $1}' /etc/protocols | sort -nr | head -n 5

<img width="669" alt="Снимок экрана 2024-10-02 в 14 41 15" src="https://github.com/user-attachments/assets/a7d627de-5d47-45d7-a593-6074e96ba9ee">


## Задача 3

#!/bin/bash

text=$*
length=${#text}

for i in $(seq 1 $((length + 2))); do
    line+="-"
done

echo "+${line}+"
echo "| ${text} |"
echo "+${line}+"

<img width="707" alt="Снимок экрана 2024-10-02 в 14 51 53" src="https://github.com/user-attachments/assets/ce80af5a-f99e-410c-bf1a-f698a9f228a6">

<img width="716" alt="Снимок экрана 2024-10-02 в 15 01 56" src="https://github.com/user-attachments/assets/7441383e-0cb9-4887-aadd-a49d5cd2c7f6">

<img width="394" alt="Снимок экрана 2024-10-02 в 14 53 34" src="https://github.com/user-attachments/assets/17b73234-8ccd-4fa3-bf41-335b3780d40f">


## Задача 4

Написать программу для вывода всех идентификаторов (по правилам C/C++ или Java) в файле (без повторений).

Пример для hello.c:

```
h hello include int main n printf return stdio void world
```

## Задача 5

Написать программу для регистрации пользовательской команды (правильные права доступа и копирование в /usr/local/bin).

Например, пусть программа называется reg:

```
./reg banner
```

В результате для banner задаются правильные права доступа и сам banner копируется в /usr/local/bin.

## Задача 6

Написать программу для проверки наличия комментария в первой строке файлов с расширением c, js и py.

## Задача 7

Написать программу для нахождения файлов-дубликатов (имеющих 1 или более копий содержимого) по заданному пути (и подкаталогам).

## Задача 8

Написать программу, которая находит все файлы в данном каталоге с расширением, указанным в качестве аргумента и архивирует все эти файлы в архив tar.

## Задача 9

Написать программу, которая заменяет в файле последовательности из 4 пробелов на символ табуляции. Входной и выходной файлы задаются аргументами.

## Задача 10

Написать программу, которая выводит названия всех пустых текстовых файлов в указанной директории. Директория передается в программу параметром. 

## Полезные ссылки

Линукс в браузере: https://bellard.org/jslinux/

ShellCheck: https://www.shellcheck.net/

Разработка CLI-приложений

Общие сведения

https://ru.wikipedia.org/wiki/Интерфейс_командной_строки
https://nullprogram.com/blog/2020/08/01/
https://habr.com/ru/post/150950/

Стандарты

https://www.gnu.org/prep/standards/standards.html#Command_002dLine-Interfaces
https://www.gnu.org/software/libc/manual/html_node/Argument-Syntax.html
https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap12.html

Реализация разбора опций

Питон

https://docs.python.org/3/library/argparse.html#module-argparse
https://click.palletsprojects.com/en/7.x/
