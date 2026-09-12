<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h3 align="center">User Authentication made with ASP.NET</h3>

  <p align="center">
    In diesem Readme wird erklärt, wie das ganze funktioniert, welche Fehler erschienen sind und wie man sie behebt.
    <br />
    <a href=""><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="">View Demo</a>
    ·
    <a href="">Report Bug</a>
    ·
    <a href="">Request Feature</a>
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Inhaltsverzeichnis</summary>
  <ol>
    <li>
      <a href="#über-das-projekt">Über das Projekt</a>
    </li>
    <li>
      <a href="#vorgang">Vorgang</a>
    </li>
    <li>
      <a href="#fehler">Fehler</a>
    </li>
    <li>
      <a href="#installation">Installation</a>
    </li>
  </ol>
</details>

## Über das Projekt
Das Projekt wird als Vorbereitung für das Ulrich + Hefti Projekt genutzt. In dieser Applikation soll man sich einfach ein- und wieder ausloggen können. Dem entsprechend sollen noch Zugriffsdaten, je nach dem mit welchem Benutzer man eingeloggt ist angezeigt, oder eben nicht angezeigt werden.<br>
Projektauftrag stammt von Janik Lüthi.

## Vorgang
Die Version von Visual Studio sollte egal sein, aber in diesem Beispiel wird Visual Studio 2022 verwendet.
Nach dem Öffnen von Visual Studio muss ein neues Projekt erstellt werden.<br>

![projekt_erstellen_1](https://user-images.githubusercontent.com/64250640/177317021-feffa02b-b9eb-40a5-9b3a-ec46a1ac2aac.png)

In der Eingabe "ASP.NET Core-Web-App (Model View Controller)" auswählen. Man kann aber auch "ASP.NET Core-Web-App" eingeben. Danach kann man auch dort selber entscheiden, welche Vorlage man gerne nehmen würde.

![projekt_auswaehlen_2](https://user-images.githubusercontent.com/64250640/177317107-01ce1dd6-ab40-49dc-b0dc-beea5719f83a.png)

Hier kann man nun den Projektnamen definieren, sowie dauch den Speicherort.

![projektname_definieren_3](https://user-images.githubusercontent.com/64250640/177317143-269a151d-73b5-438b-88a7-d56c5283a1b9.png)

Hier muss man anschliessend als Framework die .NET Version 6 verwenden. Falls .NET 6 nicht mehr die neuste wäre, einfach die Neuste auswählen.
Zudem muss man als Authentifizierungstyp "Einzelne Konten" auswählen. Im Englischen wäre es "Individual User Accounts". Nun kann man das Projekt erstellen.

![einzelne_konten_auswaehlen_4](https://user-images.githubusercontent.com/64250640/177317169-e820d80c-f1ed-48aa-8514-45c2b303f5a3.png)

Nach dem Erstellen des Projekts kann man das Projekt ausführen. Nach der Ausführung sollte es in etwas so aussehen.

![oeffnen_5](https://user-images.githubusercontent.com/64250640/177317204-6d5236c2-45c2-403d-9f9d-76c9e1d8fae1.png)

Das angeschaute Video um den Auftrag überarbeiten zu können:
https://www.youtube.com/watch?v=CzRM-hOe35o&t=849s

## Fehler
Falls bei beim Starten des Projekts ein Fehler auftaucht mit dem Fehler 
```sh
IOException: IDX20807: Unable to retrieve document from: 'System.String'. HttpResponseMessage:
```

Sollte man die zwei folgenden Befehle ausführen. 
```sh
dotnet tool install -g msidentity-app-sync
dotnet tool list -g
```

Warum, wüsste ich selber auch nicht. Für mehr Details muss man diesen Link besuchen: 
https://stackoverflow.com/questions/66865872/ioexception-idx20807-unable-to-retrieve-document-from-system-string-httpre

## Installation

1. Als erstes müssen Sie git auf Ihrem lokalen Computer installieren. Dazu müssen Sie diese [Website] (https://git-scm.com/downloads) besuchen.
2. Suchen Sie in Ihrem Windows-Explorer nach einem geeigneten Speicherort für das Projekt
3. Klicken Sie nun mit der rechten Maustaste auf den Ordner oder den Speicherort und dann auf "Git Bash Here".
4. Schließlich öffnet sich etwas wie die Windows-Eingabeaufforderung. Wenn Sie das tun, müssen Sie nur folgendes eingeben
```sh
git clone https://github.com/olivierluethy/UserAuthInAsp.NET.git
```
5. Wenn Sie das Projekt erfolgreich geklont haben, müssen Sie eine lokale Datenbank haben. Ich habe [XAMPP](https://www.apachefriends.org/de/index.html) verwendet. Wenn du es auch benutzen willst, dann stelle bitte sicher, dass du die neueste Version herunterlädst. Sonst funktioniert es nicht wie erwartet.
