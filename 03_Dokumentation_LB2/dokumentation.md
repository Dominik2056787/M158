# Projektdokumentation – M158 LB2 <br>WordPress-Migration

## Übersicht
# Projektdokumentation – Webserver-Projekt

Diese Dokumentation ist nach den Aufgaben (1–14) gegliedert. Jede Aufgabe ist in drei Phasen unterteilt. Bitte tragen Sie Ihre Ergebnisse jeweils unter den entsprechenden Abschnitten ein.

---

## Aufgabe 1 – Projektplan erstellen

### Stufe 1 - 3

In diesem Abschnitt habe ich einen Projektplan für meine WordPress-Migration erstellt. Der Plan zeigt alle wichtigen Aufgaben, die ich in den verschiedenen Phasen erledigen muss – von der Planung über das Einrichten der Server bis hin zur Migration und dem Abschluss.

Der Projektplan ist als Gantt-Diagramm mit Mermaid dargestellt. So kann ich die Aufgaben übersichtlich nach Datum und Phase darstellen.

Hier ist mein Projektplan zu den oben genannten Themen:

```mermaid
gantt
    title LB2 WordPress Migration – Projektübersicht
    dateFormat  YYYY-MM-DD
    axisFormat  %d.%m.%Y
    section Phase 1: Planung
    Projektstart & Planung              :a1, 2025-05-15, 1d
    Architekturdiagramm erstellen       :a2, 2025-05-22, 1d
    Planung abgeschlossen               :milestone, after a2, 0d
    section Phase 2: Zielumgebung
    Linux-Server Setup                  :b1, 2025-05-29, 1d
    Umgebung bereit                     :milestone, after b1, 0d
    section Phase 3: Dienste einrichten
    Webserver installieren              :c1, 2025-06-05, 1d
    PHP installieren                    :c2, 2025-06-05, 1d
    Datenbank konfigurieren             :c3, 2025-06-12, 1d
    Adminer installieren                :c4, 2025-06-12, 1d
    Dienste testen                      :c5, 2025-06-19, 1d
    Sicherheit konfigurieren            :c6, 2025-06-19, 1d
    Dienste bereit                      :milestone, after c6, 0d
    section Phase 4: Migration
    WordPress-Migration durchführen     :d1, 2025-06-26, 1d
    Migration abgeschlossen             :milestone, after d1, 0d
    section Phase 5: Abschluss
    Dokumentation erstellen             :e1, 2025-07-03, 1d
    Präsentation vorbereiten            :e2, 2025-07-03, 1d
    Lehrer zeigen                       :e3, after e2, 1d
    Projekt reflektieren                :e4, after e3, 1d
    Projekt abgeschlossen               :milestone, after e4, 0d
```
---

## Aufgabe 2 – Architekturdiagramm erstellen

### Stufe 1 - 3

Mein Architektur diagramm habe ich als datei in diesem Ordner gespeichert damit man eine Bessere sicht hat weil es sehr gross geworden ist.

---

## Aufgabe 3 – AWS-Umgebung einrichten

### Stufe 2


![image](https://github.com/user-attachments/assets/bc5b277f-61e2-41dc-9567-ed6ee998488d)
Hier sieht man meine Server

![image](https://github.com/user-attachments/assets/85003dcf-8d27-499b-8e5a-770a448f74cd)

Diese Server laufen in diesem VPC.

![image](https://github.com/user-attachments/assets/e9454b0e-64d0-4b06-bcdd-fe2be8920178)

Hier sieht man das Subnetz das ich erstellt habe.

![image](https://github.com/user-attachments/assets/59f94f36-adf9-43f2-865e-646fc97ab47b)

Hier sieht man die Sicherheitsgruppe die ich erstellt habe. Ich habe die ganze umgebung wie in meinem Architekturdiagramm aufgebaut die Ip Addresen stimmen auch. Dan habe ich mir noch 3 éffentliche Ips gemacht damit ich auf meine Instnazen komme mit ssh.


---

## Aufgabe 4 – DNS-Konfiguration

Ändern Sie die Stufe, für die Sie sich entschieden haben, selbst.

### Stufe 3

![image](https://github.com/user-attachments/assets/2d261cc4-3e56-4d9e-aaf9-0ad6311b3395)

Auf dem Bild sieht man meinen DNS Server der Active ist.

---

## Aufgabe 5 – Webserver konfigurieren

### Stufe 1

![image](https://github.com/user-attachments/assets/b8a46b0e-63af-4c45-b8f5-9199eec4f2a0)

### Stufe 2

![image](https://github.com/user-attachments/assets/0f909cc6-af7e-4de9-b9ff-2bbb4bfe5a89)

### Stufe 3

![image](https://github.com/user-attachments/assets/0813bfcc-06bf-4b39-9a32-880245f5f8cd)


---

## Aufgabe 6 – PHP einrichten

### Stufe 1

![image](https://github.com/user-attachments/assets/1ab4be13-29b6-4da2-9413-99db8c0d07d9)

### Stufe 2

![image](https://github.com/user-attachments/assets/ad2b0a5f-fd2d-4b01-bbe7-1fdda866a406)

Gelb Markiert sieht man die einträge die ich geändert habe.

### Stufe 3

![image](https://github.com/user-attachments/assets/123b9949-c4f4-432f-8b07-b991e98d09d7)

---

## Aufgabe 7 – MySQL/MariaDB aufsetzen

### Stufe 1

![image](https://github.com/user-attachments/assets/27e01dd5-6795-4637-b6d9-2f719ef93b54)


### Stufe 2

![image](https://github.com/user-attachments/assets/ee366644-8193-42de-a3e5-aec78f3cd122)

![image](https://github.com/user-attachments/assets/900261cc-c444-482a-ab0a-bcf9ae9e5270)


### Stufe 3

![image](https://github.com/user-attachments/assets/5f4489e8-09ce-4772-b198-c82249dad66f)


---

## Aufgabe 8 – Web-Datenbanktool (phpMyAdmin/Adminer)

### Stufe 1

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 2

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 1-3

![image](https://github.com/user-attachments/assets/992457ac-6c74-4217-8941-916f54999380)

phpMyAdmin wurde auf dem Webserver installiert und dan mit dem Datenbank Server verknüpft anmeldung mit meinem User funktioniert. Den user habe ich definiert in dem Architekturdiagramm an das habe ich mich genau gehalten.
---

## Aufgabe 9 – FTP-Zugang einrichten

### Stufe 1

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 2

Fügen Sie hier Ihre Ergebnisse ein

---

## Aufgabe 10 – WordPress migrieren

### Stufe 1

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 2

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 3

Fügen Sie hier Ihre Ergebnisse ein

---

## Aufgabe 11 – Backup-Konzept umsetzen

### Stufe 1

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 2

Fügen Sie hier Ihre Ergebnisse ein

---

## Aufgabe 12 – Testing der Webapplikation

### Stufe 1

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 2

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 3

Fügen Sie hier Ihre Ergebnisse ein

---

## Aufgabe 13 – Deployment automatisieren

### Stufe 1

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 2

Fügen Sie hier Ihre Ergebnisse ein

### Stufe 3

Fügen Sie hier Ihre Ergebnisse ein

---

## Aufgabe 14 – Docker verwenden

### Stufe 1 - 3

Fügen Sie hier Ihre Ergebnisse ein

---

