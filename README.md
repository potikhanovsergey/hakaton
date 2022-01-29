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

###ссылка на решение
https://mospolytech-course-work-vk-cup.netlify.app

## Участники

| Учебная группа | Имя пользователя  | ФИО                      | Роль                     |
|----------------|-------------------|--------------------------|--------------------------|
| 201-327        | @halaponga2       | Лобов И.К.               | Тимлид                   |
| 201-327        | @GrabovyiS        | Грабовый С.П.            | Тестировщик, разработчик |
| 201-327        | @potikhanovsergey | Потиханов С.В.           | Разработчик              |
| 201-327        | @vancode111       | Елисеев И.П.             | Разработчик              |
| 201-327        | @LevFenev         | Фенев Л.Е.               | Дизайрен, тестировщик    |

## Личный вклад участников

### Лобов И.К.
Организация коммуникации в команде, своевременный сбор всех людей в Discord - 3ч  
Формулировка идей для дополнительного функционала (Совместно с Фенев Л.Е.) (Кнопки UNDO, REDO, Порталы, воспроизведение шагов по введенной JSON строке) 6ч  
Поиск оптимального маршрута игры 6ч+  
Тестировка приложения (Поиск визуальных и функциональных багов, запросы на исправление разработчикам) 6ч  
Совершенствование маршрута, поиск лучших ходов в конкретной части карты 6ч  
Понимание правил игры и объяснение сути разработчикам (Потиханов С.В. и Елисеев И.П.) 6ч  
Написание документации к проекту - 3ч  

### Грабовый С. П.  
Логика работы приложения 6ч  
Тестировка приложения (Поиск визуальных и функциональных багов, запросы на исправление разработчикам) 6ч  
Поиск оптимального маршрута игры 6ч+  
Совершенствование маршрута, поиск лучших ходов в конкретной части карты 6ч  
Понимание правил игры и объяснение сути разработчикам (Потиханов С.В. и Елисеев И.П.) 6ч  
Коммуникация с администраторами по поводу правил 2ч  
Дополнительный функционал с отправкой решений на почту (не попал в прод) 3ч  
Написание документации к проекту - 3ч  

### Потиханов С.В.
Создание и введение ГИТ репозитория, проверка и прием merge-request-ов - 3ч <br>
Визуализация исходного массива карты (Совместно с Фенев Л.Е.) (Поле 100х100), каждая клетка - отдельная кнопка - 3ч  
Создание логики ходов Санты в JavaScript (Сохранение вектора, создание возможных полей для хода исходя из текущего вектора скорости) (совместно с Грабовый С.П., Лобов И.К.) - 3ч  
Сохрание ходов игрока в JSON формате пригодного для сдачи (записываются шаги и улучшения) - 6ч  
Создание панели управления (Записывается вся статистика об игре, есть функциональные поля телепорта, ввода JSON и сохранения решения) - 6ч  
Фиксы визуальных багов от тестировщиков (Грабовый С.П., Лобов И.К., Фенев Л.Е.) - 6ч  
Разработка функционала "Улучшение поля" (На панели управления есть два инпута с плэйсхолдерами "X" и "Y", куда вписываются координаты клетки для улучшения) - 6ч  
Написание документации к проекту - 3ч  

### Елисеев И.П.

Сохрание истории шагов Санты (На панели управления имеются кнопки Undo и Redo) - 6ч  
Разработка "Воспроизведения ходов Санты по введеному JSON" (На панели управления есть input с кнопкой(🗿), в который вставляется JSON с ходами) - 6ч  
Разработка "телепорта Санты" - инпут с кнопкой(🌀) на конкретный шаг в истории шагов - 6ч  
Фиксы функциональных багов от тестировщиков (Грабовый С.П., Лобов И.К., Фенев Л.Е.) - 6ч  
Оптимизация JS-кода (Была проблема с лагами из-за вложенных циклов и логики портала) - 3ч  
Совершенствование маршрута, поиск лучших ходов в конкретной части карты 6ч  
Написание документации к проекту - 3ч  

### Фенев Л.Е.
Формулировка задач проекта, организация коммуникации между разработчиками и тестировщиками - 3ч  
Формулировка идей для дополнительного функционала (Совместно с Лобов И.К.) (Кнопки UNDO, REDO, Порталы, воспроизведение шагов по введенной JSON строке) 6ч  
Тестировка приложения (Поиск визуальных и функциональных багов, запросы на исправление разработчикам) 6ч  
Совершенствование маршрута, поиск лучших ходов в конкретной части карты 6ч  
Поиск оптимального маршрута игры 6ч+    
Поиск и создание материалов для визуального улучшения интерфейса (Картинки полей, подарков, санты) - 6ч  
Написание документации к проекту - 3ч  

