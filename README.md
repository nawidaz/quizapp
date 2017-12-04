# NaWiDaZ Quiz App
![Travis Build](https://travis-ci.org/dekome/quizapp.svg?branch=master)

This repository contains the code of a mobile quiz web app that was developed within the [NaWi-DaZ 2.0 project](http://se.ifi.uni-heidelberg.de/research/projects/nawi_daz_20.html).
It is written in Java and web programming languages (e.g., Java Server Pages, Java Script) and stores data in an [SQLite database](https://www.sqlite.org).
The app runs on a Java servlet container such as [Tomcat](https://tomcat.apache.org/) or [Jetty](https://www.eclipse.org/jetty/) and can be accessed via browser.

The app has been developed in order to teach students German language with a focus on natural sciences and the scientific terminology. 
The app distinguishes between three user roles: administrators, students and teachers.

![Screenshot of the index page](screenshots/WelcomePage.png)

## NaWi-DaZ 2.0 Project

[NaWi-DaZ 2.0](http://se.ifi.uni-heidelberg.de/research/projects/nawi_daz_20.html) was a corporate project between the Heidelberg School of Education and the Software Engineering group of the Heidelberg University. 
It was financially supported by the [PLACE programme](https://hse-heidelberg.de/forschung/place-aktuell/).
The NaWi-DaZ 2.0 project investigated how students can learn the German language with focus on natural sciences.
For this purpose, this mobile quiz web app was developed, which enables students to learn scientific terminology without using their first language.

## Einsatz der App auf einem Raspberry Pi

Die App kann im Unterricht eingesetzt werden, ohne dass eine Verbindung mit Internet benötigt wird. Die App ist lauffähig auf einen Raspberry Pi und 
von dort aus dann erreichbar auf den lokalen Geräten wie Smartphones und Tablets. Das hat die folgenden Vorteile:
- Die App kann (theoretisch) überall zum Einsatz kommen, d.h. auch in Schulen, die kein öffentliches WLAN zur Verfügung stellen können
- Vertraulichkeit der Daten ist gewährleistet

## Beschreibung der Entwicklung

Bei der Entwicklung der App werden Methoden kontinuierlicher Softwareentwicklung eingesetzt. Zur Sicherung der Qualität wurde das Testsystem in der 
kontinuierlichen Softwareentwicklung eingebunden so das nach jeder Version in der Versionsverwaltung (Git) Regressionstest durchlaufen wurden. Test der 
Erreichbarkeit und Nutzbarkeit wurden mit Hilfe von Selenium und Selenium Grid durchgeführt. Komponenten Test wurden mit Hilfe von JUnit Test durchgeführt.

# Benutzerbeschreibung
## Installationsbeschreibung
## Lehrer nutzung
![alt tag](screenshots/LehreStart.jpg)
Lehrer können die Ergebnisse der Schüler im Lehrerzugang sich anzeigen lassen. Der Lehrerzug ermöglicht zwischen allgemeine Ergebnissen, für alle Aufgaben, 
sich ebenso die Ergebnisse für jeden Schüler separat anzeigen zu lassen. Eine Dritte Möglichkeit bietet hier die Metrik Ansicht in der Visuell 
die anzahlen der Richtigen bzw. Falschen Antworten dargestellt wird.

## Administrator nutzung
![alt tag](screenshots/AdministratorLogin.jpg)
Der Administrator Zugang ermöglicht die Verwaltung des Systems. Nach dem Einlogen kann der Administrator neben der Aufgabenerstellung der 3 Typen 
(Richtig/Falsch- , Satzverbindungs- und Beschriftungs-Aufgaben)  ebenso noch die Verwendeten Informationen Verwalten. Unter den Einstellung ist es möglich die 
Datenbank zu löschen und eine Neue Datenbank zu integrieren.

## Schüler nutzung
![alt tag](screenshots/SchuelerLogin.jpg)
Schüler haben, nach dem sie sich Registriert haben, die Möglichkeit
Aufgaben zu lösen. Hier können sie zwischen 3 Typen von Aufgaben auswählen
(Richtig/Falsch- , Satzverbindungs- und Beschriftung-Aufgaben) ebenso wie die
Schwierigkeit der Aufgaben. Nach der Bearbeitung einer Aufgaben bekommt der
Schüler direktes Feedback und hat die Möglichkeit sich weitere Aufgaben aus dem
Katalog zu suchen und diese weiter zu bearbeiten.
