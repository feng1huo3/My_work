                                                                                         "То, чего я не могу создать, я не понимаю".
                                                                                                                    Ричард Фейнман
Суть прогнозирования заключается в симуляции представительного элемента объема композита, на основе данных о характеристиках входящих компонентов (связующего и армирующего компонента).

Задачи:
1)	по имеющимся данным построить модель, прогнозирующую модуль упругости композита при растяжении;
2)	построить модель, прогнозирующую прочность композита при растяжении;
3)	написать нейронную сеть, которая будет рекомендовать соотношение “матрица-наполнитель”.

Датасет характеризуется 1023 наблюдениями и 13 признаками.

Этапы разведочного анализа:
●	изучение распределения переменных и признаков и логарифмирование в случае необходимости;

●	обнаружение и удаление аномалий;

●	описательная статистика (используем ProfileReport из библиотеки Pandas);

●	поиск корреляций между признаками (при сильной корреляции можно объединить неважные);

●	важность признаков с помощью f-regression из библиотеки sklearn;

●	построение графиков для поиска парных особенностей и поиск инсайтов.


Методы: Lasso, Ridge-регрессии, квантильная регрессия, попытка SVR; нейронная сеть (функция активации - RELU).

Результаты неадекватные, но было очень много вопросов к исходным данным.
