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

<img width="766" alt="Снимок экрана 2024-10-02 в 15 04 18" src="https://github.com/user-attachments/assets/be960278-a408-453d-ac64-a20ffd33f380">

## Задача 5

<img width="546" alt="Снимок экрана 2024-10-02 в 15 07 42" src="https://github.com/user-attachments/assets/0547f974-7dbb-4fb5-ad97-ccbf3169ce9e">

<img width="308" alt="Снимок экрана 2024-10-02 в 15 07 48" src="https://github.com/user-attachments/assets/b70bc71d-831c-4c76-80e7-b6413054e500">


