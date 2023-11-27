# Projekt-Dokumentation

<span style="background: azure">☝️ Alle Text-Stellen, welche hell-blau hinterlegt sind, dienen nur Ihrer Information. Sie können sie löschen, sobald Sie sie gelesen haben. </span>

<span style="background: azure">Stellen, an welchen Sie etwas ausfüllen müssen, beginnen mit ✍️. Wenn Sie die nötige Information eingetragen haben, können Sie ✍️ entfernen.</span>

Erjon Hulaj, Avenazer Melles, Seyon Demiroglu

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|       | 0.0.1   | ✍️ Jedes Mal, wenn Sie an dem Projekt arbeiten, fügen Sie hier eine neue Zeile ein und erklären in *einem* griffigen Satz, was Sie an dem Tag erreicht haben. Diese Stelle gibt Ihnen und Ihrer Lehrperson eine einfache Möglichkeit, sich eine Übersicht über Ihr Projekt zu verschaffen. |
|       | 0.0.2  |  Heute haben wir am Code gearbeitet der für Forms dann verwendet werden soll, wir haben auch den Code in Forms eingebaut, aber wir müssen das Design vielleicht ein bisschen anders machen.                                                            |
|       | 0.0.3  |   Der Code ist fast fertig, wir müssen nur noch vielleicht das double, den wir für die berechnung benutzen, auf decimal ändern. Das Design ist auch fertig.                                                           |
|       | 0.0.4  |   Der Code ist fertig. Wir haben es sogar geschafft die API hinzuzufügen. Es funktioniert alles so wie es soll.                                                           |

## 1 Informieren

### 1.1 Ihr Projekt

In unserem Projekt entwickeln wir eine Anwendung zur Berechnung von unterjährigen Marchzins für Obligationen, bei der Benutzer Kauf- und Verkaufsdatum, Zinssatz und Kapital eingeben können, während unser Schwerpunkt auf präziser Zinsberechnung und der Integration von Internetinformationen liegt.

### 1.2 Anforderungen

| №    | Verbindlichkeit | Typ  | Beschreibung |
| ---- | --------------- | ---- | ------------ |
| 1    |  Muss               |  Funktional    |   Die Anwendung soll in der Lage sein, den Marchzins zu berechnen. Dies erfordert die Eingabe des Kauf- und Verkaufsdatums, des Kapitals und des Zinssatzes, die vom Benutzer erfragt werden.           | 
| 2    |  Muss               |  Funktional    |  Die aus dem bezogenen Daten sollen in einer Datei gespeichert werden, um für zukünftige Verwendungen verfügbar zu sein.           |
| 3   |  Kann              |  Funktional    |   Zinssatz vom Internet abfragen können mit API           |
| 4   |  Kann              |  Qualität    |   Die Benutzeroberfläche der Anwendung sollte benutzerfreundlich und ansprechend gestaltet sein, um eine positive Benutzererfahrung zu gewährleisten.           |

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
| 2.A  | 20.11.23      | Erjon, Aven         | Anforderung 1: Erlernen wie man Dateien speichert und das umsetzen. Design weiterarbeiten (Farben, Bilder)             |
| 2.B  | 20.11.23      | Erjon          | Anforderung 2: Durchführung von Tests.             |
| 2.C  | 27.11.23      | Aven         | Anforderung 2: Benutzerfreundliche Präsentation der gespeicherten Kursdaten in der Anwendung, Dokumentation der Benutzeroberfläche.             |
| 3.A  | 27.11.23      | Aven, Erjon          | Anforderung 3: API einbauen sodass es funktioniert             |
| 4.A  | 06.11.23      | Aven, Erjon          | Anforderung 4: Überarbeitung der Benutzeroberfläche, um sie benutzerfreundlicher und ansprechender zu gestalten, Dokumentation der Überarbeitung.             |
| 4.B  | 13.11.23      | Aven, Erjon          | Anforderung 4: Implementierung von Verbesserungen in der Benutzeroberfläche basierend auf den Benutzeranforderungen, Durchführung von Tests.             |
| ...  |       |           |              |

Total: 12 Arbeitspakete

<span style="background: azure">Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. *Frist* bedeutet, wann das AP abgeschlossen sein muss; *Zuständig* bezeichnet die (haupt-)verantwortliche Person.</span>

<span style="background: azure">Die Arbeitspakete sind wie die Testfälle nummeriert; aber gebrauchen A, B, C, ... statt 1, 2, 3.... Das erste Arbeitspaket zur Anforderung 1 ist also 1.A, das zweite 1.B etc. </span>

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | tatsächliche Zeit |
| ---- | ----- | ----------------- |
| 1.A  | 06.11.23      |  2 - 3 Stunden                 |
| 4.A  | 06.11.23      |  1 Stunde                 |
| 1.B  | 13.11.23      |  1 - 2 Stunden                 |
| 4.B  | 13.11.23      |  1 - 2 Stunden                 |
| 2.A  | 20.11.23      |  1 - 2 Stunden                 |
| 2.B  | 20.11.23      |  1 Stunde                 |
| 2.C  | 27.11.23      |  1 Stunde                 |
| 3.A  | 27.11.23      |  2 - 3 Stunden                 |



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

Wir haben am Anfang ziemlich schnell gearbeitet und sind gut vorangekommen, sodass wir jetzt früher fertig sind als gedacht. Wir haben immer wieder das Programm verfeinert und besser gemacht und jetzt läuft es so wie es soll.
Wir sind zufrieden.

## 7 Code

