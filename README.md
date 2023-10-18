# Общая информация

Репозиторий содержит данные dataset.csv и 4 notebook-а с решениеями

* 1_EDA.ipynb - содержит анализ данных по dataset
* 2_baseline.ipynb - бейзлайн решение с помощью линейной регрессии с l1 регуляризацией
* 3_Boosting.ipynb - решение с помощью градиентного бустинга
* 4_Alternative_solution.ipynb - показано 2 решение 2-х задач: 
    1) Решение задачи классификации. Кодируем target 0 и 1, где 0 -  клиент ничего не потратит, 1 - клиент потратит какую-то сумму
    2) Как только определили людей которые потратят какую-то сумму денег. Решаем задачу регресси и предсказываем сумму

# Выводы

1) Ошибки в моделях представленных в 2_baseline и 3_Boosting меньше чем 4_Alternative_solution. Происходит Это за счет того что в 2_baseline и 3_Boosting в наблюдениях много целевых значений равныз 0.0 (97% наблюдений).
2) Огромный разброс целевого события. Разброс может объяснятся тем что действительно есть клиенты которые много тратят или это из-за валюты в которой тратятся деньги не нормированны.
3) Лучшие результаты дала модель 3_Boosting.