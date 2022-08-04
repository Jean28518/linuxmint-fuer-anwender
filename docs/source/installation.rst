Einfache Installation
=====================


Bootstick erstellen
-------------------

Hierfür empfiehlt sich das Programm `Etcher <https://www.balena.io/etcher/>`_. 
Hat man alternativ schon eine Linux Mint Maschine verfügbar, 
kann man dies über das Programm ``USB-Abbilderstellung`` erledigen.


Speicherplatz frei machen
-------------------------

Dies kann man bei Windows über das Programm ``Festplattenpartitionen erstellen`` erledigen.
Bei Linux Mint kann man dies über das Programm ``gparted`` oder über ``Laufwerke`` machen.
Es ist empfohlen, mindestens 50 GB verfügbar zu machen.
Das Erstellen einer Partition auf dem freien Speicherplatz ist nicht nötig. 

.. note:: 
    Wenn man Linux Mint neben Windows installieren möchte, ist dringend empfohlen,
    die beiden Systeme jeweils auf eine eigene Festplatte zu installieren.
    Somit hat Windows nicht die Möglichkeit, den Linux-Bootloader zu überschreiben.    


Installation
------------

Den USB-Stick starten. Sollten Sie Probleme haben, den USB-Stick zu starten, 
suchen Sie im Internet nach Ihrem Laptop-Modell oder Mainboardhersteller und fügen Sie ``von USB-Stick starten`` hinten an.
Gängige Tasten sind: ``ESC``, ``F2``, ``F8``, ``F11``, ``F12``, oder ``Entf``.

.. note:: 
    Sollte es Probleme beim Hochfahren von Linux Mint geben, können Sie beim Starten des USB-Sticks den ``Compatibility`` Modus auswählen.
    Wenn danach die Bildschirmauflösung noch nicht perfekt sein sollte, ist das okay.

Bei der Installation wie gehabt vorgehen. 
Es ist empfohlen, die Multimedia-Codecs zu installieren.

Sollten Sie wie oben beschrieben freien Speicherplatz geschaffen haben, wählen sie ``Linux Mint daneben installieren`` aus.
Der Rest wird automatich erledigt. Diese Prozedur ist empfohlen, da sie am wenigsten Komplikationen erfordert.

Konfigurieren Sie danach in den restlichen Schritten die Linux Mint Installation nach Ihren Wünschen.

.. warning:: 
    Bitte wählen Sie bei der Benutzerkonfiguration ``Meinen Persönlichen Ordner verschlüsseln`` nicht unbedacht aus.
    Sollten Sie den Wiederherstellungs-Schlüssel (den Sie beim ersten Start des Systems dann angezeigt bekommen) 
    und Ihr Passwort verloren haben, gibt  es keine Möglichkeit mehr, Ihre Daten wiederherzustellen.