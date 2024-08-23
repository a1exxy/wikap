Очень хороший способ запустить tmux:

tmux attach || tmux new — делая так, вы сперва пытаетесь подключиться к уже существующему серверу tmux, если он существует; если такого ещё нет — создаёте новый.

После этого вы попадаете в полноценную консоль.

Ctrl+b d — отключиться. (Точно так же вы отключитесь, если прервётся соединение. Как подключиться обратно и продолжить работу — см. выше.)

В одной сессии может быть сколько угодно окошек:

Ctrl+b c — создать окошко;

Ctrl+b 0...9 — перейти в такое-то окошко;

Ctrl+b p — перейти в предыдущее окошко;

Ctrl+b n — перейти в следующее окошко;

Ctrl+b l — перейти в предыдущее активное окошко (из которого вы переключились в текущее);

Ctrl+b & — закрыть окошко (а можно просто набрать exit в терминале).

В одном окошке может быть много панелей:

Ctrl+b % — разделить текущую панель на две, по вертикали;

Ctrl+b " — разделить текущую панель на две, по горизонтали (это кавычка, которая около Enter, а не Shift+2);

Ctrl+b →←↑↓ — переходить между панелями;

Ctrl+b x — закрыть панель (а можно просто набрать exit в терминале).

Недостаток — непривычным становится скроллинг:

Ctrl+b PgUp — вход в «режим копирования», после чего:

PgUp, PgDown — скроллинг;

q — выход из «режима копирования».

tmux — консольный оконный менеджер, похожий на GNU Screen, но отличающийся от него рядом серьёзных усовершенствований.

Основные преимущества tmux в сравнении с GNU Screen:

Ясная и прозрачная клиент-серверная модель (например, можно без проблем подключать разные окна к разным сеансам);

Простой интерфейс командной строки;

Единый синтаксис команд в конфигурационном файле, в командной строке оболочки и в командной строке tmux;

Простота написания скриптов;

Множество буферов вставки;

Комбинации клавиш vi/emacs;

Простой синтаксис командной строки, поддерживающий вывод внешних команд shell.

Содержание [убрать]

1 Управление окнами

2 Управление панелями

3 .tmux.conf

4 Возможности Screen не поддерживаемые в tmux

5 Приятные дополнения и навороты

5.1 Как сделать максимизацию текущей панели?

5.2 Как включить прокрутку по shift pgup/pgdn?

5.3 Как послать текст в окно tmux?

5.4 Как копировать текст между окнами/буферами tmux?

6 Дополнительная информация

[править]

Управление окнами
Очень похоже на то, как это сделано в screen.

ctrl-b c (tmux new-window)

создать новое окно

ctrl-b 0-9 (tmux select-window -t 

0-9)

перейти на окно с заданным номером

ctrl-b , (tmux rename-window)

переименовать текущее окно

ctrl-b n

перейти на следующее окно

ctrl-b f

найти окно по имени

ctrl-b w

выбрать окно в меню

[править]

