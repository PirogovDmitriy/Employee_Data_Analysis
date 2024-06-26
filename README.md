# Анализ данных о сотрудниках и прогнозирование увольнений

## Обзор

Этот проект посвящен анализу данных о сотрудниках компании и построению прогнозной модели для определения вероятности увольнения сотрудников на основе различных факторов. Цель проекта — использовать методы анализа данных и машинного обучения для предсказания увольнений, что позволит компании лучше понимать причины текучести кадров и принимать меры для её снижения.

## Введение

В современных условиях конкурентного бизнеса понимание динамики сотрудников и причин их увольнения имеет решающее значение для успеха любой организации. Цель этого проекта — использовать методы науки о данных для анализа данных о сотрудниках и построения модели, которая предсказывает, уволится ли сотрудник, на основе различных факторов.

## Данные HR

Набор данных, использованный в этом проекте, содержит следующие атрибуты, связанные с сотрудниками:
 - `satisfaction_level` - Уровень удовлетворенности работой
 - `Last_evaluation` - Время с момента последней оценки в годах
 - `number_projects` - Количество проектов, выполненных за время работы
 - `average_monthly_hours` - Среднее количество часов на рабочем месте в месяц
 - `time_spend_company` - Стаж работы в компании в годах
 - `work_accident` - Происходили ли несчастные случаи на рабочем месте с сотрудником
 - `left` - уволился ли сотрудник
 - `promotion_last_5years` - повышался ли сотрудник за последние пять лет
 - `department` - отдел в котором работает сотрудник
 - `salary` - относительный уровень зарплаты

## Цели

1. Загрузите файл HR.csv в pandas dataframe
2. Рассчитайте основные статистики для переменных (среднее, медиана, мода, мин/макс, сред.отклонение)
3. Рассчитайте и визуализируйте корреляционную матрицу для количественных переменных. Определите две самые скоррелированные и две наименее скоррелированные переменные.
4. Рассчитайте, сколько сотрудников работает в каждом департаменте
5. Показать распределение сотрудников по зарплатам
6. Показать распределение сотрудников по зарплатам в каждом департаменте по отдельности
7. Проверить гипотезу, что сотрудники с высоким окладом проводят на работе больше времени, чем сотрудники с низким окладом
8. Рассчитать следующие показатели среди уволившихся и не уволившихся сотрудников (по отдельности): Доля сотрудников с повышением за последние 5 лет, Средняя степень удовлетворенности, Среднее количество проектов
9. Разделить данные на тестовую и обучающую выборки. Построить модель LDA, предсказывающую, уволился ли сотрудник на основе имеющихся факторов (кроме department и salary). Оценить качество модели на тестовой выборке

## Методы

Проект включает следующие ключевые этапы:
1. **Очистка и предобработка данных**: Обработка пропущенных значений, кодирование категориальных переменных, масштабирование числовых признаков.
2. **Разведочный анализ данных (EDA)**: Выявление закономерностей и взаимосвязей в данных с помощью визуализаций и статистических методов.
3. **Построение моделей**: Реализация модели машинного обучения [LDA](https://scikit-learn.org/stable/modules/lda_qda.html) для предсказания увольнений сотрудников.
4. **Оценка моделей**: Оценка производительности моделей с использованием метрик, таких как точность и AUC-ROC.

![ROC](https://imgur.com/S7M6SDW.png)

## Результаты

Проект дал несколько ключевых инсайтов и прогнозов, включая:
- Распределение зарплат по разным департаментам

![Распределение зарплат](https://imgur.com/vwCflQy.png)

- Основные признаки, влияющие на вероятность увольнения сотрудников.
- Визуализации, демонстрирующие важность различных факторов для предсказания увольнений.

![Важность признаков](https://imgur.com/WZdHkcL.png)

## Стек

![Python](https://img.shields.io/badge/-Python-333?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/-Pandas-333?style=flat&logo=pandas)
![Numpy](https://img.shields.io/badge/-Numpy-333?style=flat&logo=numpy)
![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-333?style=flat&logo=scikit-learn)
![Scipy](https://img.shields.io/badge/-Scipy-333?style=flat&logo=Scipy)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-333?style=flat&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/-Seaborn-333?style=flat&logo=Seaborn)
