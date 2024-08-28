Tmux (ти-макс) — это **менеджер терминалов**, который позволяет работать с несколькими сессиями в одном окне. То есть вместо нескольких открытых окон терминала — вы используете одно, которое можно делить на несколько окон.

Киллер фича ти-макса — сохранение состояний подключений и процессов. После разрыва соединения с сервером вы подключаетесь, и все запущенные программы и процессы продолжают работать.

Несколько основных команд tmux для управления сессиями:

- **attach-session (attach)** - подключиться к уже существующей сессии. В параметре необходимо передать опцию -t и идентификатор сессии;
- **detach-session (detach)** - отключить всех клиентов (или переданного с помощью опции -t) от сессии, переданной в опции -s;
- **has-session** - проверить существует ли сессия, аналогично, надо передать идентификатор сессии;
- **kill-server** - остановить все запущенные сессии;
- **kill-session** - завершить сессию переданную в параметре -t;
- **list-clients** - посмотреть клиентов, подключенных к сессии -t;
- **list-sessions (ls)** - вывести список всех запущенных сессий;
- **new-session** - создать новую сессию, можно передать имя сессии в опции -s и стартовую директорию в опции -c;
- **rename-session** - переименовать сессию, нужно передать идентификатор сессии и новое имя;

По умолчанию для активации сочетания клавиш нужно нажать Ctrl+B, отпустить, а потом нажать нужную клавишу. Вот основные сочетания клавиш tmux, которые вам понадобятся:

- **Ctrl+b c** - создать новое окно;
- **Ctrl+b w** - выбрать окно из списка;
- **Ctrl+b 0-9** - открыть окно по его номеру;
- **Ctrl+b ,** - переименовать текущее окно;
- **Ctrl+b %** - разделить текущую панель по горизонтали;
- **Ctrl+b "** - разделить текущую панель по вертикали;
- **Ctrl+b стрелка** - перейти на панель, находящуюся в стороне, куда указывает стрелка;
- **Ctrl+b Ctrl+стрелка** - изменить размер текущей панели;
- **Ctrl+b o** - перейти на следующую панель;
- **Ctrl+b ;** - переключаться между текущей и предыдущей панелью;
- **Ctrl+b x** - закрыть текущую панель;
- **Ctrl+b [** - войти в режим копирования (подробнее ниже);
- **Ctrl+b ]** - вставить из внутреннего буфера обмена tmux;
- **Ctrl+b d** - отключится от текущей сессии;
- **Ctrl+b :** - открыть командную строку.

С версии 2.1 для включения режима мыши (скролл, изменение размера панели, выбор панели и др.) нужно добавить в tmux.conf:  
  
```
set -g mouse on
```

**Список поддерживаемых комманд**  
``` bash
tmux list-commands
```  
  
**Дополнительная информация**  
``` bash
man tmux
```