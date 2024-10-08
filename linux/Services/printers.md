Подключение samsung ML-1210 по USB к Centos7

ML-1210 работает через gdi драйвер, splix драйвер его не поддерживает http://splix.ap2c.org/

 yum install cups usbutils foomatic

lsusb покажет включенный принтер.

cups:

/etc/cups/cupsd.conf

1. слушать порт на всех интерфейсах

Port 631 #  или конкретный интерфейс Listen 192.168.0.1:631

2. Разрешить удаленный доступ  дописать Allow в три секции 

<Location />

  # Allow remote access...

  Order allow,deny

  Allow all  # можно добавить сеть 192.168.0.0/24

</Location>

<Location /admin>

<Location /admin/conf>

3.

Поправить iptables

4.

В браузере открыть http://<ip>:631

Авторизация по рутовой учетке(иначе нужно добавлять пользователя в группу(lpadmin не нашел???))

Вкладка Администрирование:

Нажать 

       Разрешить печать из интернета

       Анонсировать веб-интерфейс

 при этом перепишится  /etc/cups/cupsd.conf и перезапустится сервер

Кнопка Добавить принтер

Должен быть виден

Локальные принтеры:

 Samsung ML-1210 (Samsung ML-1210)

Иначе смотреть lsusb и проверять питание usb кабель

Отметить 

Совместный доступ:

 Разрешить совместный доступ к этому принтеру

Подсунуть ppd файл.(выбор из списка не тестировал) источник http://www.openprinting.org/driver/gdi

5. Подключить в клиентской системе по IPP

URI будет такой: ipp://192.168.1.45:631/printers/Samsung_ML-1210

проверка принтера

# lpstat -v device for Samsung_ML-1210: usb://Samsung/ML-1210

12 CUPS lpadmin Command Examples to Setup Printers on Linux
by KARTHIKEYAN SADHASIVAM on JANUARY 12, 2015

CUPS stands for Common UNIX Printing System.

lpadmin is a command line tool used to configure printer and class queues provided by CUPS.

A system running CUPS is a host that can accept print jobs from client computers, process them, and send them to the appropriate printer. It can also be used to set the server default printer or class.

This tutorial explains how to add a new printer, setup printer options, and manage printers on Linux environment using lpadmin command examples.

1. Adding a New Printer
To add a new network printer with the name “HPLaserJetP3015” use the lpadmin command with -p option as shown below:

# lpadmin -p HPLaserJetP3015 -v socket://19.86.82.172 -P  /usr/share/cups/model/HP/LaserJet_P3005-Postscript.ppd  # lpstat -v device for HPLaserJetP3015: socket://19.86.82.172

To verify if the printer is configured currently, you can use the command as shown in the below example:

# lpstat -p HPLaserJetP3015 -l printer HPLaserJetP3015 is idle.  enabled since Sun Jan 11 16:11:41 2015

2. PPD and Log Files
In the above example, PPD files (is also known as PostScript Printer Description) are created by vendors to describe the entire set of features and capabilities available for their PostScript printers and they are usually located under /usr/share/cups/model/ directory.

If you have any problems with configuring the printer, then please verify the logs at the below location for any error messages. This location may change depending upon the different distribution of Linux.

# ls -l /var/log/cups/* -rw-r--r-- 1 root lp  6851 Jan 11 16:19 /var/log/cups/access_log -rw-r--r-- 1 root lp 13207 Jan 11 16:19 /var/log/cups/error_log

3. Configure Printer on Parallel Port
In order to configure the printer on the parallel port (/dev/lp0), use the lpadmin command as shown in this example:

# lpadmin -p HPDESKJET882 -v parallel:/dev/lp0 -m  /usr/share/cups/model/HP/DeskJet_882C-cdj880.ppd

4. View All Available Ports for Printer Setup
Also to list all the available ports or interfaces available to configure the printer can be displayed using lpinfo command,

# lpinfo -v network socket direct hp network http network ipp network lpd direct parallel:/dev/lp0 direct scsi network tpvmgp network tpvmlp network smb

5. Multiple Printer Classes
CUPS always checks for an available printer in the order in which printers were added to a class.

You can add 1 or more printers to a class and when one of the printers becomes unavailable, the other printer defined in the class handles the print job requests.

It is not mandatory to add printers in classes. One printer class can themselves be members of other classes so it is possible for you to define printer classes for high availability for printing.

Once you configure the printer class, you can print to the printer class in the same way that you point to a single printer.

For example, If you have 2 Laserjet printers and 2 deskjet printers. you can create a class known as “Class-Laserjet”consisting 2 Laserjet Printers, and create another class known as “Class-Deskjet” printers and then create another class containing these 2 classes.

