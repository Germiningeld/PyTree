# Tree 🌲

Простая и удобная утилита для визуализации структуры директорий и файлов проекта.

## Описание

Tree - это легковесный инструмент, который позволяет вывести древовидную структуру файлов и директорий в консоль с визуальным форматированием. Утилита отображает директории и файлы с соответствующими иконками (📁 для папок и 📄 для файлов), что делает вывод более наглядным.

## Особенности

- Визуальное представление структуры директорий в виде дерева
- Автоматическое исключение служебных директорий (.git, node_modules, __pycache__ и др.)
- Корректная работа с вложенностью любой глубины
- Поддержка Unicode-иконок для улучшенной читаемости

## Использование

```bash
python tree.py
```

По умолчанию утилита сканирует текущую директорию. 

## Настройка

Вы можете изменить список исключаемых директорий, отредактировав параметр `exclude_dirs` в функции `print_tree`:

```python
exclude_dirs=[
    '.venv',
    '.idea',
    '__pycache__',
    '.git',
    '.pytest_cache',
]
```

## Зависимости

- Python 3.x
- Стандартная библиотека Python (os)

## Планы развития

- Добавление параметров командной строки для настройки
- Поддержка фильтрации по расширениям файлов
- Возможность сохранения вывода в файл
- Подсветка синтаксиса для разных типов файлов

## Лицензия

[MIT](LICENSE)