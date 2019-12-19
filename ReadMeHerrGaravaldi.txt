Guten Tag Herr Garavaldi

1. Laden Sie die aktuellste XAMPP Version aus dem Internet herunter
2. Entpacken Sie die XAMPP Daten auf den Desktop
3. Kontrollieren Sie bitte, ob der Ordner mailtodisk im Ordner xampp vorhanden ist. 
   Wenn nicht, dann entpacken Sie unser mailtodisk.zip Datei und legen sie im Ordner xampp ab.
4. Passen Sie unter xampp/php/ dass php.ini an. 
   Der Pfad bis zu xampp bitte vorher kopieren z.B. C:\Users\Anja\Desktop\ME17b_LB03_AnjaFahrni_MelanieMallepell\xampp\
   Er wird als Teil des sendmail_path verwendet. Bitte bis ...\xampp\ durch Ihren Pfad ersetzen.
   - Suchen Sie mail function und machen Sie folgende Anpassungen (und speichern Sie die Datei anschliessend):

	[mail function]
	; For Win32 only.
	; http://php.net/smtp
	;SMTP=localhost
	; http://php.net/smtp-port
	;smtp_port=25

	; For Win32 only.
	; http://php.net/sendmail-from
	;sendmail_from = me@example.com

	; For Unix only.  You may supply arguments as well (default: "sendmail -t -i").
	; http://php.net/sendmail-path
	sendmail_path = C:\Users\Anja\Desktop\ME17b_LB03_AnjaFahrni_MelanieMallepell\xampp\mailtodisk\mailtodisk.exe 

	; Force the addition of the specified parameters to be passed as extra parameters
	; to the sendmail binary. These parameters will always replace the value of
	; the 5th parameter to mail().
	;mail.force_extra_parameters =

	; Add X-PHP-Originating-Script: that will include uid of the script followed by the filename
	mail.add_x_header=Off

	; The path to a log file that will log all mail() calls. Log entries include
	; the full path of the script, line number, To address and headers.
	;mail.log =
	; Log mail to syslog (Event Log on Windows).
	;mail.log = syslog

5. Öffnen sie den XAMPP Ordner und führen Sie setup_xampp.bat aus
6. Starten Sie bitte unter XAMPP-Control den Apache-Server
7. Enpacken Sie unsere Webseite und speichern sie unter xampp/htdocs/AFWebseite_Dez19 ab
8. Öffnen Sie die Webseite auf localhost/AFWebseite_Dez19

Kontrollpfade
Pfad für das Mail: xampp/mailoutput (wird beim ersten Mailversand erstellt)
Pfad für die gespeicherten Daten: xampp/htdocs/AFWebseite_Dez19/php/Daten.csv

Vielen Dank und viel Spass auf der Webseite.

Gruss
Anja und Melanie