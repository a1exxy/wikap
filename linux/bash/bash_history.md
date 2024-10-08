~/.bashrc

HISTSIZE=1000 HISTFILESIZE=2000

So for an infinite history list, make: 

HISTSIZE=(some number less than 0) 

So for an infinite .bash_history history file, make: 

HISTFILESIZE=(some number less than 0)

History size timing:

echo "HISTTIMEFORMAT='%F %T '" >> /home/$USER/.bashrc

Поиск в истории: CTRL+r

Повторение команды:

    Если команда начиналась с comm:

        #!comm

    Если команда содержала comm:

        #!?comm

Очистка экрана: CTRL+l

Настройка истории команд в Bash осуществляется путем добавления переменных окружения в файл ~/.bashrc.

Чтобы изменеия в ~/.bashrc вступили в силу, выполните:

source ~/.bashrc

1. Добавляем Отображение Даты и Времени в Bash History
Иногда очень полезно узнать время, когда какая-либо команда была выполнена.

Установите HISTTIMEFORMAT, чтобы сохранять время выполнения каждой команды.

Для этого добавьте следующую строку в файл ~/.bashrc:

export HISTTIMEFORMAT="%h %d %H:%M:%S "

Теперь, набрав history, Вы получите следующий вывод:

113  Jun 08 16:31:06 sudo ifconfig 114  Jun 08 16:31:10 top 115  Jun 08 16:31:19 ping 8.8.8.8 116  Jun 08 16:31:22 history

2. Увеличиваем Размер Хранимой Истории
Увеличьте HISTSIZE — количество команд, которые необходимо запоминать в списке истории (стандартное значение — 500).

export HISTSIZE=10000

Увеличьте HISTFILESIZE — максимальное количество строк, содержащееся в файле истории (стандартное значение — 500).

export HISTFILESIZE=10000

3. Добавляем Команды Bash в Файл с Историей
Bash перезаписывает файл .bash_history?

Чтобы добавлять новые команды в файл с историей, а не переписывать его каждый раз, добавьте следующую строку в ~/.bashrc:

shopt -s histappend

4. Мгновенно Сохранять Историю Команд
По умолчанию, Bash записывает историю команд в .bash_history, при завершении сессии.

Если сессия внезапно оборвется Вы потеряете текущую историю команд.

Используйте переменную $PROMPT_COMMAND, чтобы сохранять команды сразу после выполнения:

Добавьте следующую строку в файл ~/.bashrc, если переменная $PROMPT_COMMAND не была задана ранее:

PROMPT_COMMAND='history -a'

Добавьте следующую строку, если переменная $PROMPT_COMMAND уже была задана:

PROMPT_COMMAND='$PROMPT_COMMAND; history -a'

5. Контролируйте Bash History
HISTCONTROL — представляет из себя список опций, разделенных двоеточиями.

Они контролируют каким образом список команд сохраняется в истории.

| Опция | Описание |
|-------|-----------------------------------|
| ignorespace | не сохранять строки начинающиеся с символа <пробел> |
|-------|-----------------------------------|
| ignoredups | не сохранять строки, совпадающие с последней выполненной командой | 
|-------|-----------------------------------|
| ignoreboth | использовать обе опции ‘ignorespace’ и ‘ignoredups’ | 
|-------|-----------------------------------|
| erasedups | удалять ВСЕ дубликаты команд с истории |
|-------|-----------------------------------|

Пример:

export HISTCONTROL=ignorespace:erasedups

6. Игнорировать Определенные Команды
HISTIGNORE — список шаблонов через двоеточие, используемых для принятия решения о сохранении строк с командами в списке истории.

Не сохранять команды ls, ps и history:

export HISTIGNORE="ls:ps:history"

Не сохранять команды начинающиеся с s:

export HISTIGNORE="s*"

7. Одна Команда — Одна Запись в Истории
Сохранять все строки многострочной команды в одной записи списка истории:

shopt -s cmdhist

Изменить Имя Файла с Историй Команд
Используйте HISTFILE для изменения имени файла, в котором сохраняется история команд. Стандартное значение ~/.bash_history.

export HISTFILE=~/.custom_file