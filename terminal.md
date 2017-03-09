# Terminal

## Создать папку и сразу перейти в неё

```bash
mkdir folder_name && cd $_
```

А чтобы вернуться в предыдущий каталог, есть команда `cd -`.

## Список файлов

```bash
find ./ -type f -exec echo {} \;
```

## Конвертировать line endings (конец строки) from Windows to Unix

```bash
find ./ -type f -name "*.php" -exec dos2unix {} \;
```

## Удалить доки

```bash
find ./ -type f -name "*.doc*" -exec rm {} \;
```

## Расширение файла в нижний регистр переименовать

```bash
find ./ -type f -exec rename "s/\.JPG$/.jpg/" *.jpg {} \;
```

## Заменить пробелы на подчеркивания

```bash
find ./ -type f -exec rename "s/ /_/" *.jpg {} \;
```

## Имена файлов из русского в транслит

```bash
find ./ -type f -exec totranslit.sh {} \;
```

И папки:

```bash
find ./ -type d -exec totranslit.sh {} \;
```

## Вес размер каталога

```bash
du -sh .git
```

## Вывести все IP-адреса из файлов логов
```
grep -roE '[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}'
```

Если «вышли» из программы через <kbd>Ctrl</kbd>+<kbd>Z</kbd>, то вернуться можно командой `fg`.

`kill` может принимать аргументом номер задачи, а не только идентификатор процесса: `kill %1`.
