# Projekt-Dokumentation

<span style="background: azure">☝️ Alle Text-Stellen, welche hell-blau hinterlegt sind, dienen nur Ihrer Information. Sie können sie löschen, sobald Sie sie gelesen haben. </span>

<span style="background: azure">Stellen, an welchen Sie etwas ausfüllen müssen, beginnen mit ✍️. Wenn Sie die nötige Information eingetragen haben, können Sie ✍️ entfernen.</span>

Erjon Hulaj, Avenazer Melles, Seyon Demiroglu

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|       | 0.0.1   | ✍️ Jedes Mal, wenn Sie an dem Projekt arbeiten, fügen Sie hier eine neue Zeile ein und erklären in *einem* griffigen Satz, was Sie an dem Tag erreicht haben. Diese Stelle gibt Ihnen und Ihrer Lehrperson eine einfache Möglichkeit, sich eine Übersicht über Ihr Projekt zu verschaffen. |
|       | 0.0.2  |  Heute haben wir am Code gearbeitet der für Forms dann verwendet werden soll, wir haben auch den Code in Forms eingebaut, aber wir müssen das Design vielleicht ein bisschen anders machen.                                                            |
|       | 0.0.3  |   Der Code ist fast fertig, wir müssen nur noch vielleicht das double, den wir für die berechnung benutzen, auf decimal ändern. Das Design ist auch fertig.                                                           |

## 1 Informieren

### 1.1 Ihr Projekt

In unserem Projekt entwickeln wir eine Anwendung zur Berechnung von unterjährigen Marchzins für Obligationen, bei der Benutzer Kauf- und Verkaufsdatum, Zinssatz und Kapital eingeben können, während unser Schwerpunkt auf präziser Zinsberechnung und der Integration von Internetinformationen liegt.

### 1.2 Anforderungen

| №    | Verbindlichkeit | Typ  | Beschreibung |
| ---- | --------------- | ---- | ------------ |
| 1    |  Muss               |  Funktional    |   Die Anwendung soll in der Lage sein, den Marchzins zu berechnen. Dies erfordert die Eingabe des Kauf- und Verkaufsdatums, des Kapitals und des Zinssatzes, die vom Benutzer erfragt werden.           | 
| 2    |  Muss               |  Funktional    |  Die aus dem bezogenen Daten sollen in einer Datei gespeichert werden, um für zukünftige Verwendungen verfügbar zu sein.           |
| 3   |  Kann              |  Qualität    |   Die Benutzeroberfläche der Anwendung sollte benutzerfreundlich und ansprechend gestaltet sein, um eine positive Benutzererfahrung zu gewährleisten.           |

<span style="background: azure">Jede Anforderung hat eine ganzzahlige Nummer (1, 2, 3 etc.), eine Verbindlichkeit (Muss oder Kann?), und einen Typ (Funktional, Qualität, Rand).</span>

### 1.3 Testfälle

| TC-№ | Vorbereitung (*given*) | Eingabe (*when*) | Erwartete Ausgabe (*then*) |
| ---- | ---------------------- | ---------------- | -------------------------- |
| 1.1  | Die Anwendung ist gestartet.                       |  Der Benutzer gibt das Kaufdatum, das Verkaufsdatum, das Kapital und den Zinssatz ein und bestätigt die Eingabe.                |  Die Anwendung berechnet den Marchzins und zeigt das Ergebnis auf dem Bildschirm an.                          |
| 1.2  |  Die Anwendung ist gestartet.                      | Der Benutzer gibt ungültige Daten für die Berechnung des Marchzinses ein, z.B. ein Kaufdatum, das nach dem Verkaufsdatum liegt, und bestätigt die Eingabe.                 |  Die Anwendung zeigt eine Fehlermeldung an und verhindert die Berechnung des Marchzinses.                          |
| 2.1  | Die Anwendung ist gestartet.                       |  Der Benutzer wählt die Option zur Internetabfrage aus. Die Anwendung kann keine Verbindung zum Internetdienst herstellen.                |  Die Anwendung zeigt eine Fehlermeldung an und speichert keine Daten.                          |
| 3.1  | Die Anwendung ist gestartet.                       |  Die Anwendung verfügt bereits über zuvor abgerufene Kursdaten.                |  Der Benutzer wählt die Option zur Anzeige der gespeicherten Kursdaten aus.                          |

