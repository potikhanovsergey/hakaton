# Краткое описание хакатона
Задача вкраце: нам дана карта в виде двумерного массива, по которой ходит игровой персонаж и набирает очки, за то, что он собирает некоторые целевые поля.
На карте есть несоклько типов полей, которые изменяют передвижение.
Передвижение происходит по определенным правилам, похожим на вектор скорости.
Перед началом движения можено потретить очки действия на изменение полей карты.
Всего у нас есть 3600 очков действия, которые мы тратим на передвижение (один ход = одно очко) и на изменения полей карты (улучшение одного поля = одно очко).
Цель - набрать максимальное количество очков по формуле
Score = 3600 * 1.1^p / (t + j), где:
p - количество успешно доставленных подарков (P > 0)
t - время (количество шагов), затраченное на выполнение задания (20 <= t <= 3600)
j - количество улучшенных клеток карты (0 <= j;  t + j <= 3600)

Решение - JSON файл с набором векторов, по которым ходил персонаж и набором выбранных улучшений

###ссылка на хакатон
https://cups.online/ru/contests/vkwinterquest
###телеграм канал
https://t.me/allcupsjunior

## Участники

| Учебная группа | Имя пользователя  | ФИО                      |
|----------------|-------------------|--------------------------|
| 201-327        | @GrabovyiS        | Грабовый С.П.            |
| 201-327        | @halaponga2       | Лобов И.К.               |
| 201-327        | @potikhanovsergey | Потиханов С.В.           |
| 201-327        | @vancode111       | Елисеев И.П.             |
| 201-327        | @LevFenev         | Фенев Л.Е.               |

## Личный вклад участников

### Грабовый С. П.  
Логика работы приложения 6ч  
Тестировка приложения 6ч  
Поиск оптимального маршрута игры 6ч+  
Совершенствование маршрута 6ч  
Дополнительный функционал с отправкой решений на почту (не попал в прод) 2ч  
Понимание правил игры и объяснение сути разработчикам 6ч  
Формулировка идей для дополнительного функционала 2ч  
Коммуникация с администраторами по поводу правил 2ч

### Лобов И.К.

### Потиханов С.В.
Логика работы игры 6ч  
Логика работы дополнительного функционала 6ч  
Вёрстка 6ч  


### Елисеев И.П.

### Фенев Л.Е.
