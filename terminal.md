# Terminal

- See: https://learnxinyminutes.com/docs/ru-ru/bash-ru/
- See: https://github.com/rupa/z

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

## Вес размер каталога

```bash
du -sh .git
```

## Вывести все IP-адреса из лог-файлов

```bash
grep -roE '[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}'
```

## Поиск внутри файлов

```bash
grep -rn "что ищем"
```

## Найти все запущенные процессы определённого пользователя

```bash
ps aux | grep node | grep sergey
```

Если «вышли» из программы через <kbd>Ctrl</kbd>+<kbd>Z</kbd>, то вернуться можно командой `fg`.

`kill` может принимать аргументом номер задачи, а не только идентификатор процесса: `kill %1`.

## Сжать видео через FFMPEG

```bash
ffmpeg -i input.mp4 -vcodec h264 -acodec mp2 output.mp4
```
