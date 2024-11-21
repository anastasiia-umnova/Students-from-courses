# Ученики с годовых курсов ЕГЭ

# Описание проекта
Проект направлен на анализ данных образовательной IT-платформы подготовки к экзаменам в РФ. В ходе выполнения работы из базы данных с использованием SQL-запроса выбрана информация по ученикам с годовых курсов ЕГЭ. Проведена предобработка датасета и проверка на аномалии. Выполнено деление учеников на группы в зависимости от того, когда ученики присоединились к курсу. Выявлены наиболее популярные предметы и города с наибольшим количеством учащихся.

# Входные данные

В качестве входных данных - база данных по ученикам, включающая 11 таблиц (https://disk.yandex.ru/d/W6t4WFTWmqNE2g). 
Схема базы данных – db_schema.jpg (https://disk.yandex.ru/i/KD76DFv8gEkVQQ).


# Анализ данных
* С использованием SQL-запроса выгружена из базы данных информация по ученикам с годовых курсов. Поля в итоговой выгрузке содержат: ID курса, Название курса, Предмет, Тип предмета, Тип курса, Дата старта курса, ID ученика, Фамилия ученика, Город ученика, Ученик не отчислен с курса, Дата открытия курса ученику, Сколько полных месяцев курса открыто у ученика, Число сданных ДЗ ученика на курсе
* Исследование датафрейма на пропуски, типы данных и аномалии.
* Поиск наиболее распространенных предметов и анализ географии расределения учеников образовательной IT-платформы подготовки к экзаменам в РФ.
* Группировка ученников в зависимости от времени присоединения к курсу (присоединились к курсу до его начала, в течение 1 недели после даты старта курса включительно, от 1 до 2 недель включительно, от 2 до 3 недель включительно, от 3 до 4 недель включительно, от 4 недель после даты старта курса).
* 
#  Выводы
В проекте проведена работа с базой данных, проанализированы характеристики и поведения учеников. Выявлены приорететные предметы у учеников (обществознание, русский язык и математика). Вероятно, стоит сделать акцент на преподавателях по этим предметам. Показано, что ученики чаще всего приоединяются к курcy до его начала. Наибольшее количество учеников проживает в таких городах как Москва, Санкт-Петербург, Краснодар, Казань и Новосибирск. Скорее всего распределение учеников по городам коррелирует с размером города. Большинство учеников выбирают по 1 предмету, 13 учеников выбрало наибольшее количество предметов (5), следовательно необходимо проихвести работу над увеличением спроса.

# Библиотеки и технологии
SQL, pandas, numpy, seaborn, matplotlib.

