# Проект. Экспресс-угадывание числа путем бинарного поиска

## Оглавление  
[1. Описание проекта](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readmeОписание-проекта)  
[2. Цель проекта](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readmes#Цель-проекта)  
[3. Краткая информация о данных](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Краткая-информация-о-данных)  
[4. Задачи-этапы проекта](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Задачи-этапы-проекта)  
[5. Результаты](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Результаты)    
[6. Выводы](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Выводы) 

### Описание проекта    
Система загадывает произвольное целое число (integer), которое нужно угадать пользователю за фиксированное число попыток.

:arrow_up:[к оглавлению](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Оглавление)


### Цель проекта    
Требуется составить эффективный алгоритм, позволяющий определить зашифрованное компьютером число.

**Основные требования к разрабатываемой программе:**  
- Компьютер загадывает целое число от 0 до 100, и пользователю его нужно угадать. Под «угадать», подразумевается «написать программу, которая угадывает число».
- Алгоритм учитывает информацию о том, больше ли случайное число или меньше нужного нам.

**Оценка качества программы по угадыванию числа**     
Результаты работы алгоритма оцениваются по среднему количеству попыток при 1000 повторений.

**Формируемые скиллы**     
1. Написание рабочего кода на языке Python
2. Оформление кода в соответствии с стандарту PEP8.


### Краткая информация о данных
Целочисленные переменные генерируются произвольно. Фиксируется random.seed(20) для работы программы на угадывание числа, что повысит воспроизводимость написанного кода.
  
:arrow_up:[к оглавлению](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Оглавление)


### Задачи-этапы проекта  
1. Оптимизировать код программы по угадыванию случайного числа, зашифрованного системой
2. Сравнить эффективность работы разработанного алгоритма с имеющимися подходами по таргетной задаче.
3. Зафиксировать версии библиотек, необходимых для реализации оформленного кода в Python.

:arrow_up:[к оглавлению](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Оглавление)


### Результаты
Новый подход к составлению программы по угадыванию заданного системой целого числа основан на бинарном поиске. То есть принимаются верхняя и нижняя границы для генерации числа компьютером. В зависимости от введенного пользователем числа происходит переопределение этих границ, чтобы сократить интервал для загаданного числа.
Оценка трех программ проводилась с использованием функции score_game(). Данная функция возвращает среднее число попыток, затрачиваемых для угадывания числа (на 1000 проб).
Сводные данные по эффективности алгоритмов (алгоритм - среднее число попыток, необходимых для обнаружения загаданного числа):
1. Алгоритм_1 ("Случайное угадывание"): 99 попыток
2. Алгоритм_2 ("Угадывание с коррекцией"): 33 попытки
3. Алгоритм_3 ("Экспресс-угадывание числа путем бинарного поиска"): 5 попыток.
:arrow_up:[к оглавлению](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Оглавление)


### Выводы
1. Разработан алгоритм для обнаружения заданного компьтером целого числа с применением бинарного поиска. Это резко сокращает время работы алгоритма для выполнения конкретной задачи.
2. Наиболее эффективным является подход бинарного поиска в выявлении rand-числа, что показали результаты метрики алгоритмов с использованием функции score_game().

:arrow_up:[к оглавлению](https://github.com/Edgars97/Projects/tree/https/github.com/Edgars97/Projects#readme#Оглавление)


Если информация по этому проекту покажется вам интересной или полезной, то я буду очень вам благодарен, если отметите репозиторий и профиль ⭐️⭐️⭐️-дами