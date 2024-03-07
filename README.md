# Предварительная обработка данных спектра почвы

> Предварительная подготовка данных спектра для дальнейшего обучения ML.

---

## Описание проекта

Этот проект включает в себя предварительную обработку данных спектра почвы, собранных в видимом и ближнем инфракрасном диапазоне. В процессе предварительной обработки были использованы следующие методы:

- Фильтрация Савицкого-Голея с производной первого порядка
- Дискретное вейвлет-преобразование
- Нормализация данных
- Стандартизация данных

![Output](https://github.com/novoselov-ie/Spectr_data_preparation/blob/main/Интенсивность_спектра.png)

## Использование фильтрации Савицкого-Голея
Фильтрация Савицкого-Голея является широко используемым методом сглаживания и выравнивания спектральных данных. В данном проекте мы использовали этот метод с производной первого порядка для сглаживания и выделения основных характеристик спектра почвы.

![Output](https://github.com/novoselov-ie/Spectr_data_preparation/blob/main/swg.png)
## Дискретное вейвлет-преобразование
Дискретное вейвлет-преобразование (DWT) является мощным методом анализа сигналов, который позволяет разложить сигнал на различные уровни детализации и аппроксимации. Мы использовали DWT для извлечения скрытых структур и особенностей из спектральных данных почвы.

![Output](https://github.com/novoselov-ie/Spectr_data_preparation/blob/main/dwt.png)

## Нормализация данных
Нормализация данных является процессом приведения данных к диапазону от 0 до 1. Этот процесс позволяет стабилизировать обучение модели и ускорить сходимость алгоритмов машинного обучения.


## Cтек
<b> Предварительная обработка данных: </b>
- pandas
- matplotlib
- scipy
- numpy
- pywt
- os

<b> Нормализация и стандартизация:  </b>
- sklearn.preprocessing

