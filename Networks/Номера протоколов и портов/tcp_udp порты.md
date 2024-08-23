
## Общеизвестные порты

<table xmlns="http://www.w3.org/1999/xhtml" style="font-size:14px;background-color:rgb(248,249,250);color:rgb(34,34,34);margin-top:1em;margin-bottom:1em;border:1px solid rgb(162,169,177);border-collapse:collapse;font-family:sans-serif" data-table-local-id="table-2">
  <thead>
    <tr>
      <th style="border-top:1px solid rgb(162,169,177);border-right:1px solid rgb(162,169,177);border-left:1px solid rgb(162,169,177);border-bottom-color:rgb(162,169,177);padding:0.2em 21px 0.2em 0.4em;background-color:rgb(234,236,240);text-align:center;background-image:linear-gradient(transparent,transparent),url(&quot;&quot;);background-repeat:no-repeat;background-position:right center" title="Упорядочить по возрастанию">Порт/Протокол</th>
      <th style="border-top:1px solid rgb(162,169,177);border-right:1px solid rgb(162,169,177);border-left:1px solid rgb(162,169,177);border-bottom-color:rgb(162,169,177);padding:0.2em 21px 0.2em 0.4em;background-color:rgb(234,236,240);text-align:center;background-image:linear-gradient(transparent,transparent),url(&quot;&quot;);background-repeat:no-repeat;background-position:right center" title="Упорядочить по возрастанию">Описание</th>
      <th style="border-top:1px solid rgb(162,169,177);border-right:1px solid rgb(162,169,177);border-left:1px solid rgb(162,169,177);border-bottom-color:rgb(162,169,177);padding:0.2em 21px 0.2em 0.4em;background-color:rgb(234,236,240);text-align:center;background-image:linear-gradient(transparent,transparent),url(&quot;&quot;);background-repeat:no-repeat;background-position:right center" title="Упорядочить по возрастанию">Использование</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">0/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв (допустимо использование в качестве значения порта источника, если отправляющий процесс не ожидает ответных сообщений)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Tcpmux" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Tcpmux">TCPMUX (TCP Port Service Multiplexer)</a>
        &nbsp;— для обслуживания нескольких служб через один TCP-порт
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">2/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">COMPRESSNET, процесс управления</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">3/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">COMPRESSNET, процесс сжатия</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">5/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RJE (Remote Job Entry)&nbsp;— обслуживает отправку файлов и вывод отчётов при работе рабочей станции с&nbsp;
        <a href="https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D0%B9%D0%BD%D1%84%D1%80%D0%B5%D0%B9%D0%BC" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Мейнфрейм">мейнфреймами</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">7/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ECHO&nbsp;— предназначен для тестирования связи путём отправки данных на сервер и получения от него их же в неизменном виде</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">9/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        DISCARD&nbsp;— предназначен для тестирования связи путём отправки данных на сервер, который отбрасывает принятое, не отправляя никакого ответа. Также используется для&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Wake-on-LAN" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Wake-on-LAN">Wake-on-LAN</a>
        -удалённого включения компьютера.
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">11/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SYSTAT&nbsp;— выдаёт список активных пользователей в операционной системе</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">13/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DAYTIME&nbsp;— предназначен для тестирования связи путём получения от сервера текущих даты и времени в текстовом виде</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">15/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        не назначено; ранее&nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/NETSTAT" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NETSTAT">NETSTAT</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">17/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Quote_of_the_day" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Quote of the day">QOTD (Quote of the Day)</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">18/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Message_Send_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Message Send Protocol (страница отсутствует)">MSP (Message Send Protocol)</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Message_Send_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Message Send Protocol">
              <span title="Message Send Protocol — версия статьи «Message Send Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">19/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/CHARGEN" rel="nofollow" style="color:rgb(11,0,128);background:none" title="CHARGEN">CHARGEN (Character Generator)</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">20/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        FTP-DATA&nbsp;— для передачи данных&nbsp;
        <a href="https://ru.wikipedia.org/wiki/FTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="FTP">FTP</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">21/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        FTP&nbsp;— для передачи команд&nbsp;
        <a href="https://ru.wikipedia.org/wiki/FTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="FTP">FTP</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">22/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/SSH" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSH">SSH (Secure SHell)</a>
        &nbsp;— криптографический сетевой протокол для безопасной передачи данных
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">23/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Telnet" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Telnet">Telnet</a>
        &nbsp;— применяется для передачи текстовых сообщений в незашифрованном виде
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">24/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PRIV-MAIL&nbsp;— для использования в любых частных системах пересылки почтовых сообщений</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">25/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/SMTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SMTP">SMTP (Simple Mail Transfer Protocol)</a>
        &nbsp;— применяется для пересылки почтовых сообщений в виде незашифрованного текста
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">26/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RSFTP&nbsp;— упрощенный аналог протокола&nbsp;
        <a href="https://ru.wikipedia.org/wiki/FTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="FTP">FTP</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">26/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в игре&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Dungeon_Siege_II" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Dungeon Siege II">Dungeon Siege II</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">27/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NSW-FE (NSW User System FE)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">29/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MSG-ICP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">31/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MSG-AUTH</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">33/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DSP (Display Support Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">35/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        PRIV-PRINT&nbsp;— для использования любыми частными&nbsp;
        <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B5%D1%80%D0%B2%D0%B5%D1%80_%D0%BF%D0%B5%D1%87%D0%B0%D1%82%D0%B8" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Сервер печати">серверами печати</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">35/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в игре&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Delta_Force_(%D1%81%D0%B5%D1%80%D0%B8%D1%8F_%D0%B8%D0%B3%D1%80)" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Delta Force (серия игр)">Delta Force</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">37/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=TIME_(%D0%BF%D1%80%D0%BE%D1%82%D0%BE%D0%BA%D0%BE%D0%BB)&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="TIME (протокол) (страница отсутствует)">TIME</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Time_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Time Protocol">
              <span title="Time Protocol — версия статьи «TIME (протокол)» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;— используется для синхронизации времени (устар.)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">38/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RAP (Route Access Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">39/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RLP (Resource Location Protocol)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-1" rel="nofollow" style="color:rgb(11,0,128);background:none">[1]</a>
        </sup>
        , протокол поиска ресурсов&nbsp;— служит для нахождения серверов, предоставляющих услуги верхнего уровня
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">41/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Graphics&nbsp;— используется графическими модулями некоторых браузерных программ</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">42/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NAME, NAMESERVER&nbsp;—&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=ARPA_Host_Name_Server_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="ARPA Host Name Server Protocol (страница отсутствует)">ARPA Host Name Server Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/ARPA_Host_Name_Server_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:ARPA Host Name Server Protocol">
              <span title="ARPA Host Name Server Protocol — версия статьи «ARPA Host Name Server Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        , протокол сервера имён&nbsp;
        <a href="https://ru.wikipedia.org/wiki/ARPA" rel="nofollow" style="color:rgb(11,0,128);background:none" title="ARPA">ARPA</a>
        &nbsp;(устар.)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">42/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Windows_Internet_Name_Service" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Windows Internet Name Service">WINS (Windows Internet Name Service)</a>
        &nbsp;— в настоящее время считается устаревшим
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">43/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/WHOIS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="WHOIS">WHOIS</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">44/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MPM-FLAGS (Message Processing Module, Flags)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">45/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MPM (Message Processing Module, receive)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">46/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MPM-SND (Message Processing Module, send)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">47/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NI-FTP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">48/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AUDITD (Digital Audit Daemon)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">49/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/TACACS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TACACS">TACACS</a>
        &nbsp;Login Host protocol
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">50/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RE-MAIL-CK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">51/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв; ранее&nbsp;— LA-MAINT (IMP Logical Address Maintenance)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">52/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        XNS-TIME (
        <a href="https://ru.wikipedia.org/wiki/Xerox_Network_Services" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Xerox Network Services">Xerox Network Services</a>
        &nbsp;Time Protocol)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">53/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        DOMAIN (
        <a href="https://ru.wikipedia.org/wiki/Domain_Name_System" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Domain Name System">Domain Name System</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">54/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        XNS-CH (
        <a href="https://ru.wikipedia.org/wiki/Xerox_Network_Services" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Xerox Network Services">Xerox Network Services</a>
        &nbsp;ClearingHouse)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">55/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        ISI-GL (ISI Graphics Language)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-2" rel="nofollow" style="color:rgb(11,0,128);background:none">[2]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">56/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        XNS-AUTH (
        <a href="https://ru.wikipedia.org/wiki/Xerox_Network_Services" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Xerox Network Services">Xerox Network Services</a>
        &nbsp;Authentication)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">56/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RAP (Route Access Protocol)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-3" rel="nofollow" style="color:rgb(11,0,128);background:none">[3]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">57/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        PRIV-TERM&nbsp;— для любых служб, обеспечивающих терминальный доступ; ранее&nbsp;— MTP (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Mail_Transfer_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Mail Transfer Protocol (страница отсутствует)">Mail Transfer Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Mail_Transfer_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Mail Transfer Protocol">
              <span title="Mail Transfer Protocol — версия статьи «Mail Transfer Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">58/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        XNS-MAIL (
        <a href="https://ru.wikipedia.org/wiki/Xerox_Network_Services" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Xerox Network Services">Xerox Network Services</a>
        &nbsp;Mail)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">59/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PRIV-FILE&nbsp;— для любых служб обработки файлов</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">61/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NI-MAIL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">62/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ACAS (ACA Services)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">63/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">WHOISPP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">64/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">COVIA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">65/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        TACACS-DS (
        <a href="https://ru.wikipedia.org/wiki/TACACS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TACACS">TACACS</a>
        &nbsp;Database Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">66/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SQL-NET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">67/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        BOOTPS (
        <a href="https://ru.wikipedia.org/wiki/Bootstrap_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Bootstrap Protocol">Bootstrap Protocol</a>
        &nbsp;Server)&nbsp;— для сервера, с которого выполняется загрузка бездисковых рабочих станций; также используется DHCP (
        <a href="https://ru.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Dynamic Host Configuration Protocol">Dynamic Host Configuration Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">68/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        BOOTPC (
        <a href="https://ru.wikipedia.org/wiki/Bootstrap_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Bootstrap Protocol">Bootstrap Protocol</a>
        &nbsp;Client)&nbsp;— для клиентов бездисковых рабочих станций, загружающихся с сервера BOOTP; также используется DHCP (
        <a href="https://ru.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Dynamic Host Configuration Protocol">Dynamic Host Configuration Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">69/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        TFTP (
        <a href="https://ru.wikipedia.org/wiki/Trivial_File_Transfer_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Trivial File Transfer Protocol">Trivial File Transfer Protocol</a>
        )&nbsp;— тривиальный FTP применяется, например, при установке операционной системы на большое количество компьютеров в сетях предприятий. Для этого сервер TFTP и поддержка удалённого развёртывания (UAM) включены в состав серверных ОС&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Windows_NT" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Windows NT">Windows NT4 Server</a>
        &nbsp;и новее
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">70/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Gopher_(%D1%81%D0%B5%D1%82%D0%B5%D0%B2%D0%BE%D0%B9_%D0%BF%D1%80%D0%BE%D1%82%D0%BE%D0%BA%D0%BE%D0%BB)" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Gopher (сетевой протокол)">Gopher</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">71/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETRJS-1 (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Remote_job_entry&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Remote job entry (страница отсутствует)">Remote job entry</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Remote_job_entry" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Remote job entry">
              <span title="Remote job entry — версия статьи «Remote job entry» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">72/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETRJS-2 (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Remote_job_entry&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Remote job entry (страница отсутствует)">Remote job entry</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Remote_job_entry" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Remote job entry">
              <span title="Remote job entry — версия статьи «Remote job entry» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">73/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETRJS-3 (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Remote_job_entry&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Remote job entry (страница отсутствует)">Remote job entry</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Remote_job_entry" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Remote job entry">
              <span title="Remote job entry — версия статьи «Remote job entry» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">74/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETRJS-4 (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Remote_job_entry&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Remote job entry (страница отсутствует)">Remote job entry</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Remote_job_entry" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Remote job entry">
              <span title="Remote job entry — версия статьи «Remote job entry» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">75/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PRIV-DIAL&nbsp;— для любых приложений телефонного дозвона</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">76/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DEOS (Distributed External Object Store)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">77/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        PRIV-RJE&nbsp;— для использования в любых службах&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Remote_Job_Entry&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Remote Job Entry (страница отсутствует)">Remote Job Entry</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Remote_job_entry" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Remote job entry">
              <span title="Remote job entry — версия статьи «Remote Job Entry» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">78/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VETTCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">79/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Finger" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Finger">Finger</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">80/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HTTP (
        <a href="https://ru.wikipedia.org/wiki/HyperText_Transfer_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="HyperText Transfer Protocol">HyperText Transfer Protocol</a>
        ); ранее&nbsp;— WWW
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">81/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HTTP (
        <a href="https://ru.wikipedia.org/wiki/HyperText_Transfer_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="HyperText Transfer Protocol">HyperText Transfer Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">81/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        используется в приложениях проекта&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Tor" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Tor">Tor</a>
        &nbsp;для целей маршрутизации
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">81/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HOSTS2-NS (HOSTS2 Name Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">82/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">XFER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">82/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        используется в приложениях проекта&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Tor" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Tor">Tor</a>
        &nbsp;для целей управления
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">83/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MIT-ML-DEV (MIT ML Device)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">84/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CTF (Common Trace Facility)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">85/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MIT-ML-DEV (MIT ML Device)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">86/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MFCOBOL (Micro Focus Cobol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">87/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        PRIV-TERM-L&nbsp;— для любых приложений, обеспечивающих терминальное соединение типа «текстовый&nbsp;
        <a href="https://ru.wikipedia.org/wiki/%D0%A7%D0%B0%D1%82" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Чат">чат</a>
        » (например, аналогичных&nbsp;
        <a href="https://ru.wikipedia.org/w/index.php?title=Talk_(software)&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Talk (software) (страница отсутствует)">talk</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">88/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        Система аутентификации&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">89/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SU-MIT-TG (SU/MIT Telnet Gateway)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">90/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        DNSIX (
        <a href="https://ru.wikipedia.org/wiki/DoD" rel="nofollow" style="color:rgb(11,0,128);background:none" title="DoD">DoD</a>
        &nbsp;Network Security for Information eXchange) Securit Attribute Token Map
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">90/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=PointCast&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="PointCast (страница отсутствует)">PointCast</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/PointCast_(dotcom)" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:PointCast (dotcom)">
              <span title="PointCast (dotcom) — версия статьи «PointCast» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">91/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MIT-DOV (MIT Dover Spooler)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">92/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NPP (Network Printing Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">93/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DCP (Device Control Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">94/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OBJCALL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">95/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SUPDUP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">96/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DIXIE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">97/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SWIFT-RVF (Swift Remote Virtural File Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">98/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TACNEWS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">98/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LINUXCONF</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">99/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">METAGRAM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">100/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NEWACCT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">101/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HOSTNAME (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=InterNIC&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="InterNIC (страница отсутствует)">NIC</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Network_Information_Center" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Network Information Center">
              <span title="Network Information Center — версия статьи «InterNIC» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Host Name Server)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">102/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        ISO-TSAP (Transport&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Service_Access_Point&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Service Access Point (страница отсутствует)">Service Access Point</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Service_Access_Point" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Service Access Point">
              <span title="Service Access Point — версия статьи «Service Access Point» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Class 0)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-4" rel="nofollow" style="color:rgb(11,0,128);background:none">[4]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">103/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GPPITNP (Genesis Point-to-Point Trans Net)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">104/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        ACR-NEMA (ACR/NEMA&nbsp;
        <a href="https://ru.wikipedia.org/wiki/DICOM" rel="nofollow" style="color:rgb(11,0,128);background:none" title="DICOM">DICOM</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">105/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        CSO, CSNET-NS (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=CCSO&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="CCSO (страница отсутствует)">CCSO</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/CCSO_Nameserver" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:CCSO Nameserver">
              <span title="CCSO Nameserver — версия статьи «CCSO» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        /Mailbox Name Nameserver)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">106/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">3COM-TSMUX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">107/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RTELNET (Remote&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Telnet" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Telnet">Telnet</a>
        &nbsp;Service
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-5" rel="nofollow" style="color:rgb(11,0,128);background:none">[5]</a>
        </sup>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">108/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SNAGAS (
        <a href="https://ru.wikipedia.org/wiki/SNA" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SNA">SNA</a>
        &nbsp;Gateway Access Server)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">109/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        POP2 (
        <a href="https://ru.wikipedia.org/wiki/Post_Office_Protocol#%D0%98%D1%81%D1%82%D0%BE%D1%80%D0%B8%D1%8F" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Post Office Protocol">Post Office Protocol</a>
        &nbsp;Version 2)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">110/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        POP3 (
        <a href="https://ru.wikipedia.org/wiki/Post_Office_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Post Office Protocol">Post Office Protocol</a>
        &nbsp;Version 3)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">110/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в игре&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Final_Fantasy_XI" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Final Fantasy XI">Final Fantasy XI</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">111/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SUNRPC (
        <a href="https://ru.wikipedia.org/wiki/Sun_Microsystems" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Sun Microsystems">Sun</a>
        &nbsp;
        <a href="https://ru.wikipedia.org/wiki/Remote_Procedure_Call" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Remote Procedure Call">Remote Procedure Call</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">112/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MCIDAS (McIDAS Data Transmission)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">113/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AUTH (Authentication Service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">113/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Ident" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Ident">IDENT</a>
        &nbsp;— старая система идентификации, до сих пор используется в&nbsp;
        <a href="https://ru.wikipedia.org/wiki/IRC" rel="nofollow" style="color:rgb(11,0,128);background:none" title="IRC">IRC</a>
        -серверах
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">114/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AUDIONEWS (Audio News Multicast)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">115/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SFTP (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Simple_File_Transfer_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Simple File Transfer Protocol (страница отсутствует)">Simple File Transfer Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Simple_File_Transfer_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Simple File Transfer Protocol">
              <span title="Simple File Transfer Protocol — версия статьи «Simple File Transfer Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">116/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ANSANOTIFY (ANSA REX Notify)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">117/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        UUCP-PATH (
        <a href="https://ru.wikipedia.org/wiki/UUCP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="UUCP">UUCP</a>
        &nbsp;Path Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">118/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SQLSERV (
        <a href="https://ru.wikipedia.org/wiki/SQL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SQL">SQL</a>
        &nbsp;Services)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">119/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NNTP (
        <a href="https://ru.wikipedia.org/wiki/Network_News_Transfer_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Network News Transfer Protocol">Network News Transfer Protocol</a>
        )&nbsp;— используется для отправки сообщений новостных рассылок
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">120/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        CFDPTKT (
        <a href="https://tools.ietf.org/html/rfc1235" rel="nofollow" style="color:rgb(102,51,102);background:linear-gradient(transparent,transparent) right center no-repeat,url(&quot;&quot;);padding-right:13px">RFC 1235</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">121/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ERPC (Encore Expedited Remote Protocol Call)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">122/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SMAKYNET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">123/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NTP (
        <a href="https://ru.wikipedia.org/wiki/Network_Time_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Network Time Protocol">Network Time Protocol</a>
        )&nbsp;— используется для синхронизации времени
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">124/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ANSATRADER (ANSA REX Trader)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">125/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LOCUS-MAP (Locus PC-Interface Net Map Ser)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">125/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        используется как альтернатива порту 25/TCP (
        <a href="https://ru.wikipedia.org/wiki/SMTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SMTP">SMTP</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">126/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NXEdit; ранее&nbsp;— Unisys Unitary Login</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">127/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LOCUS-CON (Locus PC-Interface Conn Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">127/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в игре&nbsp;
        <a href="https://ru.wikipedia.org/w/index.php?title=Command_and_Conquer_Generals&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Command and Conquer Generals (страница отсутствует)">Command and Conquer Generals</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">128/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GSS-XLICEN (GSS X License Verification)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">129/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PWDGEN (Password Generator Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">130/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CISCO-FNA (Cisco FNATIVE)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">131/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CISCO-TNA (Cisco TNATIVE)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">132/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CISCO-SYS (Cisco SYSMAINT)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">133/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">STATSRV (Statistics Service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">134/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">INGRES-NET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">135/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        EPMAP (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Distributed_Computing_Environment&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Distributed Computing Environment (страница отсутствует)">DCE</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Distributed_Computing_Environment" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Distributed Computing Environment">
              <span title="Distributed Computing Environment — версия статьи «Distributed Computing Environment» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Endpoint Mapper)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">135/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        MSRPC (
        <a href="https://ru.wikipedia.org/wiki/Microsoft" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Microsoft">Microsoft</a>
        &nbsp;
        <a href="https://ru.wikipedia.org/wiki/Remote_procedure_call" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Remote procedure call">RPC</a>
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-6" rel="nofollow" style="color:rgb(11,0,128);background:none">[6]</a>
        </sup>
        )&nbsp;— используется в приложениях «клиент—сервер» Microsoft (например, Exchange)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">135/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        LOC-SRV (Locator service)&nbsp;— используется службами удалённого обслуживания (
        <a href="https://ru.wikipedia.org/wiki/DHCP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="DHCP">DHCP</a>
        ,&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Domain_Name_System" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Domain Name System">DNS</a>
        ,&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Windows_Internet_Name_Service" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Windows Internet Name Service">WINS</a>
        &nbsp;и&nbsp;т.&nbsp;д.)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">136/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PROFILE Naming System</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">137/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETBIOS-NS (
        <a href="https://ru.wikipedia.org/wiki/NetBIOS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NetBIOS">NetBIOS</a>
        &nbsp;Name Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">138/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETBIOS-DGM (
        <a href="https://ru.wikipedia.org/wiki/NetBIOS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NetBIOS">NetBIOS</a>
        &nbsp;Datagram Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">139/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETBIOS-SSN (
        <a href="https://ru.wikipedia.org/wiki/NetBIOS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NetBIOS">NetBIOS</a>
        &nbsp;Session Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">140/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">EMFIS-DATA (EMFIS Data Service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">141/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">EMFIS-CNTL (EMFIS Control Service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">142/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BL-IDM (Britton-Lee IDM)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">143/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IMAP (
        <a href="https://ru.wikipedia.org/wiki/Internet_Message_Access_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Internet Message Access Protocol">Internet Message Access Protocol</a>
        )&nbsp;— используется для получения и синхронизации сообщений электронной почты
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">144/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UMA (Universal Management Architecture)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">144/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NEWS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">145/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UAAC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">146/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ISO-TP0</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">147/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ISO-IP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">148/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">JARGON</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">148/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CRONUS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">149/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AED-512</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">150/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SQL-NET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">151/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HEMS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">152/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        BFTP (Background File Transfer Program)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-7" rel="nofollow" style="color:rgb(11,0,128);background:none">[7]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">153/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SGMP (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Simple_Gateway_Monitoring_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Simple Gateway Monitoring Protocol (страница отсутствует)">Simple Gateway Monitoring Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Simple_Gateway_Monitoring_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Simple Gateway Monitoring Protocol">
              <span title="Simple Gateway Monitoring Protocol — версия статьи «Simple Gateway Monitoring Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">154/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETSC-PROD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">155/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETSC-DEV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">156/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SQLSRV (
        <a href="https://ru.wikipedia.org/wiki/SQL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SQL">SQL</a>
        &nbsp;Service)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">157/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">KNET-CMP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">158/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PCMAIL-SRV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">158/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DMSP (Distributed Mail Service Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">159/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NSS-ROUTING</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">160/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SGMP-TRAPS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">161/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SNMP (
        <a href="https://ru.wikipedia.org/wiki/Simple_Network_Management_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Simple Network Management Protocol">Simple Network Management Protocol</a>
        )&nbsp;— используется как порт прослушивания агентами удалённого мониторинга
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">162/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SNMPTRAP (
        <a href="https://ru.wikipedia.org/wiki/Simple_Network_Management_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Simple Network Management Protocol">Simple Network Management Protocol</a>
        &nbsp;Trap)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-8" rel="nofollow" style="color:rgb(11,0,128);background:none">[8]</a>
        </sup>
        &nbsp;— используется как порт приёма асинхронных прерываний (traps)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">163/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CMIP-MAN (CMIP/TCP Manager)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">164/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CMIP-AGENT (CMIP/TCP Agent)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">165/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        XNS-COURIER (
        <a href="https://ru.wikipedia.org/wiki/Xerox_Network_Services" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Xerox Network Services">Xerox Network Services</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">166/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">S-NET (Sirius Systems Network)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">167/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NAMP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">168/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RSVD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">169/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SEND</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">170/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        PRINT-SRV (Network&nbsp;
        <a href="https://ru.wikipedia.org/wiki/PostScript" rel="nofollow" style="color:rgb(11,0,128);background:none" title="PostScript">PostScript</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">171/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MULTIPLEX (Network Innovations Multiplex)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">172/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CL-1 (Network Innovations CL/1); ранее&nbsp;— CL/1</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">173/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">XYPLEX-MUX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">174/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MAILQ</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">175/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VMNET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">176/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GENRAD-MUX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">177/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">XDMCP (X Display Manager Control Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">178/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NEXTSTEP (NextStep Window Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">179/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        BGP (
        <a href="https://ru.wikipedia.org/wiki/Border_Gateway_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Border Gateway Protocol">Border Gateway Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">180/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RIS (Intergraph)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">181/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UNIFY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">182/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AUDIT (Unisys Audit SITP)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">183/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OCBINDER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">184/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OCSERVER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">185/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">REMOTE-KIS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">186/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">KIS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">187/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ACI (Application Communication Interface)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">188/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MUMPS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">189/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">QFT (Queued File Transport)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">190/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GACP (Gateway Access Control Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">191/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PROSPERO (Prospero Directory Service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">192/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OSU-NMS (OSU Network Monitoring System)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">193/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SRMP (Spider Remote Monitoring Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">194/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IRC (
        <a href="https://ru.wikipedia.org/wiki/Internet_Relay_Chat" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Internet Relay Chat">Internet Relay Chat</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">195/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DN6-NLM-AUD (DNSIX Network Level Module Audit)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">196/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DN6-SMM-RED (DNSIX Session Mgt Module Audit Redir)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">197/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DLS (Directory Location Service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">198/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DLS-MON (Directory Location Service Monitor)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">199/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SMUX (
        <a href="https://ru.wikipedia.org/wiki/SNMP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SNMP">SNMP</a>
        &nbsp;Unix Multiplexer)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">200/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SRC (
        <a href="https://ru.wikipedia.org/wiki/IBM" rel="nofollow" style="color:rgb(11,0,128);background:none" title="IBM">IBM</a>
        &nbsp;System Resource Controller)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">201/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AT-RTMP (AppleTalk Routing Maintenance)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">202/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AT-NBP (AppleTalk Name Binding)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">203/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AT-3 (AppleTalk Unused)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">204/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AT-ECHO (AppleTalk Echo)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">205/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AT-5 (AppleTalk Unused)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">206/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AT-ZIS (AppleTalk Zone Information)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">207/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AT-7 (AppleTalk Unused)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">208/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AT-8 (AppleTalk Unused)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">209/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">QMTP (The Quick Mail Transfer Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">210/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Z39-50 (ANSI Z39.50)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">211/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">914C-G (Texas Instruments 914C/G Terminal)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">212/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ANET (ATEXSSTR)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">213/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/IPX" rel="nofollow" style="color:rgb(11,0,128);background:none" title="IPX">IPX</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">214/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VMPWSCS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">215/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SOFTPC (Insignia Solutions)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">216/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CALLIC (Computer Associates Int’l License Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">216/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ATLS (Access Technology License Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">217/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DBASE (dBASE Unix)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">218/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MPP (Message Posting Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">219/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UARPS (Unisys ARPs)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">220/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IMAP3 (Interactive Mail Access Protocol, version 3)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">221/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FLN-SPX (Berkeley rlogind with SPX auth)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">222/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RSH-SPX (Berkeley rshd with SPX auth)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">223/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CDC (Certificate Distribution Center)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">224/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MASQDIALER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">242/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DIRECT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">243/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SUR-MEAS (Survey Measurement)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">244/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">INBUSINESS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">245/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LINK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">246/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DSP3270 (Display Systems Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">247/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SUBNTBCST-TFTP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">248/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BHFHS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">249/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">250/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">251/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">252/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">253/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">254/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">255/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">256/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">256/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-SYNC (Checkpoint FW-1 state table sync)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">257/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SET (Secure Electronic Transaction)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">257/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-LOG (Checkpoint FW-1 log transfer)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">258/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-MC (Checkpoint FW-1 management console)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">258/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">YAK-CHAT (Yak Winsock Personal Chat)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">259/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ESRO-GEN (Efficient Short Remote Operations)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">259/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-RDP (Checkpoint FW-1 RDP)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">260/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OPENPORT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">260/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-SNMP (Checkpoint FW-1 SNMP agent)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">261/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NSIIOPS (IIOP Name Service over TLS/SSL)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">261/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-MGMT (Checkpoint FW-1 management)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">262/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ARCISDMS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">263/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HDAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">264/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        BGMP (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Border_Gateway_Multicast_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Border Gateway Multicast Protocol (страница отсутствует)">Border Gateway Multicast Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Border_Gateway_Multicast_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Border Gateway Multicast Protocol">
              <span title="Border Gateway Multicast Protocol — версия статьи «Border Gateway Multicast Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">264/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-TOPO (Checkpoint FW-1 topology download)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">265/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">X-BONE-CTL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">265/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-KEY (Checkpoint FW-1 public key transfer protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">266/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SST (SCSI on ST)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">267/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TD-SERVICE (Tobit David Service Layer)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">268/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TD-REPLICA (Tobit David Replica)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">269/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MANET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">270/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">270/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GIST (Q-mode encapsulation for GIST messages)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">271/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PT-TLS (IETF Network Endpoint Assessment/NEA Posture Transport Protocol over TLS)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">271/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">280/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HTTP-MGMT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">281/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PERSONAL-LINK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">282/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CABLEPORT-AX (Cable Port A/X)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">283/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RESCAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">284/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CORERJD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">286/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FXP (FXP Communication)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">287/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">K-BLOCK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">308/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NOVASTORBAKCUP (Novastor Backup)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">309/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ENTRUSTTIME</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">310/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BHMDS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">310/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в игре&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Delta_Force_(%D1%81%D0%B5%D1%80%D0%B8%D1%8F_%D0%B8%D0%B3%D1%80)" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Delta Force (серия игр)">Delta Force</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">311/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        ASIP-WEBADMIN (AppleShare IP WebAdmin), используется в&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Mac_OS_X_Server" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Mac OS X Server">Mac OS X Server</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">312/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VSLMP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">313/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MAGENTA-LOGIC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">314/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OPALIS-ROBOT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">315/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DPSI</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">316/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DECAUTH</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">317/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ZANNET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">318/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        PKIX-TIMESTAMP (PKIX&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Time_Stamp_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Time Stamp Protocol">Time Stamp Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">319/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PTP-EVENT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">320/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PTP-GENERAL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">321/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PIP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">322/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RTSPS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">323/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RPKI-RTR (Resource PKI to Router Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">323/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">323/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IMMP (Internet Message Mapping Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">324/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RPKI-RTR-TLS (Resource PKI to Router Protocol over TLS)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">324/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">333/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TEXAR (Texar Security Port)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">344/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PDAP (Prospero Data Access Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">345/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PAWSERV (Perf Analysis Workbench)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">346/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ZSERV (Zebra server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">347/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FATSERV (Fatmen Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">347/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в игре&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Operation_Flashpoint" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Operation Flashpoint">Operation Flashpoint</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">348/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CSI-SGWP (Cabletron Management Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">349/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MFTP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">350/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MATIP-TYPE-A (Mapping of Airline Traffic over Internet Protocol, Type A)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">351/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MATIP-TYPE-B (Mapping of Airline Traffic over Internet Protocol, Type B)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">351/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BHOETTY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">352/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DTAG-STE-SB</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">352/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BHOEDAP4</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">353/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NDSAUTH</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">354/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BH611</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">355/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DATEX-ASN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">356/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CLOANTO-NET-1</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">357/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BHEVENT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">358/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SHRINKWRAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">359/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NSRMP (Network Security Risk Management Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">360/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCOI2ODIALOG</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">361/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SEMANTIX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">362/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SRSSEND</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">363/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RSVP-TUNNEL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">364/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AURORA-CMGR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">365/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DTK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">366/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ODMR (On-Demand Mail Relay)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">367/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MORTGAGEWARE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">368/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">QBIKGDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">369/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RPC2PORTMAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">370/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CODAAUTH2</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">370/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SECURECAST1&nbsp;— использовался серверами&nbsp;
        <a href="https://ru.wikipedia.org/wiki/McAfee" rel="nofollow" style="color:rgb(11,0,128);background:none" title="McAfee">NAI</a>
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-9" rel="nofollow" style="color:rgb(11,0,128);background:none">[9]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">371/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CLEARCASE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">372/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ULISTPROC (ListProcessor)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">373/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LEGENT-1 (Legent Corporation)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">374/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LEGENT-2 (Legent Corporation)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">375/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HASSLE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">376/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NIP (Amiga Envoy Network Inquiry Proto)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">377/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TNETOS (NEC Corporation)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">378/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DSETOS (NEC Corporation)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">379/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IS99C (TIA/EIA/IS-99 modem client)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">380/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IS99S (TIA/EIA/IS-99 modem server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">381/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HP-COLLECTOR (
        <a href="https://ru.wikipedia.org/wiki/Hewlett-Packard" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Hewlett-Packard">Hewlett-Packard</a>
        &nbsp;performance data collector)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">382/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HP-MANAGED-NODE (
        <a href="https://ru.wikipedia.org/wiki/Hewlett-Packard" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Hewlett-Packard">Hewlett-Packard</a>
        &nbsp;performance data managed node)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">383/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HP-ALARM-MGR (
        <a href="https://ru.wikipedia.org/wiki/Hewlett-Packard" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Hewlett-Packard">Hewlett-Packard</a>
        &nbsp;data alarm manager)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">384/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ARNS (A Remote Network Server System)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">385/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IBM-APP (
        <a href="https://ru.wikipedia.org/wiki/IBM" rel="nofollow" style="color:rgb(11,0,128);background:none" title="IBM">IBM</a>
        &nbsp;Application)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">386/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ASA (ASA Message Router Object Def.)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">387/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AURP (AppleTalk Update-based Routing Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">388/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UNIDATA-LDM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">389/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        LDAP (
        <a href="https://ru.wikipedia.org/wiki/Lightweight_Directory_Access_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Lightweight Directory Access Protocol">Lightweight Directory Access Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">390/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UIS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">391/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SYNOTICS-RELAY (SynOptics SNMP Relay Port)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">392/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SYNOTICS-BROKER (SynOptics Port Broker Port)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">393/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">META5</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">394/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">EMBL-NDT (EMBL Nucleic Data Transfer)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">395/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETCP (NetScout Control Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">396/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETWARE-IP (Novell Netware over IP)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">397/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MPTN (Multi Protocol Trans. Net.)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">398/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">KRYPTOLAN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">399/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ISO-TSAP-C2 (ISO Transport Class 2 Non-Control over TCP)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">400/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OSB-SD (Oracle Secure Backup)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">401/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        UPS (
        <a href="https://ru.wikipedia.org/wiki/%D0%98%D1%81%D1%82%D0%BE%D1%87%D0%BD%D0%B8%D0%BA_%D0%B1%D0%B5%D1%81%D0%BF%D0%B5%D1%80%D0%B5%D0%B1%D0%BE%D0%B9%D0%BD%D0%BE%D0%B3%D0%BE_%D0%BF%D0%B8%D1%82%D0%B0%D0%BD%D0%B8%D1%8F" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Источник бесперебойного питания">Uninterruptible Power Supply</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">402/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GENIE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">402/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Altiris" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Altiris">Altiris</a>
        &nbsp;Deployment Client
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">403/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DECAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">404/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NCED</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">405/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NCLD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">406/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IMSP (Interactive Mail Support Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">407/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TIMBUKTU</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">408/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PRM-SM (Prospero Resource Manager&nbsp;— System Management)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">409/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PRM-NM (Prospero Resource Manager&nbsp;— Node Management)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">410/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DECLADEBUG (DECLadebug Remote Debug Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">411/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RMT (Remote MT Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">411/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Direct_Connect" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Direct Connect">Direct Connect</a>
        &nbsp;Hub
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">412/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SYNOPTICS-TRAP (Trap Convention Port)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">412/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Direct_Connect" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Direct Connect">Direct Connect</a>
        &nbsp;Client-to-Client
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">413/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SMSP (Storage Management Services Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">414/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">INFOSEEK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">415/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BNET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">416/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SILVERPLATTER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">417/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ONMUX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">418/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HYPER-G</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">419/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ARIEL1</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">420/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SMPTE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">421/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ARIEL2</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">422/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ARIEL3</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">423/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OPC-JOB-START (IBM Operations Planning and Control Start)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">424/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OPC-JOB-TRACK (IBM Operations Planning and Control Track)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">425/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ICAD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">426/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SMARTDSP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">427/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SVRLOC (SLP,&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Service_Location_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Service Location Protocol">Service Location Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">428/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OCS-CMU</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">429/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OCS-AMU</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">430/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UTMPSD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">431/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UTMPCD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">432/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IASD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">433/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NNSP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">434/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MOBILEIP-AGENT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">435/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MOBILIP-MN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">436/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DNA-CML</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">437/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">COMSCM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">438/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DSFGW</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">439/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DASP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">440/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SGCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">441/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DECVMS-SYSMGT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">442/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CVC-HOSTD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">443/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HTTPS (
        <a href="https://ru.wikipedia.org/wiki/HTTPS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="HTTPS">HyperText Transfer Protocol Secure</a>
        )&nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/HTTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="HTTP">HTTP</a>
        &nbsp;с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">443/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">использовался в различных играх</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">444/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SNPP (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Simple_Network_Paging_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Simple Network Paging Protocol (страница отсутствует)">Simple Network Paging Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Simple_Network_Paging_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Simple Network Paging Protocol">
              <span title="Simple Network Paging Protocol — версия статьи «Simple Network Paging Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-10" rel="nofollow" style="color:rgb(11,0,128);background:none">[10]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">445/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        MICROSOFT-DS&nbsp;— используется в Microsoft Windows 2000 и поздних версий для прямого TCP/IP-доступа без использования&nbsp;
        <a href="https://ru.wikipedia.org/wiki/NetBIOS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NetBIOS">NetBIOS</a>
        &nbsp;(например, в&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Active_Directory" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Active Directory">Active Directory</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">446/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DDM-RDB (DDM-Remote Relational Database Access)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">447/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DDM-DFM (DDM-Distributed File Management)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">448/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DDM-SSL (DDM-Remote DB Access Using Secure Sockets)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">449/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AS-SERVERMAP (AS Server Mapper)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">450/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TSERVER (Computer Supported Telecomunication Applications)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">451/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SFS-SMP-NET (Cray Network Semaphore server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">452/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SFS-CONFIG (Cray SFS config server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">453/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CREATIVESERVER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">454/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CONTENTSERVER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">455/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CREATIVEPARTNR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">456/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MACON-TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">456/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MACON-UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">457/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCOHELP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">458/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">APPLEQTC (Apple QuickTime Conferencing)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">459/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AMPR-RCMD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">460/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SKRONK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">461/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DATASURFSRV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">462/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DATASURFSRVSEC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">463/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ALPES</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">464/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        KPASSWD (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;Change/Set password)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">465/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">URD (URL Rendezvous Directory), для Cisco Source Specific Multicast (SSM)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">465/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IGMPV3LITE (
        <a href="https://ru.wikipedia.org/wiki/IGMP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="IGMP">IGMP</a>
        &nbsp;Version 3 Lite), для Cisco Source Specific Multicast (SSM)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">465/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SMTPS (Simple Mail Transfer Protocol Secure)&nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SMTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SMTP">SMTP</a>
        &nbsp;с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">466/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DIGITAL-VRC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">467/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MYLEX-MAPD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">468/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PHOTURIS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">469/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RCP (Radio Control Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">470/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCX-PROXY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">471/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MONDEX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">472/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LJK-LOGIN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">473/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HYBRID-POP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">474/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TN-TL-W1</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">475/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        TCPNETHASPSRV (
        <a href="https://ru.wikipedia.org/wiki/HASP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="HASP">HASP</a>
        &nbsp;services, TCP/IP version)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">476/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TN-TL-FD1</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">477/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SS7NS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">478/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SPSC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">479/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IAFDBASE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">480/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IAFDBASE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">481/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PH (Ph service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">481/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DVS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">482/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BGS-NSI</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">483/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ULPNET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">484/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">INTEGRA-SME</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">485/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">POWERBURST</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">486/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AVIAN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">487/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SAFT (Simple Asynchronous File Transfer)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">488/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GSS-HTTP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">489/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NEST-PROTOCOL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">490/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MICOM-PFS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">491/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GO-LOGIN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">492/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TICF-1 (Transport Independent Convergence for FNA)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">493/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TICF-2 (Transport Independent Convergence for FNA)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">494/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">POV-RAY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">495/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">INTECOURIER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">496/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PIM-RP-DISC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">497/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RETROSPECT&nbsp;— для службы архивации и восстановления&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Retrospect" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Retrospect">Retrospect</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">498/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SIAM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">499/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ISO-ILL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">500/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        ISAKMP (
        <span>
          <a href="https://ru.wikipedia.org/wiki/ISAKMP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="ISAKMP">Internet Security Association and Key Management Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://ru.wikipedia.org/wiki/%D0%A8%D0%B0%D0%B1%D0%BB%D0%BE%D0%BD:%D0%9D%D0%B5_%D0%BF%D0%B5%D1%80%D0%B5%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%BE_5#%D0%95%D1%81%D0%BB%D0%B8_%D1%81%D1%82%D1%80%D0%B0%D0%BD%D0%B8%D1%86%D0%B0_%D1%81%D1%83%D1%89%D0%B5%D1%81%D1%82%D0%B2%D1%83%D0%B5%D1%82" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Шаблон:Не переведено 5">
              <span style="color:red;font-weight:bold" title="Уберите шаблон «Не переведено 5» из статьи и замените его простой вики-ссылкой">?!</span>
            </a>
          </sup>
        </span>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">500/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">использовался Vodafone Sure Signal и некоторыми приложениями Apple</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">501/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">STMF</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">502/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ASA-APPL-PROTO</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">502/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Modbus" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Modbus">Modbus</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">503/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">INTRINSA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">504/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CITADEL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">505/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MAILBOX-LM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">506/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OHIMSRV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">507/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CRS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">508/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">XVTTP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">509/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SNARE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">510/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FCP (FirstClass Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">511/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PASSGO</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">512/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">EXEC (Remote Process Execution)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">512/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        COMSAT (аутентификация с использованием паролей и UNIX-логинов);
        <br>
        BIFF (используется системой электронной почты для уведомления пользователей о новых сообщениях, см.&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Biff&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Biff (страница отсутствует)">biff</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/biff" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:biff">
              <span title="biff — версия статьи «Biff» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        ; в настоящее время получает сообщения только от процессов, выполняющихся на той же машине)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">513/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        LOGIN&nbsp;— удаленный вход наподобие&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Telnet" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Telnet">Telnet</a>
        ; автоматическая проверка подлинности выполняется на основе номеров привилегированных портов и распределённых баз данных, которые идентифицируют «домены аутентификации»
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">513/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">WHO&nbsp;— поддержка базы данных открытых сеансов на машинах в локальной сети</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">514/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SHELL&nbsp;— для выполнения команд на удалённой системе; используется в аналогах командной строки с автоматической аутентификацией (например,&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Rsh&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Rsh (страница отсутствует)">rsh</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Remote_Shell" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Remote Shell">
              <span title="Remote Shell — версия статьи «Rsh» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        ,&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Rcp&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Rcp (страница отсутствует)">rcp</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/rcp_(Unix)" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:rcp (Unix)">
              <span title="rcp (Unix) — версия статьи «Rcp» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">514/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Syslog" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Syslog">SYSLOG</a>
        &nbsp;— доставка сообщений о происходящих в системе событиях
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-11" rel="nofollow" style="color:rgb(11,0,128);background:none">[11]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">515/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        PRINTER&nbsp;— для служб печати, ожидающих входящие соединения (например,&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Line_Printer_Daemon" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Line Printer Daemon">Line Printer Daemon</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">516/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VIDEOTEX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">517/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TALK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">518/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NTALK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">519/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UTIME</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">520/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">EFS (Extended Filename Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">520/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        ROUTER&nbsp;— локальный процесс маршрутизации; используется разновидность протокола Xerox NS&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Routing_Information_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Routing Information Protocol">RIP</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">521/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RPING</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">522/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ULP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">523/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IBM-DB2</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">524/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NCP (
        <a href="https://ru.wikipedia.org/wiki/NetWare_Core_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NetWare Core Protocol">NetWare Core Protocol</a>
        )&nbsp;— используется, например, для доступа к ресурсам главного сервера NetWare, синхронизации времени и&nbsp;т.&nbsp;д.
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">525/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TIMED</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">526/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TEMPO</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">527/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">STX (Stock IXChange)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">528/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CUSTIX (Customer IXChange)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">529/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IRC-SERV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">530/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        COURIER (
        <a href="https://ru.wikipedia.org/wiki/Remote_procedure_call" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Remote procedure call">RPC</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">531/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CONFERENCE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">531/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AOL Instant Messenger, IRC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">532/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETNEWS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">533/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETWALL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">534/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">WINDREAM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">535/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IIOP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">536/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OPALIS-RDV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">537/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NMSP (Networked Media Streaming Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">538/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GDOMAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">539/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">APERTUS-LDP (Apertus Technologies Load Determination)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">540/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        UUCP (
        <a href="https://ru.wikipedia.org/wiki/Uucp" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Uucp">Unix-to-Unix Copy Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">541/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        UUCP-RLOGIN (
        <a href="https://ru.wikipedia.org/wiki/Uucp" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Uucp">Unix-to-Unix Copy Protocol</a>
        &nbsp;Remote Login)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">542/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">COMMERCE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">543/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        KLOGIN (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;login)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">544/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        KSHELL (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;remote shell)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">545/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">APPLEQTCSRVR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">546/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DHCPV6-CLIENT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">547/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DHCPV6-SERVER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">548/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        AFPOVERTCP (
        <a href="https://ru.wikipedia.org/wiki/Apple_Filing_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Apple Filing Protocol">Apple Filing Protocol</a>
        &nbsp;over&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TCP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TCP">TCP</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">549/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IDFP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">550/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NEW-RWHO</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">551/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        CYBERCASH (CyberCash Credit Card Protocol)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-12" rel="nofollow" style="color:rgb(11,0,128);background:none">[12]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">552/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DEVSHR-NTS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">553/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PIRP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">554/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RTSP (
        <a href="https://ru.wikipedia.org/wiki/Real_Time_Streaming_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Real Time Streaming Protocol">Real Time Streaming Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">555/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DSF</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">556/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        REMOTEFS (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Remote_File_Sharing&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Remote File Sharing (страница отсутствует)">Remote File Sharing</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Remote_File_Sharing" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Remote File Sharing">
              <span title="Remote File Sharing — версия статьи «Remote File Sharing» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Server)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">557/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OPENVMS-SYSIPC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">558/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SDNSKMP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">559/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TEEDTAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">560/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RMONITOR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">561/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MONITOR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">562/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CHSHELL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">563/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NNTPS (Network News Transfer Protocol Secure)&nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/NNTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NNTP">NNTP</a>
        &nbsp;с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">564/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">9PFS (Plan 9 File Service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">565/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">WHOAMI</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">566/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">STREETTALK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">567/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BANYAN-RPC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">568/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MS-SHUTTLE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">569/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MS-ROME</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">570/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">METER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">571/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UMETER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">572/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SONAR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">573/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BANYAN-VIP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">574/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FTP-AGENT (FTP Software Agent System)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">575/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VEMMI</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">576/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IPCD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">577/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VNAS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">578/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IPDD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">579/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DECBSRV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">580/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SNTP-HEARTBEAT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">581/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BDP (Bundle Discovery Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">582/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCC-SECURITY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">583/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PHILIPS-VC (Philips Video-Conferencing)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">584/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">KEYSERVER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">585/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободно; ранее&nbsp;— IMAP4-SSL (см. порт 993)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">586/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PASSWORD-CHG (Password Change)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">587/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SUBMISSION (Message Submission for Mail
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-13" rel="nofollow" style="color:rgb(11,0,128);background:none">[13]</a>
        </sup>
        )&nbsp;— используется (
        <a href="https://ru.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Simple Mail Transfer Protocol">SMTP</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">588/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CAL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">589/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">EYELINK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">590/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TNS-CML</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">591/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HTTP-ALT (HTTP Alternate, см. порт 80)&nbsp;— используется программой&nbsp;
        <a href="https://ru.wikipedia.org/wiki/FileMaker" rel="nofollow" style="color:rgb(11,0,128);background:none" title="FileMaker">FileMaker</a>
        &nbsp;начиная с версии 6.0
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">592/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">EUDORA-SET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">593/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        HTTP-RPC-EPMAP (
        <a href="https://ru.wikipedia.org/wiki/Remote_procedure_call" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Remote procedure call">RPC</a>
        &nbsp;посредством&nbsp;
        <a href="https://ru.wikipedia.org/wiki/HTTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="HTTP">HTTP</a>
        )&nbsp;— используется, например, службами&nbsp;
        <a href="https://ru.wikipedia.org/wiki/DCOM" rel="nofollow" style="color:rgb(11,0,128);background:none" title="DCOM">DCOM</a>
        &nbsp;и&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Microsoft_Exchange_Server" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Microsoft Exchange Server">Microsoft Exchange Server</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">594/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TPIP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">595/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CAB-PROTOCOL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">596/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SMSD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">597/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PTCNAMESERVICE (PTC Name Service)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">598/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCO-WEBSRVRMG3 (SCO Web Server Manager 3)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">599/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ACP (Aeolon Core Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">600/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IPCSERVER (Sun IPC server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">601/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SYSLOG-CONN&nbsp;— используется Reliable&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Syslog" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Syslog">Syslog</a>
        &nbsp;Service (служба надёжной доставки сообщений о происходящих в системе событиях с использованием&nbsp;
        <a href="https://ru.wikipedia.org/wiki/XML" rel="nofollow" style="color:rgb(11,0,128);background:none" title="XML">XML</a>
        -схем протокола&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Blocks_Extensible_Exchange_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Blocks Extensible Exchange Protocol (страница отсутствует)">BEEP</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/BEEP" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:BEEP">
              <span title="BEEP — версия статьи «Blocks Extensible Exchange Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-14" rel="nofollow" style="color:rgb(11,0,128);background:none">[14]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">602/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        XMLRPC-BEEP (XML-RPC посредством&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Blocks_Extensible_Exchange_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Blocks Extensible Exchange Protocol (страница отсутствует)">BEEP</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/BEEP" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:BEEP">
              <span title="BEEP — версия статьи «Blocks Extensible Exchange Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-15" rel="nofollow" style="color:rgb(11,0,128);background:none">[15]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">603/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IDXP (Intrusion Detection Exchange Protocol)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-16" rel="nofollow" style="color:rgb(11,0,128);background:none">[16]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">604/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        TUNNEL&nbsp;— используется для туннелирования протокола&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Blocks_Extensible_Exchange_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Blocks Extensible Exchange Protocol (страница отсутствует)">BEEP</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/BEEP" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:BEEP">
              <span title="BEEP — версия статьи «Blocks Extensible Exchange Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;на прикладном уровне
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-17" rel="nofollow" style="color:rgb(11,0,128);background:none">[17]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">605/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SOAP-BEEP&nbsp;— используется для передачи сообщений&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SOAP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SOAP">SOAP</a>
        &nbsp;посредством протокола&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Blocks_Extensible_Exchange_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Blocks Extensible Exchange Protocol (страница отсутствует)">BEEP</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/BEEP" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:BEEP">
              <span title="BEEP — версия статьи «Blocks Extensible Exchange Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-18" rel="nofollow" style="color:rgb(11,0,128);background:none">[18]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">606/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">URM (Cray Unified Resource Manager)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">607/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NQS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">607/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в играх&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Operation_Flashpoint" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Operation Flashpoint">Operation Flashpoint</a>
        ,&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Railroad_Tycoon_3" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Railroad Tycoon 3">Railroad Tycoon 3</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">608/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SIFT-UFT (Sender-Initiated/Unsolicited File Transfer)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">609/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NPMP-TRAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">610/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NPMP-LOCAL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">611/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NPMP-GUI</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">612/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HMMP-IND (HMMP Indication)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">613/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HMMP-OP (HMMP Operation)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">614/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SSHELL (
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;shell)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">615/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCO-INETMGR (SCO Internet Configuration Manager)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">616/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCO-SYSMGR (SCO System Administration Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">617/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCO-DTMGR (SCO Desktop Administration Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">618/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DEI-ICDA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">619/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">COMPAQ-EVM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">620/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SCO-WEBSRVRMGR (SCO WebServer Manager)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">621/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ESCP-IP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">622/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">COLLABORATOR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">623/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OOB-WS-HTTP (DMTF out-of-band web services management protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">623/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ASF-RMCP (ASF Remote Management and Control Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">624/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CRYPTOADMIN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">625/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DEC-DLM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">626/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ASIA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">627/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PASSGO-TIVOLI</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">628/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">QMQP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">629/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">3COM-AMP3</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">630/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RDA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">631/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IPP (
        <a href="https://ru.wikipedia.org/wiki/Internet_Printing_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Internet Printing Protocol">Internet Printing Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">632/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BMPP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">633/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SERVSTAT (Service Status update)&nbsp;— для Sterling Software</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">634/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GINAD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">635/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RLZDBASE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">636/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        LDAPS (Lightweight Directory Access Protocol Secure)&nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/LDAP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="LDAP">LDAP</a>
        &nbsp;с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">637/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LANSERVER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">638/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MCNS-SEC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">639/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        MSDP (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Multicast_Source_Discovery_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Multicast Source Discovery Protocol (страница отсутствует)">Multicast Source Discovery Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Multicast_Source_Discovery_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Multicast Source Discovery Protocol">
              <span title="Multicast Source Discovery Protocol — версия статьи «Multicast Source Discovery Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">640/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ENTRUST-SPS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">640/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PCNFS (PC-NFS DOS Authentication)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">641/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">REPCMD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">642/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ESRO-EMSDP (v1.3)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">643/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SANITY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">644/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DWR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">645/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PSSC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">646/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        LDP (
        <a href="https://ru.wikipedia.org/wiki/Label_Distribution_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Label Distribution Protocol">Label Distribution Protocol</a>
        )&nbsp;— используется для маршрутизации в сетях&nbsp;
        <a href="https://ru.wikipedia.org/wiki/MPLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="MPLS">MPLS</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">647/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        DHCP-FAILOVER (
        <a href="https://ru.wikipedia.org/wiki/DHCP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="DHCP">DHCP</a>
        &nbsp;
        <a href="https://ru.wikipedia.org/wiki/Failover" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Failover">Failover</a>
        )
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-DHCP-FAILOVER-19" rel="nofollow" style="color:rgb(11,0,128);background:none">[19]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">648/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RRP (Registry Registrar Protocol)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-20" rel="nofollow" style="color:rgb(11,0,128);background:none">[20]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">649/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CADVIEW-3D</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">650/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OBEX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">651/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IEEE-MMS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">652/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HELLO-PORT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">652/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DTCP (Dynamic Tunnel Configuration Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">653/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">REPSCMD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">654/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        AODV (
        <a href="https://ru.wikipedia.org/wiki/Ad-hoc_On-demand_Distance_Vector" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Ad-hoc On-demand Distance Vector">Ad-hoc On-demand Distance Vector</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">655/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TINC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">656/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SPMP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">657/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RMC (Remote monitoring and Control)&nbsp;— используется в системах&nbsp;
        <a href="https://ru.wikipedia.org/wiki/IBM" rel="nofollow" style="color:rgb(11,0,128);background:none" title="IBM">IBM</a>
        &nbsp;(
        <a href="https://ru.wikipedia.org/wiki/AIX" rel="nofollow" style="color:rgb(11,0,128);background:none" title="AIX">AIX</a>
        &nbsp;Integrated Virtualization Manager
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-21" rel="nofollow" style="color:rgb(11,0,128);background:none">[21]</a>
        </sup>
        ,&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Hardware_Management_Console&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Hardware Management Console (страница отсутствует)">Hardware Management Console</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/IBM_Hardware_Management_Console" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:IBM Hardware Management Console">
              <span title="IBM Hardware Management Console — версия статьи «Hardware Management Console» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        ) для динамической конфигурации&nbsp;
        <a href="https://ru.wikipedia.org/wiki/LPAR" rel="nofollow" style="color:rgb(11,0,128);background:none" title="LPAR">управляемых логических разделов</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">658/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TENFOLD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">659/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">URL-RENDEZVOUS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">660/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MAC-SRVR-ADMIN (Mac OS X Server administration)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">661/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">662/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PFTP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">663/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PURENOISE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">664/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OOB-WS-HTTPS (DMTF out-of-band secure web services management protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">664/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ASF-SECURE-RMCP (ASF Secure Remote Management and Control Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">665/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SUN-DR (SUN Remote Dynamic Reconfiguration)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">666/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        MDQS;
        <br>
        DOOM&nbsp;— использовался в играх&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Doom_(%D0%B8%D0%B3%D1%80%D0%B0,_1993)" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Doom (игра, 1993)">Doom</a>
        ,&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Doom_2" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Doom 2">Doom 2</a>
        &nbsp;компании&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Id_Software" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Id Software">id Software</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">667/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DISCLOSE (campaign contribution disclosures, SDR Technologies)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">668/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MECOMM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">669/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MEREGISTER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">670/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VACDSM-SWS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">671/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VACDSM-APP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">672/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VPPS-QUA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">673/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CIMPLEX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">674/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        ACAP (
        <a href="https://ru.wikipedia.org/wiki/Application_Configuration_Access_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Application Configuration Access Protocol">Application Configuration Access Protocol</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">675/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DCTP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">676/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VPPS-VIA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">677/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VPP (Virtual Presence Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">678/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GGF-NCP (GNU Generation Foundation NCP)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">679/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MRM</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">680/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ENTRUST-AAAS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">681/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ENTRUST-AAMS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">682/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">XFR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">683/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CORBA-IIOP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">684/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CORBA-IIOP-SSL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">685/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MDC-PortMapper</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">686/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HCP-Wismar (Hardware Control Protocol Wismar)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">687/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ASIPREGISTRY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">688/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">REALM-RUSD (ApplianceWare managment protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">689/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NMAP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">690/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VATP (Velazquez Application Transfer Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">691/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        MSEXCH-ROUTING (
        <a href="https://ru.wikipedia.org/wiki/Microsoft_Exchange_Server" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Microsoft Exchange Server">Microsoft Exchange Server</a>
        &nbsp;Routing)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">692/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Hyperwave-ISP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">693/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CONNENDP (almanid Connection Endpoint)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">694/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">HA-CLUSTER (Linux High Availability Cluster heartbeat)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">695/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IEEE-MMS-SSL (
        <a href="https://ru.wikipedia.org/wiki/IEEE" rel="nofollow" style="color:rgb(11,0,128);background:none" title="IEEE">IEEE</a>
        &nbsp;Media Management System over&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        )
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-22" rel="nofollow" style="color:rgb(11,0,128);background:none">[22]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">696/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RUSHD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">697/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UUIDGEN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">698/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        OLSR (
        <a href="https://ru.wikipedia.org/wiki/OLSR" rel="nofollow" style="color:rgb(11,0,128);background:none" title="OLSR">Optimized Link-State Routing</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">699/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ACCESSNETWORK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">700/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        EPP (
        <a href="https://ru.wikipedia.org/wiki/Extensible_Provisioning_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Extensible Provisioning Protocol">Extensible Provisioning Protocol</a>
        )
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-23" rel="nofollow" style="color:rgb(11,0,128);background:none">[23]</a>
        </sup>
        &nbsp;— используется для управления регистрационной информацией&nbsp;
        <a href="https://ru.wikipedia.org/wiki/DNS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="DNS">DNS</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">701/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        LMP (Link Management Protocol)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-24" rel="nofollow" style="color:rgb(11,0,128);background:none">[24]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">702/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IRIS-BEEP (IRIS over BEEP)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-25" rel="nofollow" style="color:rgb(11,0,128);background:none">[25]</a>
        </sup>
        &nbsp;— используется для передачи сообщений IRIS (Internet Registry Information Service)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-26" rel="nofollow" style="color:rgb(11,0,128);background:none">[26]</a>
        </sup>
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-27" rel="nofollow" style="color:rgb(11,0,128);background:none">[27]</a>
        </sup>
        посредством протокола&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Blocks_Extensible_Exchange_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Blocks Extensible Exchange Protocol (страница отсутствует)">BEEP</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/BEEP" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:BEEP">
              <span title="BEEP — версия статьи «Blocks Extensible Exchange Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">703/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">704/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ELCSD (errlog copy/server daemon)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">705/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">AGENTX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">706/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SILC (
        <a href="https://ru.wikipedia.org/wiki/Secure_Internet_Live_Conferencing" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Secure Internet Live Conferencing">Secure Internet Live Conferencing</a>
        )&nbsp;— для организации безопасных аудио- и видеоконференций
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">707/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BORLAND-DSJ</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">708/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">709/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ENTRUST-KMSH</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">710/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ENTRUST-ASH</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">711/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        CISCO-TDP (
        <a href="https://ru.wikipedia.org/wiki/Cisco" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Cisco">Cisco</a>
        &nbsp;Tag Distribution Protocol)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-28" rel="nofollow" style="color:rgb(11,0,128);background:none">[28]</a>
        </sup>
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-29" rel="nofollow" style="color:rgb(11,0,128);background:none">[29]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">712/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        TBRPF (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=TBRPF&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="TBRPF (страница отсутствует)">Topology Broadcast based on Reverse-Path Forwarding routing protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Topology_dissemination_based_on_reverse-path_forwarding" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Topology dissemination based on reverse-path forwarding">
              <span title="Topology dissemination based on reverse-path forwarding — версия статьи «TBRPF» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-30" rel="nofollow" style="color:rgb(11,0,128);background:none">[30]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">712/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">используется Promise RAID Controller</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">713/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IRIS-XPC (IRIS over XPC)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">713/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IRIS-XPCS (IRIS over XPCS)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">715/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IRIS-LWZ</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">716/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PANA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">720/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SMQP (Simple Message Queue Protocol)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">729/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETVIEWDM1 (IBM NetView DM/6000 Server/Client)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">730/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETVIEWDM2 (IBM NetView DM/6000 send/tcp)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">731/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETVIEWDM3 (IBM NetView DM/6000 receive/tcp)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">732—740</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободны</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">741/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETGW</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">742/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NETRCS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">743/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">744/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FLEXLM (Flexible License Manager)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">745/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">746/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">747/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FUJITSU-DEV (Fujitsu Device Control)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">748/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RIS-CM (Russell Info Sci Calendar Manager)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">749/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        KERBEROS-ADM (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;administration)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">750/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RFILE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">750/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">750/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">LOADAV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">750/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        KERBEROS-IV (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;version IV)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">751/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PUMP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">751/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        kerberos_master (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;authentication)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">752/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">QRH</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">752/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        passwd_server (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;password server)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">753/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RRH (Reverse Routing Header)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-31" rel="nofollow" style="color:rgb(11,0,128);background:none">[31]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">753/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        userreg_server (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;user registration server)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">754/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">TELL</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">754/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        krb5_prop (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;v5 slave propagation)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">755/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">756/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">757/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">758/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NLOGIN</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">759/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CON</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">760/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">760/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        krbupdate, kreg (
        <a href="https://ru.wikipedia.org/wiki/Kerberos" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Kerberos">Kerberos</a>
        &nbsp;registration)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">761/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RXE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">762/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">QUOTAD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">763/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CYCLESERV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">764/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OMSERV</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">765/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">WEBSTER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">766/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">767/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PHONEBOOK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">768/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">769/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VID</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">770/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CADLOCK</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">771/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RTIP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">772/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CYCLESERV2</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">773/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SUBMIT</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">773/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">NOTIFY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">774/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">RPASSWD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">774/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ACMAINT-DBD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">775/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ENTOMB</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">775/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ACMAINT-TRANSD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">776/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">WPAGES</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">777/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Multiling-HTTP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">778/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">779/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободен</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">780/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">WPGS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">782/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        используется&nbsp;
        <a href="http://www.conserver.com/" rel="nofollow" style="color:rgb(102,51,102);background:linear-gradient(transparent,transparent) right center no-repeat,url(&quot;&quot;);padding-right:13px">Conserver</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">783/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        используется&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SpamAssassin" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SpamAssassin">SpamAssassin</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">800/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MDBS-DAEMON</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">801/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">DEVICE</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">803/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        Agnitum&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Outpost_Firewall" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Outpost Firewall">Outpost Firewall</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">810/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">810/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FCP-UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">828/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ITM-MCELL-S</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">829/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PKIX-3-CA-RA</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">829/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        CMP (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Certificate_Management_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Certificate Management Protocol (страница отсутствует)">Certificate Management Protocol</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Certificate_Management_Protocol" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Certificate Management Protocol">
              <span title="Certificate Management Protocol — версия статьи «Certificate Management Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">830/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETCONF-SSH (NETCONF over SSH)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-32" rel="nofollow" style="color:rgb(11,0,128);background:none">[32]</a>
        </sup>
        &nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/NETCONF" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NETCONF">NETCONF</a>
        &nbsp;через&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSH" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSH">SSH</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">831/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETCONF-BEEP (NETCONF over BEEP)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-33" rel="nofollow" style="color:rgb(11,0,128);background:none">[33]</a>
        </sup>
        &nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/NETCONF" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NETCONF">NETCONF</a>
        &nbsp;через&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Blocks_Extensible_Exchange_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Blocks Extensible Exchange Protocol (страница отсутствует)">BEEP</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/BEEP" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:BEEP">
              <span title="BEEP — версия статьи «Blocks Extensible Exchange Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">832/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETCONFSOAPHTTP (NETCONF for SOAP over HTTPS)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-RFC4743-34" rel="nofollow" style="color:rgb(11,0,128);background:none">[34]</a>
        </sup>
        &nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/NETCONF" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NETCONF">NETCONF</a>
        &nbsp;через&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SOAP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SOAP">SOAP</a>
        &nbsp;и&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSH" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSH">SSH</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">833/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NETCONFSOAPBEEP (NETCONF for SOAP over BEEP)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-RFC4743-34" rel="nofollow" style="color:rgb(11,0,128);background:none">[34]</a>
        </sup>
        &nbsp;—&nbsp;
        <a href="https://ru.wikipedia.org/wiki/NETCONF" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NETCONF">NETCONF</a>
        &nbsp;через&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SOAP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SOAP">SOAP</a>
        &nbsp;и&nbsp;
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Blocks_Extensible_Exchange_Protocol&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Blocks Extensible Exchange Protocol (страница отсутствует)">BEEP</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/BEEP" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:BEEP">
              <span title="BEEP — версия статьи «Blocks Extensible Exchange Protocol» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">834—846</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободны</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">847/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        DHCP-FAILOVER2 (
        <a href="https://ru.wikipedia.org/wiki/DHCP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="DHCP">DHCP</a>
        &nbsp;
        <a href="https://ru.wikipedia.org/wiki/Failover" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Failover">Failover</a>
        )
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-DHCP-FAILOVER-19" rel="nofollow" style="color:rgb(11,0,128);background:none">[19]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">848/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        GDOI (Group Domain of Interpretation)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-35" rel="nofollow" style="color:rgb(11,0,128);background:none">[35]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">849—859</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободны</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">860/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        ISCSI (Internet Small Computer Systems Interface)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-36" rel="nofollow" style="color:rgb(11,0,128);background:none">[36]</a>
        </sup>
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-37" rel="nofollow" style="color:rgb(11,0,128);background:none">[37]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">861/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        OWAMP-CONTROL (One-way Active Measurement Protocol Control)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-38" rel="nofollow" style="color:rgb(11,0,128);background:none">[38]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">862/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        TWAMP-CONTROL (Two-way Active Measurement Protocol Control)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-39" rel="nofollow" style="color:rgb(11,0,128);background:none">[39]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">863—872</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободны</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">873/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        RSYNC (Remote Synchronization)&nbsp;— используется&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Rsync" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Rsync">rsync</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">874—885</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">свободны</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">886/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ICLCNET-LOCATE (ICL coNETion locate server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">887/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ICLCNET-SVINFO (ICL coNETion server info)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">888/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ACCESSBUILDER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">888/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        jouflay (
        <a href="https://ru.wikipedia.org/wiki/CDDB" rel="nofollow" style="color:rgb(11,0,128);background:none" title="CDDB">CDDB</a>
        &nbsp;Protocol)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">897/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Brocade_Communications_Systems" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Brocade Communications Systems">Brocade</a>
        &nbsp;SMI-S RPC
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">898/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/Brocade_Communications_Systems" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Brocade Communications Systems">Brocade</a>
        &nbsp;SMI-S RPC с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">900/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">OMGINITIALREFS</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">901/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">FW1-CLNTAUTH-HTTP (Checkpoint FW-1/VPN-1 client auth over http)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">901/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в играх серии&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Command_%26_Conquer" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Command &amp; Conquer">Command &amp; Conquer</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">901/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SMPNAMERES</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">901/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/VMware" rel="nofollow" style="color:rgb(11,0,128);background:none" title="VMware">VMware</a>
        &nbsp;Virtual Infrastructure Client (для связи от управляемого устройства к консоли)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">901/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        SWAT (
        <a href="https://ru.wikipedia.org/wiki/Samba" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Samba">Samba</a>
        &nbsp;Web Administration Tool)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">901/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ISS RealSecure (приёмный порт датчика)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">902/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IDEAFARM-DOOR</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">902/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/VMware" rel="nofollow" style="color:rgb(11,0,128);background:none" title="VMware">VMware</a>
        &nbsp;Infrastructure Client
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-vmware1-40" rel="nofollow" style="color:rgb(11,0,128);background:none">[40]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">902/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/VMware" rel="nofollow" style="color:rgb(11,0,128);background:none" title="VMware">VMware</a>
        &nbsp;Server Console (для связи от консоли управления к устройству)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-41" rel="nofollow" style="color:rgb(11,0,128);background:none">[41]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">902/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ISS RealSecure</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">903/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">IDEAFARM-PANIC</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">903/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ISS Console Manager</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">903/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/VMware" rel="nofollow" style="color:rgb(11,0,128);background:none" title="VMware">VMware</a>
        &nbsp;Remote Console
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-vmware1-40" rel="nofollow" style="color:rgb(11,0,128);background:none">[40]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">904/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <a href="https://ru.wikipedia.org/wiki/VMware" rel="nofollow" style="color:rgb(11,0,128);background:none" title="VMware">VMware</a>
        &nbsp;Server Alternate (если занят порт 902)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">910/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        KINK (Kerberized Internet Negotiation of Keys)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-42" rel="nofollow" style="color:rgb(11,0,128);background:none">[42]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">911/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">XACT-BACKUP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">911/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался Network Console on Acid (NCA) для локального перенаправления с использованием&nbsp;
        <a href="https://ru.wikipedia.org/wiki/OpenSSH" rel="nofollow" style="color:rgb(11,0,128);background:none" title="OpenSSH">OpenSSH</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">912/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        APEX-MESH (Application Exchange relay to relay service)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-RFC3340-43" rel="nofollow" style="color:rgb(11,0,128);background:none">[43]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">913/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        APEX-EDGE (Application Exchange endpoint to relay service)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-RFC3340-43" rel="nofollow" style="color:rgb(11,0,128);background:none">[43]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">981/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался для удалённого управления устройствами Checkpoint FW-1 по протоколу&nbsp;
        <a href="https://ru.wikipedia.org/wiki/HTTPS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="HTTPS">HTTPS</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">989/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        FTPS-DATA (
        <a href="https://ru.wikipedia.org/wiki/FTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="FTP">FTP</a>
        -данные с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">990/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        FTPS (
        <a href="https://ru.wikipedia.org/wiki/FTP" rel="nofollow" style="color:rgb(11,0,128);background:none" title="FTP">FTP</a>
        -команды с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">991/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        NAS (Netnews Administration System)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-44" rel="nofollow" style="color:rgb(11,0,128);background:none">[44]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">992/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        TELNETS (
        <a href="https://ru.wikipedia.org/wiki/Telnet" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Telnet">Telnet</a>
        &nbsp;с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">993/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        IMAPS (
        <a href="https://ru.wikipedia.org/wiki/Internet_Message_Access_Protocol" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Internet Message Access Protocol">Internet Message Access Protocol</a>
        &nbsp;с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">994/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        резерв; ранее&nbsp;— IRCS (
        <a href="https://ru.wikipedia.org/wiki/IRC" rel="nofollow" style="color:rgb(11,0,128);background:none" title="IRC">IRC</a>
        &nbsp;с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">995/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        POP3S (
        <a href="https://ru.wikipedia.org/wiki/POP3" rel="nofollow" style="color:rgb(11,0,128);background:none" title="POP3">POP3</a>
        &nbsp;с шифрованием по&nbsp;
        <a href="https://ru.wikipedia.org/wiki/SSL" rel="nofollow" style="color:rgb(11,0,128);background:none" title="SSL">SSL</a>
        &nbsp;или&nbsp;
        <a href="https://ru.wikipedia.org/wiki/TLS" rel="nofollow" style="color:rgb(11,0,128);background:none" title="TLS">TLS</a>
        )
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">996/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">VSINET</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">996/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">XTREELIC (XTREE License Server)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">997/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">MAITRD</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">998/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">BUSBOY</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">998/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PUPARP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">999/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">PUPROUTER</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">999/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">GARCON</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">999/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">APPLIX</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">999/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">ScimoreDB Database System</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1000/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">CADLOCK2</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1001/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">sabserv (Sabre Desktop Reservation Software for Windows)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1001/UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        использовался в игре&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Tom_Clancy%E2%80%99s_H.A.W.X." rel="nofollow" style="color:rgb(11,0,128);background:none" title="Tom Clancy’s H.A.W.X.">Tom Clancy’s H.A.W.X.</a>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1002/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        MS-ILS, WIN2K-ILS, WINDOWS-ICFW&nbsp;— используется в&nbsp;
        <a href="https://ru.wikipedia.org/wiki/Microsoft" rel="nofollow" style="color:rgb(11,0,128);background:none" title="Microsoft">Microsoft</a>
        &nbsp;Windows Internet Connection Firewall и Windows Internet Locator Server service (служба программы организации видеоконференций&nbsp;
        <a href="https://ru.wikipedia.org/wiki/NetMeeting" rel="nofollow" style="color:rgb(11,0,128);background:none" title="NetMeeting">NetMeeting</a>
        ) вместо LDAP (см. порт 389)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1002/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        cogbot (
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=Opsware&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="Opsware (страница отсутствует)">Opsware</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/Opsware" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:Opsware">
              <span title="Opsware — версия статьи «Opsware» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;agent)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr bgcolor="lightsteelblue">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1008/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">UFSD (UFS-совместимый сервер)</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1010/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">SURF</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr bgcolor="khaki">
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1010/TCP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        <span>
          <a href="https://ru.wikipedia.org/w/index.php?title=ThinLinc&amp;action=edit&amp;redlink=1" rel="nofollow" style="color:rgb(165,88,88);background:none" title="ThinLinc (страница отсутствует)">ThinLinc</a>
          <sup style="line-height:1em;font-size:11.2px">
            <a href="https://en.wikipedia.org/wiki/ThinLinc" rel="nofollow" style="color:rgb(102,51,102);background:none" title="en:ThinLinc">
              <span title="ThinLinc — версия статьи «ThinLinc» на английском языке">[en]</span>
            </a>
          </sup>
        </span>
        &nbsp;Web Administration (Cendio AB)
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Неофициально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1011—1020</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1021/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        EXP1 (Experiment 1 по RFC3692)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-RFC4727-45" rel="nofollow" style="color:rgb(11,0,128);background:none">[45]</a>
        </sup>
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-46" rel="nofollow" style="color:rgb(11,0,128);background:none">[46]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1022/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">
        EXP2 (Experiment 2 по RFC3692)
        <sup style="line-height:1em;white-space:nowrap;font-size:11.2px">
          <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BF%D0%BE%D1%80%D1%82%D0%BE%D0%B2_TCP_%D0%B8_UDP#cite_note-RFC4727-45" rel="nofollow" style="color:rgb(11,0,128);background:none">[45]</a>
        </sup>
      </td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
    <tr>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">1023/TCP,UDP</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">резерв</td>
      <td style="border:1px solid rgb(162,169,177);padding:0.2em 0.4em">Официально</td>
    </tr>
  </tbody>
  <tfoot></tfoot>
</table>



## Динамические порты
Диапазон 49152—65535 содержит динамически выделяемые или частные порты, которые не регистрируются IANA. Эти порты используются временными (короткоживущими) соединениями «клиент — сервер» или в определенных частных случаях. Некоторые примеры таких частных случаев приведены в следующей таблице:

| Порт |  Описание |
| ---- | --------- |
|50000/TCP | Default DB2® database port|
|55777/UDP| ViPNet|