This way even if both the laserjet or deskjet printers go down, the other class serves the printing jobs.

6. Add Printer to a Class
To add a printer to the class, use the below command.

# lpadmin -h localhost -p HPLaserJetP3015 -c myclass

To verify whether the printers are in printer class:

# lpstat -c myclass members of class myclass:         HPLaserJetP3015

7. Remove Printer from a Class
To remove a printer from the class you can use the lpadmin command as shown in the below example:

in this example, myclass has two printers:

# lpstat -c myclass members of class myclass:         HPLaserJetP3015         HPDESKJET882

Remove the HPDESKJET882 printer from myclass as shown below:

# lpadmin -p HPDESKJET882 -r myclass

Once you remove it, you’ll see only the HP Laser Jet Printer:

# lpstat -c myclass members of class myclass:         HPLaserJetP3015

8. Remove a Whole Printer Class
Using the -x option, you can remove the class. as shown below.

# lpstat -c myclass members of class myclass:         HPLaserJetP3015  # lpadmin -x myclass  # lpstat -c myclass lpstat: Unknown destination "myclass"!

Please note that the printer configuration still exists even if you removed the class.

9. Change Printing Option
To change the printing options for the printer, you can execute the below commands.

List all the available options for the printer using lpoptions command as shown below.

In this example, you will see all the activated options is prefixed with asterisk symbol. If there is no asterisk is present, then it uses default settings.

# lpoptions -p HPLaserJetP3015 -l  PageSize/Page Size: *A4 Letter 11x17 A3 A5 B5 Env10 EnvC5 EnvDL EnvISOB5  EnvMonarch Executive Legal PageRegion/PageRegion: A4 Letter 11x17 A3 A5 B5 Env10 EnvC5 EnvDL EnvISOB5  EnvMonarch Executive Legal Resolution/Resolution: 150x150dpi 300x300dpi *600x600dpi 1200x1200dpi InputSlot/Media Source: *Default Tray1 Tray2 Tray3 Manual Duplex/Double-Sided Printing: DuplexNoTumble DuplexTumble *None

10. Change Printer Resolution
To change the resolution of the printer to 300x300dpi, you can use the lpadmin command as shown below:

# lpadmin -p HPLaserJetP3015 -o Resolution=300x300dpi  # lpoptions -p HPLaserJetP3015 -l

Here are the other options you can set for any printer using lpadmin with –o option as described in above example,

job-k-limit=value – Sets the kilobyte limit for per-user quotas. The value is an integer number of kilobytes.

job-page-limit=value – Sets the page limit for per-user quotas. The value is the integer number of pages that can be printed; double-sided pages are counted as two pages.

job-quota-period=value – Sets the accounting period for per-user quotas. The value is an integer number of seconds.

job-sheets-default=banner – Sets the default banner pages to use for print jobs.

name=value – Sets a PPD option for the printer. PPD options can be listed using the -l option with the lpoptions(1) command.

name-default=value – Sets a default server-side option for the printer.

port-monitor=name – The specified port monitor must be listed in the printer’s PPD file.

printer-error-policy=name – Sets the error policy to be used when the printer backend is unable to send the job to the printer.

printer-is-shared=true/false – Sets the printer to shared/published or unshared/unpublished.

printer-op-policy=name – Sets the IPP operation policy associated with the printer. The name must be defined in the cupsd.conf in a Policy section. The default operation policy is “default”.

11. Remove Printer from Configuration File
To remove a CUPS printer from the printer configuration file, you can use the -x option as shown below:

# lpstat -v device for HPLaserJetP3015: socket://19.86.82.172  # lpadmin -x HPLaserJetP3015  # lpstat -v lpstat: No destinations added.

12. Allow/Deny User or Groups to Configure Printer Options
You can allow the individual users or group to configure the printer options using lpadmin commands.

The following command will allow the user karthik to configure the printer option on HPLaserJetP3015 printer:

# lpadmin -p HPLaserJetP3015 -u allow:karthik

You can also block the user from changing the settings/options or configure printer using the below command.

The following command will deny the user karthik to configure the printer option on HPLaserJetP3015 printer:

# lpadmin -p HPLaserJetP3015 -u deny:karthik

If there is a group that needs to be allowed access, you can use the group name preceding with @ symbol. Multiple user names or groups can be given separated by commas.

For example, the following will allow users from sysadmin group to configure printer options.

# lpadmin -p HPLaserJetP3015 -u allow:@sysadmin

The following will deny users from developer group to configure printer options.

# lpadmin -p HPLaserJetP3015 -u deny:@developer