<span style="background: azure">Jede Anforderung hat mindestens einen dazugehörigen Testfall. Der erste Testfall, der zur Anforderung mit der Nummer 1 gehört, hat die Nummer 1.1, der zweite Testfall, der zur Anforderung 1 gehört, die 1.2; der erste Testfall zur Anforderung 2 die 2.1 und so weiter. </span>

### 1.4 Diagramme

✍️ Hier können Sie PAPs, Use Case- und Gantt-Diagramme oder Ähnliches einfügen.

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung |
| ---- | ----- | --------- | ------------ |
| 1.A  | 06.11.23      | Erjon, Seyon, Aven         | Anforderung 1: Erstellung der Benutzeroberfläche und ausseinandersetzung mit Forms (Design u.s.w) [Erjon] für die Eingabe von Kauf- und Verkaufsdatum, Kapital und Zinssatz (Code) [Seyon]. Code für Forms kästchen [Aven] Dokumentation [Erjon]             |
| 1.B  | 13.11.23      | Aven          | Anforderung 1: Code für Exceptions, weil wir konnten noch nicht alle Fehler abfangen.             |
| 2.A  | 20.11.23      | Erjon         | Anforderung 1: Erlernen wie man Dateien speichert und das umsetzen. Design weiterarbeiten (Farben, Bilder)             |
| 2.B  | 20.11.23      | Erjon Hulaj          | Anforderung 2: Durchführung von Tests.             |
| 2.C  | 27.11.23      | Avenazer Melles          | Anforderung 2: Benutzerfreundliche Präsentation der gespeicherten Kursdaten in der Anwendung, Dokumentation der Benutzeroberfläche.             |
| 2.D  | 27.11.23      | Aven, Erjon          | Anforderung 2: Tests und Validierung der gespeicherten Datenwiedergabe, Dokumentation der Testergebnisse.             |
| 3.A  | 06.11.23      | Aven, Erjon          | Anforderung 4: Überarbeitung der Benutzeroberfläche, um sie benutzerfreundlicher und ansprechender zu gestalten, Dokumentation der Überarbeitung.             |
| 3.B  | 13.11.23      | Aven, Erjon          | Anforderung 4: Implementierung von Verbesserungen in der Benutzeroberfläche basierend auf den Benutzeranforderungen, Durchführung von Tests.             |
| 3.C  | 01.12.23      | Aven, Erjon         | Anforderung 4: Durchführung von Benutzertests und Anpassungen an der Benutzeroberfläche, Dokumentation der Benutzertests.             |
| ...  |       |           |              |

Total: 12 Arbeitspakete

<span style="background: azure">Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. *Frist* bedeutet, wann das AP abgeschlossen sein muss; *Zuständig* bezeichnet die (haupt-)verantwortliche Person.</span>

<span style="background: azure">Die Arbeitspakete sind wie die Testfälle nummeriert; aber gebrauchen A, B, C, ... statt 1, 2, 3.... Das erste Arbeitspaket zur Anforderung 1 ist also 1.A, das zweite 1.B etc. </span>

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | tatsächliche Zeit |
| ---- | ----- | ----------------- |
| 1.A  | 06.11.23      |  3 - 4 Stunden                 |
| 1.B  | 13.11.23      |  1 - 2 Stunden                 |
| 1.C  | 13.11.23      |  1 - 2 Stunden                 |
| 2.A  | 20.11.23      |                   |
| ...  |       |                   |


<span style="background: azure">Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten. </span>

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

## 6 Auswerten

✍️ Beschreiben Sie, was gut an Ihrem Projekt ging, und was Sie nächstes Mal anders machen würden.
