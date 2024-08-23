Глава 15. Управление виртуальными машинами с помощью virsh
Текстовая утилита virsh предназначена для управления гостевыми системами и гипервизором.

virsh использует libvirt API и служит альтернативой xm и графическому менеджеру виртуальных машин (virt-manager). Непривилегированные пользователи могут выполнять доступ в только в режиме чтения. С помощью virsh можно исполнять сценарии для виртуальных машин.

Обзор команд virsh

Приведенные ниже таблицы содержат перечень основных параметров командной строки virsh.


<table xmlns="http://www.w3.org/1999/xhtml" border="1" style="border:1px solid rgb(60,110,180);width:659px;border-collapse:collapse" data-table-local-id="table-2">
  <colgroup>
    <col width="50%">
    <col width="50%">
  </colgroup>
  <thead>
    <tr>
      <th style="border-top-width:1px;border-right-width:1px;border-left-width:1px;border-top-style:solid;border-right-style:solid;border-left-style:solid;border-color:rgb(0,0,0);padding:0.3em 0.5em;color:white;background-color:rgb(60,110,180)">Команда</th>
      <th style="border-top-width:1px;border-right-width:1px;border-left-width:1px;border-top-style:solid;border-right-style:solid;border-left-style:solid;border-color:rgb(0,0,0);padding:0.3em 0.5em;color:white;background-color:rgb(60,110,180)">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">help</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Краткая справка.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">list</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Просмотр всех виртуальных машин.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">dumpxml</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Вывести файл конфигурации XML для заданной виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">create</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Создать виртуальную машину из файла конфигурации XML и ее запуск.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">start</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Запустить неактивную виртуальную машину.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">destroy</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Принудительно остановить работу виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">define</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Определяет файл конфигурации XML для заданной виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">domid</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Просмотр идентификатора виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">domuuid</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Просмотр UUID виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">dominfo</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Просмотр сведений о виртуальной машине.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">domname</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Просмотр имени виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">domstate</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Просмотр состояния виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">quit</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Закрыть интерактивный терминал.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">reboot</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Перезагрузить виртуальную машину.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">restore</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Восстановить сохраненную в файле виртуальную машину.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">resume</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Возобновить работу приостановленной виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">save</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Сохранить состояние виртуальной машины в файл.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">shutdown</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Корректно завершить работу виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">suspend</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Приостановить работу виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">undefine</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Удалить все файлы виртуальной машины.</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">
        <code style="font-family:liberation mono,bitstream vera mono,dejavu mono,monospace;white-space:nowrap;font-weight:bold">migrate</code>
      </td>
      <td style="border:1px solid rgb(0,0,0);padding:0.15em 0.5em">Перенести виртуальную машину на другой узел.</td>
    </tr>
  </tbody>
</table>