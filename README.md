# Модуль фитнес-трекера

Программный модуль фитнес-трекера, который обрабатывает данные для трех видов тренировок: для бега, спортивной ходьбы и плавания.

### Этот модуль:
 - принимает от блока датчиков информацию о прошедшей тренировке,
 - определяет вид тренировки,
 - рассчитывает результаты тренировки,
 - выводит информационное сообщение о результатах тренировки.

### Информационное сообщение включает такую информацию как:
 - тип тренировки (бег, ходьба или плавание);
 - длительность тренировки
- дистанция, которую преодолел пользователь, в километрах;
- среднюю скорость на дистанции, в км/ч;
- расход энергии, в килокалориях.

### Структура программы
#### Каждый вид спортивной активности в модуле описан соответствующим классом:

Бег → class Running ;
Спортивная ходьба → class SportsWalking ;
Плавание → class Swimming .

#### Конструктор каждого из классов получает информацию с датчиков:
- action, тип int — количество совершённых действий (число шагов при ходьбе и беге либо гребков — при плавании);
- duration, тип float — длительность тренировки;
- weight, тип float — вес спортсмена.

#### Методы классов, которые отвечают за обработку данных:
- расчёт дистанции, которую пользователь преодолел за тренировку get_distance()
- расчёт средней скорости движения во время тренировки: get_mean_speed();
- расчёт количества потраченных калорий за тренировку: get_spent_calories();
- создание объекта сообщения о результатах тренировки: show_training_info().
