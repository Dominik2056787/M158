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
