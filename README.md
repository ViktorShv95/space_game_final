# Асинхронная игра про космос


## Описание 

Первая часть игры получилось медитативно-утопической. Настало время разбавить первозданный дзен суровой мусорной реальностью!

Перенесите своих игроков в 2000 год – щедро накидайте на экран обломки спутников, старые запчасти и бутылки из-под колы. Пусть уворачиваются от шквала препятствий и думают о поведении человечества!

А когда проблему осознают – переместите всех в 2020. И даруйте лазерную пушку на нос ракеты. Пусть игроки дружно аннигилируют мусорные завалы, освобождая космическое пространство для новых больших свершений. 
## Как установить

1. Клонировать git-репозиторий к себе на компьютер.

```
git clone https://github.com/ViktorKch/space_game_final
```

2. Python3 должен быть уже установлен. 
Затем используйте `pip` (или `pip3`, есть конфликт с Python2) для установки зависимостей:

```
pip3 install -r requirements.txt
```

3. Для запуска игры:

```
python main.py
```

## Дополнительные настройки

Изображения космического корабля находятся в папке `animation_frames`.

Изображения космического мусора находятся в папке `garbage`.

Экран конца игры в папке `game_over`.

По умолчанию игра начинается с 1957 года. Данный параметр можно регулировать изменяя переменную
`start_year` в теле функции `main`. 

Год идет задержка между уровнями (годами) составляет 5 секунд по умолчанию. Ее можно настраивать передавая
в функцию `count_years` параметр `level_duration_sec` с различными значениями.

Символы для изображения звезд находятся в списке `SYMBOLS = ['+', '*', '.', ':']`.

По умолчанию функция `def star_generator(height, width, number=300)` создает 300 звезд. Данный параметр можно изменять, передавая различные значения последнего аргумента в функцию.

## Пример использования программы

![Sample](https://dvmn.org/media/filer_public/f0/c1/f0c1477d-de64-475c-8aba-d30a1c3ee689/fire_garbage.gif)