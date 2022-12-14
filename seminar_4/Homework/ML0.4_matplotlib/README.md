### 0.3. Визуализация данных с использованием библиотек matplotlib и seaborn  

Автор - Одинцова В.А.

#### Цель работы

Научиться строить некоторые виды графиков, используемые в анализе данных, при помощи библиотек matplotlib и seaborn.  

#### Задания для выполнения:

0. Загрузите датасет для предсказани цены квартиры в зависимости от ряда признаков.
1. Постройте круговую диаграмму для признака `Rooms`, иллюстрирующую количество квартир в процентах в зависимости от количества комнат. Сделайте сектор с наибольшим числом квартир выдвинутым.
2. Постройте гистограмму целевой переменной `Price`. Оцените визуально, по какой цене продаётся наибольшее количество квартир. 
3. Постройте диаграммы рассеяния для признаков `Rooms`, `Square`, `HouseFloor`, `HouseYear` в зависимости от целевой переменной `Price` в одной области fiagure(). Оцените визуально, есть ли среди них такие, на которых разброс точек близок к линейной функции.
4. Постройте ядерную оценку плотности целевой переменной `Price`. Оцените визуально, напоминает ли полученный график нормальное распределение. Постройте двумерную ядерную оценку плотности для целевой переменной `Price` и признака `HouseFloor`, затем оцените визуально на каких этажах и по какой цене продаётся основная масса квартир.
5. Постройте ящиковую диаграмму признака `Square`. Оцените визуально имеются ли выбросы, и, если да, то начиная с какого размера площади значение признака можно считать выбросом.
6. При помощи сетки графиков `PairGrid` визуализируйте попарные отношения признаков `Rooms`, `Square`, `HouseFloor`, `HouseYear`, `Price` следующим образом: на диагонали - гистограммы, под диагональю - ядерные оценки плотности, над диагональю - диаграммы рассеяния. По результатам визуализации сделайте выводы (аналогичные п.2,3,4).
7. Постройте тепловую карту матрицы корреляции (`df.corr()`) признаков `Rooms`, `Square`, `HouseFloor`, `HouseYear`, `Price`. По ней определите, какие признаки являются зависимыми (у таких признаков коэффициент корреляции близок к единице).

Должны быть подписаны названия графиков, названия осей, указаны значения на осях. Оцениваться будет использование 
количества различных атрибутов при построении графиков и визуальная красота.

#### Методические указания

Ознакомьтесь с официальной документацией по библиотекам matplotlib и seaborn.

#### Дополнительные задания:

1. Постройте график jointplot (гибрид scatterplot и histogram) из библиотеки seaborn. 
2. Постройте график violinplot (гибрид boxplot и ядерной оценки плотности) из библиотеки seaborn. 
3. Поработайте с сеткой подзаголовков FacetGrid.

#### Контрольные вопросы:

1. Построение каких основных видов графиков используется при анализе данных в машинном обучении?
2. В чём разница между библиотеками matplotlib и seaborn. Преимущества каждой из них.
3. Как задать размер графика в matplotlib?
4. Как установить стили в seaborn?
5. Для чего используют подграфики subplots?
6. Что изображается на ящиковой диаграмме?
7. Как поменять палитру цветов у тепловой карты.
