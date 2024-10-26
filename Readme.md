# <center> Проект: анализ резюме из HeadHunter </center>
## Оглавление
1. [Описание проекта](#описание-проекта) 
2. [Описание данных](#описание-данных)
3. [Структура проекта](#структура-проекта)
3. [Исследование структуры данных](#исследование-структуры-данных)
4. [Преобразование данных](#преобразование-данных)               
5. [Исследование зависимостей в данных](#исследование-зависимостей-в-данных)
6. [Очистка данных](#очистка-данных)
7. [Использование](#использование)
8. [Авторы](#авторы)

## Описание проекта

В данном проекте проводится анализ резюме из HeadHunter.

Анализ данных проводится для того, чтобы сделать выводы о соискателях: выявить зависимости, в особенности, анализ желаемой заработной платы, которую соискатель указывает либо данные соискателя о желаемой заработной платы могут отсутствовать.

Проект реализован в PYTHON 3.12.3, используя библиотеки Pandas, Numpy, Matplotlib, Seaborn, Plotly.express.

### Цель данного проекта:
Анализ данных компании HeadHunter, которая хочет построить модель, которая бы автоматически определяла примерный уровень заработной платы, подходящей пользователю, исходя из информации, которую он указал о себе.

### Задачи данного проекта:
* базовый анализ структуры данных;
* преобразование данных;
* разведывательный анализ;
* очистка данных

## Структура проекта

* [data](https://disk.yandex.ru/d/qzdxw9p3aM2eLw) - папка с исходными табличными данными
* [images](./imanges/) - папка с изображениями, необходимыми для проекта
* [Project-1._Ноутбук-шаблон.ipynb](./Project-1._Ноутбук-шаблон.ipynb) - jupyter-ноутбук, содержащий основной код проекта

## Описание данных

В этом проекте используется база резюме, выгруженная с сайта поиска вакансий hh.ru. 
База включается в себя 44744 резюме по 12 признакам.
Файл с данными можно найти [здесь](https://disk.yandex.ru/d/qzdxw9p3aM2eLw).
А также выгрузка курсов валют с ресурса  [MFD.RU](https://mfd.ru/export/#Alias=false&Period=1&timeframeValue=1&timeframeDatePart=day&StartDate=04.10.2021&EndDate=04.10.2021&SaveFormat=0&SaveMode=0&FieldSeparator=%253b&DecimalSeparator=.&DateFormat=yyyyMMdd&TimeFormat=HHmmss&AddHeader=true&RecordFormat=0&Fill=false), которые встречаются в наших данных за период с 29.12.2017 по 05.12.2019. Файл с данными можно найти [здесь](https://disk.yandex.ru/d/qzdxw9p3aM2eLw)

## Исследование структуры данных
В данном разделе проведено исследование структуры данных: 
* прочитены данные с помощью библиотеки Pandas, чтобы ознакомиться с признаками и их структурой;
* выведена основная информация о числе непустых значений в столбцах и их типах в таблице;
* выведена основная статистическая информация о столбцах.

## Преобразование данных
В данном разделе проведена предобработка данных, чтобы представить признаки в "удобном" для анализа и очистки формате, а также визуальной оценки зависимости в данных. Для этого были реализованы функции-преобразования и созданы новые признаки. 

## Исследование зависимостей в данных
В данном разделе проведен разведывательный анализ (EDA), который предназначен для выявления связей между признаками, выявления закономерностей, определения распределений признаков, поиска аномалий и других дефектов данных. 

Зависимости представленны на графиках: гистограммы и коробчатые диаграммы, столбчатые и многоугорвненые диаграммы, диаграммы рассеяния, тепловые карты и реализованы постредством быблиотеки Plotly.express.

## Очистка данных
В ходе визуального анализа, было найдено несколько несостыковок в данных, что стало необходимостью поработать над очистокой данных: поиск дубликатов, пропусков, ликвидации выбросов.
Был произведен анализ и ликвидация выбросов посредством графика распределения признака в **логарифмическом масштабе** и поиск выбросов с помощью **метода z-отклонения**.

## Использование
Проект представлен в jupyter-ноутбуке
Project-1._Ноутбук-шаблон.ipynb.

## Авторы

* [Igor_M](ya.m67@yandex.ru.ru)

