Backups
=======
Backups sind für so viele Missgeschicke die Lebensversicherung.
Wir empfehlen dringend eine große externe Festplatte.

Formatieren Sie diese über das Programm Laufwerke. Als Partitionstyp empfehlen wir beispielsweise ``ext4``.

Wir setzen auf das darunterliegende Programm ``borg``.
Es komprimmiert Backups, kann diese Verschlüsseln
und speichert in mehreren Iterationen nur die sich geänderten Stellen ab.

``borg`` wird von vielen Profis und Unternehmen unter Linux genutzt.

Da ``borg`` aber normalerweise eine Interaktion auf dem Terminal benötigt,
empfehlen wir das Programm ``Pika Backup``.

``Pika Datensicherung`` kann man ganz einfach aus der Anwendungsverwaltung installieren
und ist sehr einfach zu bedienen.

Einrichtung
-----------
- Stecken Sie Ihre externe Fesplatte an, und formatieren Sie diese gegebenenfalls.

.. note:: 
    Sollten Sie keine externe Fesplatte haben empfehlen wir für Backups dringend eine.
    Sollte Ihre Festplatte im Computer kaputt gehen oder Ihr Computer beispielsweise einen Wasserschaden bekommen,
    sind Ihre Daten ohne externe Fesplatte häufig schon verloren.

- Installieren und starten Sie das Programm ``Pika Datensicherung``.
- Wählen Sie ``Datensicherung einrichten`` und wählen Sie unter ``Ein neues Sicherungsdepot anlegen`` ``Ort auf dem Datenträger``.
- Wählen Sie als Ort entweder Ihre externe Fesplatte. (Wenn Sie keine externe Festplatte haben, wählen Sie Ihren Persönlichen Ordner).
- Sollten Sie sensible Daten haben, wählen Sie ``Verschlüsselt``, andernfalls ``Unverswchlüsselt``.

.. warning:: 
    Sollten Sie bei einem verschlüsselten Backup Ihr Passwort vergessen/verlieren, gibt es keine Möglichkeit, das Backup wiederherzustellen.

- Wählen Sie rechts oben ``Anlegen``.
- Nun können Sie bei ``Zu sichernde Dateien`` weitere Ordner hinzufügen. Standardmäßig wird der Persönliche Ordner gesichert. Dies reicht in der Regel vollkommen aus. Sollten Sie weitere Partitionen wie beispielsweise ``/data`` nutzen, fügen Sie hier die Ordner hinzu.
- Bei ``Von Sicherung ausschließen`` empfehlen wir, die Ordner ``Downloads`` (und ggf. ``Tmp``) auszuschließen. *Sollten Sie als Datensicherungsort Ihren Persönnlichen Ordner ausgewählt haben, fügen Sie den dementsprechenden Ordner hinzu. Er beginnt mit ``backup``.*

Durchführung
------------
Wir empfehlen, Backups beispielsweise jede Woche oder jeden Monat auszuführen.
Schließen Sie Ihre externe Festplatte an, öffnen Sie ``Pika Datensicherung`` und klicken Sie auf ``Back Up Now``.

.. note:: 
    Sollte die Datensicherung beim Ersten Mal fehlschlagen, stellen Sie sicher, dass Sie Schreibrechte im ausgewählten Sicherungsort haben.
    Sollte dies nicht der Fall gewesen sein, müssen Sie die Einrichtung wiederholen.

Dieser Vorgang kann das erste Mal sehr lange dauern.
Starten Sie am besten das Backup direkt vor dem Feierabend.

Wiederherstellung von Daten
---------------------------
.. tip:: 
    Es ist sehr wichtig, dass Sie diesen Schritt einmal ausprobieren.
    Somit sind Sie auf einen Ernstfall vorbereitet und wissen, dass Ihr Backup funktioniert.

- Öffnen Sie das BackUp Verzeichnis in der ``Pika Datensicherung``. (Dieser Schritt ist nur nötig, falls Sie das Backup von einem anderen Systen aus öffnen.)
- Wählen Sie den Reiter ``Archive``.
- Wählen Sie Ihren gewünschten Zeitpunkt aus und wählen Sie ``Gesicherte Dateien öffnen`` aus.
- Ein Dateimanger öffnet sich nun mit den Dateien. Kopieren Sie aus diesem Verzeichnis verschiedene Dateien auf Ihren Rechner. Die Zwei-Listen-Anicht mit ``F3`` empfiehlt sich hier sehr.
- Am Ende wählen Sie im Pika Datensicherungsprogramm ``Auswerfen`` aus. (Das Symbol dazu sehen Sie im Bild unten)

.. image:: images/pika_auswerfen.png


    
