# Настраиваем IntelejiIDEA

Настраиваем IntelejiIDEA:

- Устанавливаем плагины
    - Настраиваем плагин для vim
- Импортируем раскладку
- Добавляем Theme, для подсветки синтаксиса

# Простой способ установки

Простой способ - не совсем рабочий метод:

- File -> Manage IDE Settings -> Import Settings... -> Выбираем путь: ./settings/settings.zip

Минусы:

- Плагины придется устанавливать самому
- Theme не подключается
- vimrc тоже надо скопировать

# Устанавливаем Plugins

Устанавливаем Plugins, отсюда:

```bash
File -> Setting -> Plugins -> Marketplace
```

Plugins которые ищем:

- IdeaVim
    - добавляет в editor режимы из vim
        - normal
        - insert
        - select
    - добавляет в editor раскладку из vim
        - работает только для editor
        - поэтому для полноценной работы нужно еще настроить просто keymap для IDEA
- IdeaVimExtension
    - переключает раскладку на английский при выходе из режима вставки в vim
- AceJump
    - позволяет быстро перемещаться к символу на экране


# Пошаговый способ установки

## Устанавливаем Theme

Устанавливаем Theme, заходим в IDEA в:

```bash
File -> Setting -> Editor -> Color scheme
```

В окне настроек:

- настройки - в виде иконки шестеренки

```bash
настройки -> Import Shceme -> Выбираем путь: ./style/VSCode_Dark.icls
```

## Устанавливаем Keymap

Устанавливаем Keymap, заходим в IDEA в:

```bash
File -> ManageIDEA -> Import settings... -> Выбираем путь: ./vim/keymap.zip 
```

Устанавливаем vim конфиг:

- должны быть установлены Plugins
- настройка .ideavimrc
  - в IDEA, в строке состояния(внизу) находим зеленную букву V, и в ней выбираем пункт .ideavimrc 
  - в отрывшийся файл, копируем текст из ./vim/ideavimrc
    Подключаем .vimrc:

- Включаем IdeaVim

```bash
/*Bottom Panel*/ | > V | > Enable            |
                       |   Open ~/.ideavimrc |
                       |   ...               |
```

- Копируем в открытый файл, настройки для IdeaVim, из ./ideavimrc
- Не забудь дернуть кнопку обновления, для файла ideavimrc(в правом верхнем углу editor)

```bash
/*Bottom Panel*/ | > V |   Enable            |
                       | > Open ~/.ideavimrc |
                       |   ...               |
```

## Устанавливаем UI

Устанавливаем UI - настройки интерфейса:

```bash
File -> ManageIDEA -> Import settings... -> Выбираем путь: ./vim/keymap.zip 
```
