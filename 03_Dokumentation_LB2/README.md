# Dokumentation LB2


## Projektplanung – LB2 WordPress Migration

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

### Mein Architekturdiagramm finden sie hochgeladene datei als draw.io file.

## Hier sehen sie screenshots meiner umgebung die ich aufgebaut habe

![image](https://github.com/user-attachments/assets/bc5b277f-61e2-41dc-9567-ed6ee998488d)
Hier sieht man meine Server

![image](https://github.com/user-attachments/assets/85003dcf-8d27-499b-8e5a-770a448f74cd)

Diese Server laufen in diesem VPC.

![image](https://github.com/user-attachments/assets/e9454b0e-64d0-4b06-bcdd-fe2be8920178)

Hier sieht man das Subnetz das ich erstellt habe.

![image](https://github.com/user-attachments/assets/59f94f36-adf9-43f2-865e-646fc97ab47b)

Hier sieht man die Sicherheitsgruppe die ich erstellt habe. Ich habe die ganze umgebung wie in meinem Architekturdiagramm aufgebaut die Ip Addresen stimmen auch. Dan habe ich mir noch 3 éffentliche Ips gemacht damit ich auf meine Instnazen komme mit ssh.
## Hier sieht man mein Wordpress dashboard und die Login Daten

![image](https://github.com/user-attachments/assets/f881600b-48dc-4eaf-861f-7ab710fe6dc6)

![image](https://github.com/user-attachments/assets/063230f7-29b1-4ab0-bf7c-feb69fef9827)

## Hier sieht man mein phpinfo.php im Browser meines lokalen Notebooks

![image](https://github.com/user-attachments/assets/ad2b0a5f-fd2d-4b01-bbe7-1fdda866a406)

Gelb Markiert sieht man die einträge die ich geändert habe.


Mein passwort für den Root user ist TBZ12345!
