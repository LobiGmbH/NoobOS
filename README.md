# NoobOS
# NoobOS (C#)

NoobOS ist ein **Lernprojekt** für ein kleines Betriebssystem-ähnliches Framework in C#.

> Wichtig: Ein echtes Betriebssystem auf Ubuntu/Windows/macOS-Niveau umfasst Kernel-Treiber, Speicherverwaltung, Scheduling, Netzwerk-Stack, Security, Installer, GUI-Stack usw. – das ist ein riesiges Multi-Jahres-Projekt mit sehr vielen Entwickler:innen.

Dieses Repo liefert deshalb eine saubere, erweiterbare Grundlage:

- einfacher `Kernel`-Startablauf
- virtuelle In-Memory-Dateistruktur
- simuliertes Prozessmanagement
- interaktive Shell mit Basis-Kommandos

## Features

- Dateisystem-Befehle: `pwd`, `ls`, `cd`, `mkdir`, `touch`, `write`, `cat`, `rm`, `mv`
- Prozess-Befehle: `ps`, `start`, `kill`
- System-Befehle: `date`, `clear`, `help`, `exit`

## Starten

```bash
dotnet run
```

## Beispiel

```text
noobos:/home/user$ mkdir apps
noobos:/home/user$ cd apps
noobos:/home/user/apps$ touch notes.txt
noobos:/home/user/apps$ write notes.txt "Hallo aus NoobOS"
noobos:/home/user/apps$ cat notes.txt
Hallo aus NoobOS
```

## Nächste sinnvolle Schritte

1. Persistenz (Dateien auf Host speichern statt nur RAM)
2. Benutzer-/Rechtesystem
3. Paketmanager und Service-Konzept
4. Netzwerk- und IPC-Schicht
5. GUI statt reiner Shell
