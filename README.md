# SUP Console flash programmator
## _Все представленное здесь делается Вами на свой страх и риск._

Простой программатор параллельной flash памяти

- Построен на доступной Arduino Mega 2560
- Минимум дополнительный деталей
- Простота повторения

## Возможности

- Стирание, чтение и запись микросхемы памяти K5L2731CAA-D770 или ей подобных
- Контроль процесса передачи данных между компьютером и программатором
- Контроль процесса записи данных на Flash
- Световая индикация процессов (Запись, Чтение, Стирание, Ошибка)
- Можно определить поведение кнопок (Через исходный код прошивки)
- Можно выводить информацию о процессе на дисплей программатора (Через исходный код прошивки)
- Высокая скорость работы: до 1Mbit/S (Можно и выше, но производительность микроконтроллера не позволяет поднять скорость)

## Установка проекта

Необходим Python не ниже версии 3.9.10. Все операции описаны для ОС Windows с установленным GitBash.
- Необходимо выполнять от имени администратора.

Клонируем репозиторий с GIT:

```sh
git clone git@github.com:Promolife/sup_console_programmator.git
```
Заходим в директорию проекта

```sh
cd sup_console_programmator
```
Устанавливаем и активируем виртуальное окружение

```sh
python -m venv venv
source venv/Scripts/activate
```

Обновляем pip и устанавливаем зависимости

```sh
python -m pip install --upgrade pip
pip install pyserial
```

Готово! Можно начинать использовать.