Управление панелями
tmux split-window (prefix + ")

разбить по вертикали

tmux split-window -h (prefix + %)

разбить по горизонтали

tmux swap-pane -[UDLR] (prefix + { or }, prefix + стрелки)

поменять текущую панель с другой, по указанному направлению

tmux select-pane -[UDLR]

перейти на панель в указанном направлении

tmux select-pane -t :.+

перейти на следующую панель

(prefix SPACE)

циклически менять расположение панелей (even-horizontal, even-vertical, main-horizontal, main-vertical, tiled)

(prefix !)

перенести текущую панель на новое окно

[править]

.tmux.conf
Удобные настройки (особенно при переходе со Screen), добавляются в ~/.tmux.conf:

# привязать главный префикс на ctrl-a, по умолчанию находится на ctrl-b set -g prefix C-a unbind C-b bind C-a send-prefix  # перечитать конфигурационный файл, c-a r unbind r bind r source-file ~/.tmux.conf  # перейти на другую панель c-a c-a unbind ^A bind ^A select-pane -t :.+

[править]

Возможности Screen не поддерживаемые в tmux
Функции, которые не поддерживает tmux, но поддерживает screen:

zmodem transfers. в screen можно передавать файлы по zmodem. Для этоно надо нажать ctrl-a :zmodem catch и sz на том конце. Tmux так не умеет (скриптами можно заставить).

подключение к serial-интерфейсу. Screen может работать на последовательном порту (screen -r /dev/ttyS0 115200), tmux — нет.

Автоматическое логгирование сеанса tmux тоже не может делать (скриптами можно заставить, см. ниже).

[править]

Приятные дополнения и навороты
[править]

Как сделать максимизацию текущей панели?
В самом tmux такой возможности нет, но её легко реализовать самому [1]:

unbind + bind + new-window -d -n tmux-zoom 'clear && echo TMUX ZOOM && read' \; swap-pane -s tmux-zoom.0 \; select-window -t tmux-zoom unbind - bind - last-window \; swap-pane -s tmux-zoom.0 \; kill-window -t tmux-zoom

[править]

Как включить прокрутку по shift pgup/pgdn?
Вообще прокрутка доступна по prefix [ или prefix pgup (автоматически включается режим прокрутки и прокручивается один экран), но если хочется именно по shift pgup/pgdown, то нужно добавить в tmux.conf [2]:

set -g terminal-overrides 'xterm*:smcup@:rmcup@'

[править]

Как послать текст в окно tmux?
Использовать `send-keys`:

 tmux send-keys -t 0.2 'echo hi' Enter

Здесь мы посылаем в панель 2 окна 0 текст echo hi и нажимаем Enter.

Подробнее: [3].

[править]

Как копировать текст между окнами/буферами tmux?
setw -g mode-keys vi # vim-style movement # in normal tmux mode bind Escape copy-mode # `tmux prefix + Escape` starts copy mode. bind p paste-buffer # `prefix + p` pastes the latest buffer  # in copy mode… bind -t vi-copy v begin-selection # `v` begins a selection. (movement keys to select the desired bits) bind -t vi-copy y copy-selection # `y` copies the current selection to one of tmux's "paste buffers" bind -t vi-copy V rectangle-toggle # `V` changes between line- and columnwise selection  bind -t vi-copy Y copy-end-of-line # ^1 bind + delete-buffer

Управляющие клавиши:

#           List all paste buffers. -           Delete the most recently copied buffer of text. =           Choose which buffer to paste interactively from a list. [           Enter copy mode to copy text or view the history. ]           Paste the most recently copied buffer of text. 

Источник: Copy and Paste in `tmux`.

[править]

Дополнительная информация
tmux is sweet as heck (англ.) — некоторые преимущества tmux по сравнению с GNU Screen

tmux: Productive Mouse-Free Development (англ.) — интересная книга про tmux из серии Pragmatic Programmer

Multiplexers: Screen, Tmux — Hyperpolyglot (англ.) — основные комбинации клавиш и команды tmux и screen; хорошее введение для пользователей screen чтобы быстрее перейти на tmux

screen and tmux (англ.) — сравнение основных комбинаций клавиш и команд screen и tmux

tmux and mouse mode (англ.) — вопросы использования мыши в tmux

A Tmux Crash Course (англ.) — небольшая подборка советов по работе с tmux

TMUX – The Terminal Multiplexer (англ.) — короткое, но хорошее введение в tmux; освоение можно начать с него

Специальные вопросы:

Run command in detached tmux session (англ.) — как выполнить команду в отключенном сеансе tmux

Automatically start tmux on SSH login (англ.) — автоматический запуск tmux при входе в систему

Is there an equivalent of GNU Screen's “log” command in tmux? (англ.) — как автоматически записывать всё, что происходит в консоли tmux

tmux — unlimited history? (англ.) — как сделать неограниченную историю в tmux (почти неограниченную)