# Programming Challenge

In this repository you will find my solution to the programming task that was completed in the course "Introduction to Programming" as part of the study of Business Informatics at DHBW Lörrach. The Task can be found below in German.

## Beschreibung

Die Daten, welche in dieser Challenge verwendet werden sollen, finden Sie in der Datei ```vehicle_data.xlsx```.
Bitte beachten Sie, dass die Daten zunächst aufbereitet werden müssen, also noch nicht in einer Qualität vorliegen, die
eine finale Insight-Generierung ermöglicht.

Die Quelldatei ```vehicle_data.xlsx``` beinhaltet Daten zu 500 Fahrzeugen:
Im Reiter ```sales code``` finden Sie 500 Trucks deren eindeutige Fahrzeugidentifikationsnummer
(FIN) als hash in der Spalte **_h_vehicle_hash_** dargestellt ist. Jedes Fahrzeug ist
aufgeschlüsselt nach **_Produktionsdatum_**, **_Land in welches das Fahrzeug verkauft wurde_**
und **_sales_code_array_**. Letztere Spalte beinhaltet Codes, welche die genaue Zusammensetzung
des Fahrzeuges (verbauter Motor, Leistungsklasse, Kabinentyp und weitere Merkmale) beschreiben. Im Reiter ```engines```
finden Sie 9 sales Codes, die Aufschluss darüber geben, welcher Motor (OM924, OM926, etc…) im entsprechenden
Fahrzeug verbaut ist.
Mit der Tabelle vehicle_hash können Sie die gehashte FIN (17 stellige Buchstaben-Zahlenkombination) zurück in die
originale Darstellung mappen.

Die Challenge teilt sich in zwei Aufgabenteile ein. Der erste Teil zielt auf ihre Softwareentwicklungsfertigkeiten ab.
Halten Sie bei der Code Gestaltung die gängigsten Clean Code Regeln ein und verfolgen Sie nach Möglichkeit eine
testgetriebene Entwicklung. Im zweiten Aufgabenteil sollen Sie verschiedene Analysen durchführen. Verwenden Sie
dazu die Daten, welche Sie in Aufgabenteil eins aufbereitet haben. Bevor Sie starten, bietet es sich an sich zunächst
mit den Datenätzen vertraut zu machen. Verschaffen Sie sich einen Überblick und erkunden Sie die Zusammenhänge der
Datensätze.

## Aufgabe 1

Schreiben Sie eine ETL Pipeline zur Datenaufbereitung. Gehen Sie dabei wie folgt vor.

- Daten laden
- Daten bereinigen und aufbereiten
- Daten zusammenführen
- Gesamttabelle bestehend aus folgenden Spalten abspeichern:
    - fin
    - production_date
    - country
    - sales_code_array

## Aufgabe 2

Analysieren Sie den die Daten, indem Sie folgende Fragestellungen auswerten. Visualisieren
Sie ihre Ergebnisse.

- Welches sind die top drei Länder, in die wir zwischen 01.01.2014 und 31.12.2020 am meisten Fahrzeuge verkauft haben.
- In welchem dieser Jahre haben wir insgesamt am meisten Fahrzeuge verkauft?
- Welche FIN hat das zeitlich erste verkaufte Fahrzeug.
- Wie viele Fahrzeuge wurden zwischen 01.01.2017 und 01.01.2021 mit OM934, OM936, OM470 und OM471 Motoren verkauft.
- Welche Fahrzeuge (FIN) wurden zwischen 01.01.2017 und 01.01.2021 und mit OM936 Motor nach Neuseeland verkauft.