```csharp
namespace Marchzins_Berechner
{
    public partial class Form1 : Form
    {
        private bool wurdeBerechnet = false;
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            if (wurdeBerechnet)
            {
                MessageBox.Show("Die Berechnung wurde bereits durchgeführt.");
                return;
            }

            DateTime kaufdatum, verkaufsdatum;
            double kapitalBerechnung, zinssatzProzent;

            string inputDateFormat = "dd.MM.yyyy";

            if (!DateTime.TryParseExact(kaufDatum.Text, inputDateFormat, CultureInfo.InvariantCulture, DateTimeStyles.None, out kaufdatum) ||
                !DateTime.TryParseExact(verkaufsDatum.Text, inputDateFormat, CultureInfo.InvariantCulture, DateTimeStyles.None, out verkaufsdatum))
            {
                MessageBox.Show("Ungültiges Datumsformat. Bitte geben Sie das Datum im Format 'dd.MM.yyyy' ein.");
                return;
            }

            if (kaufdatum >= verkaufsdatum)
            {
                MessageBox.Show("Kaufdatum muss vor dem Verkaufsdatum liegen");
                return;
            }

            if (!double.TryParse(kapital.Text, out kapitalBerechnung) || !double.TryParse(zinsSatz.Text, out zinssatzProzent))
            {
                MessageBox.Show("Ungültige Eingabe für Kapital oder Zinssatz");
                return;
            }

            if (kapitalBerechnung < 0 || zinssatzProzent < 0)
            {
                MessageBox.Show("Kapital und Zinssatz dürfen nicht negativ sein");
                return;
            }

            // Umwandlung Zinssatz von Prozent in Dezimalzahl
            double zinssatz = zinssatzProzent / 100.0;

            // Berechnung Anzahl Tage zwischen Kauf- und Verkaufsdatum
            int tage = (verkaufsdatum - kaufdatum).Days;

            // Berechnung Marchzins
            double marchzins = kapitalBerechnung * zinssatz * (tage / 365.0);

            // Anzeige Ergebnis
            marchZins.Text = $"{marchzins.ToString("C", System.Globalization.CultureInfo.CreateSpecificCulture("de-CH"))}";

            anzeigeBox.AppendText($"Kaufdatum: {kaufDatum.Text}" + Environment.NewLine);
            anzeigeBox.AppendText($"Verkaufsdatum: {verkaufsDatum.Text}" + Environment.NewLine);
            anzeigeBox.AppendText($"Kapital: {kapital.Text}" + Environment.NewLine);
            anzeigeBox.AppendText($"Zinssatz: {zinsSatz.Text}" + Environment.NewLine);
            anzeigeBox.AppendText($"Marchzins: {marchzins.ToString("C", System.Globalization.CultureInfo.CreateSpecificCulture("de-CH"))}" + Environment.NewLine);

            wurdeBerechnet = true;
        }

        private void button2_Click(object sender, EventArgs e)
        {
            wurdeBerechnet = false;
            kaufDatum.Clear();
            verkaufsDatum.Clear();
            kapital.Clear();
            zinsSatz.Clear();
            marchZins.Clear();
            anzeigeBox.Clear();
        }

        private void button3_Click(object sender, EventArgs e)
        {
            try
            {
                SaveFileDialog saveFileDialog = new SaveFileDialog();
                saveFileDialog.Filter = "Textdateien (*.txt)|*.txt|Alle Dateien (*.*)|*.*";
                saveFileDialog.Title = "Datei speichern";

                if (!wurdeBerechnet)
                {
                    MessageBox.Show("Es wurde noch keine Berechnung durchgeführt. Es gibt nichts zu speichern.", "Warnung", MessageBoxButtons.OK, MessageBoxIcon.Warning);
                    return;
                }

                try
                {
                    // Dein bisheriger Code für das Speichern der Datei bleibt unverändert...
                }
                catch (Exception ex)
                {
                    MessageBox.Show($"Fehler beim Speichern der Datei: {ex.Message}", "Fehler", MessageBoxButtons.OK, MessageBoxIcon.Error);
                }

                if (saveFileDialog.ShowDialog() == DialogResult.OK)
                {
                    string filePath = saveFileDialog.FileName;

                    using (StreamWriter writer = new StreamWriter(filePath))
                    {
                        writer.WriteLine($"Kaufdatum: {kaufDatum.Text}");
                        writer.WriteLine($"Verkaufsdatum: {verkaufsDatum.Text}");
                        writer.WriteLine($"Kapital: {kapital.Text}");
                        writer.WriteLine($"Zinssatz: {zinsSatz.Text}");
                        writer.WriteLine($"Marchzins: {marchZins.Text}");
                    }

                    MessageBox.Show("Datei wurde erfolgreich gespeichert.", "Erfolg", MessageBoxButtons.OK, MessageBoxIcon.Information);
                }
            }
            catch (Exception ex)
            {
                MessageBox.Show($"Fehler beim Speichern der Datei: {ex.Message}", "Fehler", MessageBoxButtons.OK, MessageBoxIcon.Error);
            }
        }

        private void anzeigeBox_TextChanged(object sender, EventArgs e)
        {

        }

        private async void api_Click(object sender, EventArgs e)
        {
            var client = new HttpClient();
            var request = new HttpRequestMessage
            {
                Method = HttpMethod.Get,
                RequestUri = new Uri("https://api.api-ninjas.com/v1/interestrate?country=Switzerland"),
                Headers =
                {
                    { "X-Api-Key", "kiMmYcZ0KHhQS7U2PVyrsQ==Jf6pvyrAxPJkYB5n" },
                },
            };
            
            try
            {
                using (var response = await client.SendAsync(request))
                {
                    response.EnsureSuccessStatusCode();
                    var body = await response.Content.ReadAsStringAsync();

                    int pos = body.IndexOf("rate_pct");
                    body = body.Substring(pos + 11, 4);

                    zinsSatz.Text = body;
                }

            }
            catch 
            {
                MessageBox.Show("Error");
            }
        }
    }
}
```
