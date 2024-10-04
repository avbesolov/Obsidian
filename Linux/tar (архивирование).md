В Linux можно заархивировать директорию несколькими способами, но наиболее распространённый и удобный метод — использование команды `tar`. Вот как это можно сделать:

### Архивирование:

1. **Создание архива `.tar`:**

    `tar -cvf archive_name.tar /path/to/directory`
    
    - `-c` (create) — создать новый архив.
    - `-v` (verbose) — вывести процесс на экран.
    - `-f` (file) — указывает имя создаваемого архива.
    - `archive_name.tar` — имя создаваемого архива.
    - `/path/to/directory` — путь к директории, которую ��ы хотите заархивировать.
2. **Создание архива с компрессией `.tar.gz`:**
    
    `tar -czvf archive_name.tar.gz /path/to/directory`
    
    - `-z` (gzip) — сжать архив с помощью gzip.
3. **Создание архива с компрессией `.tar.bz2`:**

    `tar -cjvf archive_name.tar.bz2 /path/to/directory`
    
    - `-j` (bzip2) — сжать архив с помощью bzip2.
4. **Создание архива с компрессией `.tar.xz`:**

    `tar -cJvf archive_name.tar.xz /path/to/directory`
    
    - `-J` (xz) — сжать архив с помощью xz.

### Разархивирование:

Для разархивирования архива используйте команду `tar` с ключом `-x`:

1. **Разархивирование `.tar`:**

    `tar -xvf archive_name.tar`
    
2. **Разархивирование `.tar.gz`:**

    `tar -xzvf archive_name.tar.gz`
    
3. **Разархивирование `.tar.bz2`:**

    `tar -xjvf archive_name.tar.bz2`
    
4. **Разархивирование `.tar.xz`:**

    `tar -xJvf archive_name.tar.xz`
    

Если нужно разархивировать в определённую директорию, добавьте ключ `-C` (например, `-C /path/to/extract`).
