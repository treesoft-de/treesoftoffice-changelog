# Änderungsprotokoll Version 6.4

## 6.4.16

### CAD

#### Menü "Zuletzt bearbeitete Projekte"

Im CAD gibt es im Menü "Projekt" ein Untermenü "Zuletzt bearbeitete Projekte". Im Optionen-Dialog des CAD (System->Projekt) kann der Anwender festlegen, welche Projektinformation in dem Untermenü angezeigt werden. Nach einer Neu-Installation wurden im Menü "Zuletzt bearbeitete Projekte" die Oberbegriffe angezeigt. Wechselte man in den Optonen-Dialog war dort fälschlicherweise das Feld "Bezeichnung" gewählt. 

Nach einer Installation ist die Standardvorgabe für die Anzeige der zuletzt bearbeitenden Projekte der Oberbegriff.

#### Projekt drucken

Im CAD können mit der Funktion "Projekt drucken" mehrere Dateien eines Projekets hintereinander auf dem Drucker ausgegeben werden. Nach dem Aufruf der Funktion erscheint zunächst der Dialog "Seite einrichten". Wählte man hier die Seitenansicht aus, wurde sofort die Druckausgabe gestartet.

Der Fehler ist korrigiert.

### CAD Schaltplan-Assistent

#### Einstellungen zur Beschriftung als Standard speichern

Einige Einstellungen zur Beschriftung werden im Treesoft CAD in der Datei apar.dat gespeichert. Diese Datei wird bei der Neuanlage eines Projektes aus dem AppData-Verzeichnis des Systems in das neue Projektverzeichnis kopiert. Da die Einstellungen, die in der Datei apar.dat im AppData-Verzeichnis hinterlegt sind, bisher nicht geändert werden konnten, mussten nach der Neuanlage eines Projektes die Beschriftungsparameter in der Regel zunächst angepasst werden.

Im Optionen-Dialog besteht nun die Möglichkeit die Grundeinstellungen der Beschriftungsparanter, die in der Datei apar.dat gespeichert werden, zu überschreiben. Hierzu gibt es in der Toolbar des Dialoges die neue Schaltfläche Standard. Gespeichert werden folgende Einstellungen:

- Beschriftungsregel
- Beschriftungsmodus
- Bmks immer neu vergeben
- Potentiale und Klemmen vorschlagen
- Obergrenze für Pfadtexte
- Untergrenze für Pfadtexte

#### Kommentare beim "Speichern unter"

Im Treesoft CAD können Dateien Kommentare zugeordnet werden, die den Inhalt der jeweiligen Datei beschreiben. Bei der Funktion "Speichern unter" gab es keine Möglichkeit einen Kommentartext einzugeben. 

Der Dialog "Speichern unter" wurde um ein Eingabefeld "Kommentar" erweitert. Wenn die zu speichernde Datei bereits einen Kommentar zugeordnet hat wird dieser angezeigt. Das Eingabefeld ist mit einer Auswahlliste kombiniert, aus der vordefinierte Kommentare aus der Standarddatei für Kommentartexte ausgewählt werden können. In der Auswahlliste werden nur Kommentare zu Zeichnungen (Dateien mit der Erweiterung .zng) angezeigt.

#### Datei öffnen, Datei speichern unter

Im CAD gab es bisher verschiedene Dialoge zum Öffnen von Zeichnungsdateien. Im Optionen-Dialog Schaltplan->Datei konnte man eine von drei möglichen Varianten wählen, die beim Öffnen von Dateien [Strg]+[O] verwendet werden soll.

Zukünftig wird beim Öffnen von Zeichnungen [Strg]+[O] das Dokumentenfenster eingeblendet. Zusätzlich besteht die Möglichkeit mit der Taste [F8] den Datei-Dialog zu verwenden. Analog dazu wird mit der Taste [F9] die Funktion "Speichern unter" aufgerufen.

#### Einzeln/Alles beschriften

Im Schaltplan-Assistenten können in den Dialogen "Einzeln beschriften" bzw. "Alles beschriften" die zu beschriftenden Texte individuell festgelegt werden. Es fehlte die Möglichkeit den Lieferzustand wieder herzustellen.

In der Toolbar gibt es nun eine Schaltfläche "Lieferzustand". Mit dieser Funktion werden die Einstellungen restauriert.

#### Bmk Auswahl

In den Dialogen zur BmK Auswahl bei Klemmen, Potentialen, Kontakten, SPSen und Kabeln hatte nach dem Öffnen immer das Eingabefeld "Matchcode" den Fokus, erkennbar durch den blinkenden Cursor. Um ein neues Betriebsmittelkennzeichen einzugeben musste daher zumächst z.B. mit der Taste [Tab] in das nächste Eingabefeld "BmK" gewechselt werden

Nach dem Öffnen der Dialoge zur BmK Auswahl erhält nun immer eines der beiden Eingabefelder "Matchcode" und "BmK" den Fokus, welches beim letztmaligen Öffnen zuletzt den Fokus innehatte. Diese Eigenschaft wird für jede Betriebsmittelart separat verwaltet.

#### Nummernkreis für Dummys

Bei der Neuanlage von Dummys war es bisher nicht möglich eine Nummer über einen entsprechenden Nummernkreis auszuwählen.

Die Funktion steht jetzt zur Verfügung. Die Nummer wird ermittelt, indem mit der linken Maustaste auf den Text "Nummer:", der als Hyperlink dargestellt wird, geklickt wird.

#### Symbol speichern unter, Katalogzweig wählen

Beim Erstellen von Symbolen konnte bisher nur die Symbolbibliothek gewählt werden, in der das Symbol gespeichert werden soll, sowie ein entsprechender Kommentar eingegeben werden. Eine Zuordnung zu einem Katalogzweig war nicht möglich.

Beim Speichern von Symbolen kann nun direkt ein Zweig des Eigenen Kataloges ausgewählt werden.

#### Artikelzuordnung ändern

Im Treesoft CAD können auswertungsrelevanten Symbolen Artikel zugeordnet werden. Hierzu finden sich im Menü "Symbol" die beiden Optionen "Artikel einzeln zuordnen" sowie "Alle Artikel zuordnen". Über die Menü-Option "Artikelzuordnung ändern" wird festgelegt, ob nur Symbole berücksichtigt werden sollen, die noch keinen Artikel zugeordnet haben, oder alle Symbole. Demzufolge musste man, wenn man den Artikel eines bestimmten Symboles ändern wollte, zunächst diese Option aktivieren.

Die Menü-Option "Artikelzuordnung ändern" gilt nur noch für den Befehl "Alle Artikel zurdnen". In der Funktion "Artikel einzeln zuordnen" wird dagegen immer das zur Fadenkreuzposition nächst gelegene Symbol bearbeitet, unabhängig davon, ob diesem bereits ein Artikel zugeordnet worden ist oder nicht.

#### Wiederholfunktion "W"

Wenn man in der Funktion "Artikel/Symbol setzen" ein Symbol als Grafik setzte und anschließend das Fadenkreuz mit der Tastatur an eine andere Position bewegte, funktionierte die Wiederholfunktion (Taste [W]) nicht. Erst wenn die Maustaste betätigt wurde, konnte die Funktion aufgerufen werden.

Dieser Fehler ist korrigiert.

#### Datei neu

Im Treesoft CAD können Kommentare zu Dateien hinterlegt werden. Für die meisten Zeichnungsdateien sind die Kommentare vordefiniert und in der Datei describe.dat im AppData-Verzeichnis gespeichert. Bei der Neuanlage einer Zeichnung im Schaltplan-Assistenten konnte man zwar einen Kommentar hinterlegen, ein passender vordefinierter Kommentar wurde allerdings nicht vorgeschlagen.

Bei der Neuanlage einer Zeichnungsdatei ist nun ein Standard-Kommentar voreingestellt.

#### Inhalt n beschriften

Im Menü "Text" gab es die Menü-Option "Rahmen&variable «Inhalt n» beschriften...". 

Da mit dieser Funktion nur die beiden Variablen «Inhalt 1» und «Inhalt 2» beschriften werden können, wurde der Befehl in "Inhalt 1/Inhalt 2 beschriften" umbenannt.

#### Artikel aus Fremdkatalog zuordnen

Bei der Zuordnung von Artikeln zu Symbolen werden alle Artikel zur Auswahl angeboten, bei denen das jeweilige Symbol primär bzw. sekundär zugeordnet ist. Wird die Auswahlliste um einen Artikel aus einem Fremdkatalog ergänzt, wird die Zuordnung des Artikels zum jeweiligen Symbol als Sekundärreferenz in der Datenbank gespeichert. Wenn dem neu zugeordneten Artikel kein Symbol zugeordnet ist, erfolgte bisher keine direkte Zuordnung in der Kopie des Artikels im Eigenen Katalog.

Wenn bei der Beschriftung von Symbolen Artikel neu ausgewählt werden, denen noch kein Symbol zugeordnet ist, wird automatisch eine primäre Zuordnung gebildet.

#### Freien Text erstellen/ändern

Im Schaltplan-Assistenten wird beim Betätigen der rechten Maustaste ein Kontext-Menü angeboten. Bevor das Menü dargestellt wird, wird zunächst überprüft, welche Objekte sich in der Nähe der Fadenkreuzposition befinden. Wenn das nächste Objekt ein Text ist, wird die zusätzliche Option "Freien Text erstellen / ändern" im Kontext-Menü angeboten. Die Suche nach einem Text wurde allerdings nur dann durchgeführt, wenn sich auf den sichtbaren Ebenen freie Texte befanden; Symboltexte wurden nicht berücksichtigt. Das erschwerte z.B. die Beschriftung des Zeichnungsrahmen in einer sonst leeren Datei.

Die Suche nach einem Text wird nun immer dann durchgeführt, wenn auf den sichtbaren Ebenen freie Texte oder Symboltexte vorhanden sind.

#### Automatische BmKs für Klemmen und Kabel

Im Treesoft CAD kann der Anwender bei der Beschriftung von Betriebsmitteln zwischen verschiedenen Algorithmen wählen, nach denen die Betriebsmittel beschriftet werden sollen. Bei Beschriftung von Klemmen und Kabeln konnte der Anwender bisher nur das BmK manuell eingeben oder ein bereits vergebenes Betriebsmittelkennzeichen aus einer Liste auswählen. In der Regel werden die Betriebsmittelkennzeichen von Klemmen und Kabeln nach der Beschriftungsregel "Bmk/lfd" vergeben. Bei umfangreichen Schaltplänen konnte es umständlich sein, das nächste noch nicht vergebene BmK zu ermitteln. Einige Anwender wiederum verwenden den Algorithmus "Blatt/Pfad" bei der Beschriftung von Klemmen bzw. Kabeln. Diese BmKs mussten bisher manuell eingegeben werden.

Um den o.g. Anforderungen gerecht zu werden, sind die Dialoge zur Eingabe bzw. Auswahl von Betriebsmittelkennzeichen bei Klemmen und Kabeln erweitert worden. Unmittelbar neben dem Eingabefeld "BmK:" befindet sich nun eine Schaltfläche. Hierbei wird ein neuen BmK gemäß der Beschriftungsregel "Bmk/lfd" generiert und in das Eingabefeld "BmK" übertragen. Der Fokus wechselt ebenfalls in das Eingabefeld, so dass der Dialog direkt mit der Eingabetaste beendet werden kann. Beim nächsten Aufruf des Beschriftungsdialoges bei einer unbeschrifteten Klemme bzw. eines Kabels wird das zuvor automatisch generierte BmK in der Liste vorselektiert (so wie bei der manuellen Eingabe auch), da die Beschriftungsregel "Bmk/lfd" überwiegend bei der aufgelösten Darstellung von Betriebsmitteln verwendet wird.
Über ein weiteres neues Steuerelement "Bmk vorschlagen" kann der Anwender festlegen, ob ein Vorschlag gemäß der eingestellten Beschriftungsregel in der Auswahlliste angezeigt werden soll. Dieser Vorschlag befindet sich immer am Anfang der Liste und kann unmittelbar nach dem Öffnen des jeweiligen Dialoges bei unbeschrifteteten Klemmen bzw. Kabeln mit der Eingabetaste übernommen werden. Beim nächsten Aufruf des Beschriftungsdialoges bei einer unbeschrifteten Klemme bzw. eines Kabels wird wiederum der erste Eintrag der Liste vorselektiert, da diese Form der Beschriftung bei Betriebsmitteln verwendet wird, die nicht aufgeöst dargestellt werden. Demzufolge wird hierbei in der Regel ein neues Bmk angefordert.

#### Leerzeichen in Anlage- und Ortskennzeichen

Wenn man im Schaltplan Anlagen- oder Ortskennzeichen mit Leerzeichen verwendet hatte, funktionierte die abgekürzte Schreibweise der Betriebsmittelkennzeichen nicht.

Der Fehler ist korrigiert.

#### Artikel-/Symbol setzen

In der Funktion Artikel-Symbol setzen werden Artikel oder Symbole katalogbezogen aus einer Liste ausgewählt. Startete man die Auswertung bei geöffneter Liste, so konnte anschließend nicht mehr mit den Pfeiltasten in der Liste navigiert werden.

Der Fehler ist korrigiert.

#### Variablentext

Variablentexte haben im Gegensatz zu anderen Texten weitere Spezifikationen, die als Varibalen-Art bezeichnet werden. Die Variablen-Art wird bei der Erstellung von Texten in einem separaten Dialog eingestellt. Der nächste neu zu erstellende Variablen-Text sollte die zuletzt gewählte Variablen-Art zugewiesen bekommen. Allerdings wurde die Variablen-Art nicht richtig restauriert.

Der Fehler ist korrigiert.

#### Artikel zuordnen

In der Funktion Artikel/Symbol setzen wurden Material, Leistungen und Dummys wechselweise in voneinander getrennten Listen angezeigt. Eine gemeinsame Liste der unterschiedlichen Stammdaten konnte nicht angezeigt werden.

Der Dialog "Artikel zuorden" wurde vollständig überarbeitet, so dass nun alle Stammdaten, denen dass zu beschriftende Symbol zugeordnet sind, zusammen in einer Liste angezeigt werden. Darüberhinaus wurden einige Änderungen im Handling des Dialoges vorgenommen, um den neuen Anforderungen gerecht zu werden und die Bedienung einfacher und transparenter zu gestalten.

#### Artikel/Symbol setzen

Wenn in der Funktion "Artikel/Symbol setzen" ein Artikel ausgewählt wurde, dem das Makro 0artvari zugeordnet war, befand sich nach der Positionierung des zugeordneten Symbols das Fadenkreuz nicht auf dem Bezugspunkt des Symbols.

Der Fehler ist korrigiert.

#### Überflüssige Menüs und Optionen

Die Menüs im Schaltplan-Assistenten enthielten einige überflüssige Befehle, die entfernt wurden. Der Optionen-Dialog wurde ebenfalls bereinigt.

Bereinigung der Menüs.

#### Rastergrafik setzen

Beim Einfügen einer Rastergrafik in eine Zeichnung besteht die Möglichkeit diese zu positionieren bzw. zu skalieren. Dies erfolgt über den Dialog "Rastergrafik", indem noch weitere Parameter eingestellt werden können. Der Inhalt des Dialoges wurde allerdings bei jeder Mausbewegung aktualisiert, so dass eine vernünftige Parameterierung der Rastergrafik nicht möglich war.

Der Fehler ist korrigiert.

#### SPS-Zuordnungsliste definieren

Mit der Funktion "SPS-Zuordnungsliste definieren" werden aus sequentiellen Zuordnungslisten Textbausteindateien für das CAD erzeugt oder umgekehrt. Beim erstmaligen Aufruf in einem Projekt war das Verzeichnis der Zuordnungsliste nicht vorbelegt. Darüberhinaus war für die Textbausteindatei das Verzeichnis des Projektes voreingestellt und nicht das jeweilige Unterverzeichnis TreeCAD.

Beim erstmaligen Aufruf der Funktion in einem Projekt werden beide Verzeichnisse auf auf das CAD-Unterverzeichnis des aktiven Projektes voreingestellt. Die Einstellungen des Dialoges werden anschließend in der Datei "ZolTbs.def" im jeweiligen Projekt gespeichert.

#### Projektpfad wird beim Anmelden eines Projektes nicht gespeichert

Bevor Projekte im Treesoft CAD bearbeitet werden können, müssen diese in der Datenbank gespeichert sein. Hierzu dient u.a. die Funktion "Projekt anmelden". In einigen Fällen kam es vor, dass nach dem Anmelden eines Projektes der Verzeichnispfad des Projektes nicht gespeichert wurde und somit kein Zugriff auf die Dateien möglich war. Ursächlich hierfür war, dass das Projekt bereits in der Datenbank gespeichert war und eine Lösch- bzw. Archiv-Markierung besass. So werden z.B. Projekte, die abgemeldet werden, nicht aus der Datenbank entfernt, sondern erhalten nur eine Lösch-Markierung. Gelöschte bzw. archivierte Projekte sind im CAD nicht sichtbar und können auch nicht bearbeitet werden. Beim Versuch, ein solches Projekt anzumelden, kam es dann zu dem oben beschriebenen Problem.

Beim Anmelden eines Projekets wird nun überprüft, ob bereits einen passenden Datensatz in der Datenbank vorhanden ist, der mit einer Lösch- bzw. Archiv-Markierung versehen ist. In diesem Fall erscheint eine Fehlermeldung.

#### Automatische Adernummerierung

Im CAD gibt es die Möglichkeit zwischen zwei miteinander verbundenen Betriebsmittel automatisch Adersymbole setzen zu lassen. Für die Adernummerierung gibt es eine Vielzahl von Einstellmöglichkeiten, u.a. kann der Anwender die Nummerierungsart und die Nummerrierungsfolge bestimmen. In der Kombination der Numerierungsart "Blatt/Pfadweise" und der Nummerierungsfolge "links-rechts/oben-unten" wurde beim Wechsel des Pfades immer mit der ersten zu vergeben Adernummer gestartet, auch wenn in dem Pfad oberhalb des zu beschriftenden Adersymbols bereits Adernummern vergeben waren.

Der Fehler ist korrigiert.

#### BmK-Rahmen in der Auswertung

Im CAD besteht die Möglichkeit mit Hilfe von BmK-Rahmen Teile eines Blattes einem anderen Anlagen- bzw. Ortskennzeichen zuzuordnen. Bei der Auswertung wurde die Ebenen-Zuordnung der BmK-Rahmen nicht in allen Fällen korrekt berücksichtigt, so dass falsche Querverweise generiert worden sind.

Der Fehler ist korrigiert.

#### Artikel/Symbol setzen

In der Funktion Artikel/Symbol setzen wurden Material, Leistungen und Dummys wechselweise in voneinander getrennten Listen angezeigt. Eine gemeinsame Liste der unterschiedlichen Stammdaten konnte nicht angezeigt werden. 

Der Dialog wurde vollständig überarbeitet, so dass nun alle Stammdaten zusammen in einer Liste angezeigt werden. Darüberhinaus wurden einige Änderungen im Handling des Dialoges vorgenommen, um den neuen Anforderungen gerecht zu werden und die Bedienung einfacher und transparenter zu gestalten.

#### Makro 3spsbgtd.mac

Mit dem Makro 3spsbgtd.mac werden SPS Baugruppen mit Teildarstellungen definiert. Der Dialog konnte weder mit der Eingabe-Taste noch mit der Taste [ESC] beendet werden. Die Schaltflächen "Kopieren" und "Einfügen" funktionierten ebenso nicht. Im Dialog "Symboltexte automatisch beschriften" konnte immer nur ein Element der Liste mit einem Doppelklick der linken Maustaste in den Editier-Modus gebracht werden. Hierbei flackerte das im Hintergrund liegende Listenelement. Auch dieser Dialog konnte weder mit der Taste [Einagbe] oder [Esc] beendet werden.

Die Funktionen "Kopieren" und "Einfügen" im Dialog "Parameter SPS-Komponente" sind entfernt worden, da sie auf der aktuellen Datenbankstruktur nur mit einem erheblichen Aufwand abzubilden sind. Als Alternative bietet sich an, zunächst eine Kopie des Artikels anzulegen und diese anschließend zu parametrieren. Hierbei ist zu beachten, dass bei Änderungen der Symbolzuordnungen bei einem kopierten Artikel immer die Funktion "Symboltexte automatisch zuordnen" für die Gesamtdarstellung und für jede Teildarstellung aufgerufen werden muss. Nur so ist sichergestellt, dass nur nur die Texte beschriftet werden, die in den Symbolen als Platzhalter diesen.
Der Dialog "Symboltexte automatisch beschriften" besteht nun im Wesentlichen aus einer Kombination aus einem Eingabefeld und einer Liste. In der Liste werden die möglichen Symboltexte zur Beschriftung angezeigt und im Eingabefeld kann der zu beschriftende Text des markierten Symboltextes eingegeben werden. Mit den Pfeiltasten "nach oben" und "nach unten" sowie mit dem Mausrad kann in der Liste navigiert werden, ohne dass das Eingabefeld den Fokus verliert. Auf diese Weise lassen sich sehr schnell die zu beschriftenden Texte eingeben.

### CAD Stammdaten

#### Parameter Kabel/Leitung

Zur Definition eines Kabels/Leitung werden im CAD den Artkeldaten das Makro 0cables zugeordnet. Beim Betätigen der Schaltfläche "Schaltplan-Parameter" erscheint der Dialog "Parameter Kabel/Leitung", in dem spezifischen Daten für ein Kabel bzw. eine Leitung hinterlegt werden. Bei der Neuanlage müssen zunächst die Anzahl der Adern festgelegt werden, die anschließend in dem Listenfeld "Adern einzeln definieren" dargestellt werden. Wechselte man nun den Fokus auf dieses Listenfeld, wurde dessen Inhalt gelöscht.

Der Fehler ist korrigiert.

### CAD Konverter

#### Maximale Anzahl von Objekten überschritten

Wurde beim Export nach ZNG die maximale Anzahl von Objekten überschritten, so wurde dies dem Benutzer nicht mitgeteilt. Trotz der Meldung "Export erfolgreich!" enthielt die exportierte Zeichnung nicht alle Objekte.

Dem Benutzer wird nun mitgeteilt, dass die maximale Anzahl von Objekten überschritten wird. Dabei besteht die Möglichkeit den Vorgang abzubrechen und nachträglich eine andere Zeichnung als Ziel für den Export, zu wählen. Um diesen Vorgang zu vereinfachen, wurde die Funktionalität des Befehls "Neu zuordnen" erweitert.

#### Schaltflächen bleiben nach Ausführung eines Befehls deaktiviert

Es konnte vorkommen, dass einige Schaltflächen nach der Ausführung eines Befehls nicht wieder aktiviert wurden.

Die betreffenden Schaltflächen werden nun wieder korrekt aktiviert.

#### Ausdehnung von Exportbereich nicht neu berechnet

Es konnte vorkommen, dass die Ausdehnungen von Exportbereichen nicht neu berechnet wurden, wenn Objekte in der Zeichnung verschoben oder gelöscht wurden.

Die Ausdehnungen der Exportbereiche werden nun nach Änderungen an der Zeichnung neu berechnet.

#### Zeichnung falsch vermittelt

Es konnte vorkommen, dass die zu exportierenden Zeichnungen falsch vermittelt wurden, wenn ein Exportbereich im Batch Export Modus für die Steuerungstechnik verändert wurde.

Die zu exportierenden Zeichnungen werden nun korrekt vermittelt.

### Adressverwaltung

#### Hinzufügen von Kunden-/Mitarbeiter- oder Lieferanten-/Herstellerinformationen

In dem Start-Center von Treesoft Office werden ihnen unter anderem auch die zuletzt bearbeiteten Adressen angezeigt. Beim Hinzufügen von Kunden-/Mitarbeiter-/Lieferanten- oder Hersteller-Informationen zu einer Adresse, wurde diese Adresse aber nicht die Liste der zuletzt bearbeiteten Adressen hinzugefügt.

Beim Hinzufügen von Kunden-/Mitarbeiter-/Lieferanten- oder Hersteller-Informationen, wird diese Adresse nun auch in die Liste der zuletzt bearbeitete Adressen hinzugefügt. Somit können Sie jetzt auch auf diese Adressen sehr schnell über das Start-Center zugreifen.

#### Ansprechpartner Anlegen, Vorname wird falsch erkannt

Beim Anlegen eines Ansprechpartners erkennt die Software automatisch den Titel, Anrede, Vorname sowie den Nachnamen und füllt damit die Briefanrede automatisch aus. Bei dem Namen "Frauke", oder "Herrmann" ist es dazu gekommen, dass der Vorname abgeschnitten wurde, da es ebenfalls Bestandteil der Anrede ist.

Dieses Fehlverhalten wurde behoben. Die Briefanrede wird nun auch bei Vornamen, die Teil der Anrede sind richtig gefüllt.

### Mailing

#### Dateianhänge

Beim Versenden einer E-Mail mit Dateianhängen konnte es passieren, dass die Dateianhänge als mailatt* versendet und gespeichert wurden. Dieses konnte nur passieren, wenn die E-Mail aus den Entwürfen geöffnet, dann gedruckt und direkt im Anschluss versendet wurde.

Die E-Mails werden nun auch in der oben genannten Konstellation mit den richtigen Namen für Dateianhänge verschickt und gespeichert.

#### Optimierung der Geschwindigkeit beim Mehrfachversand

Vor einem Mehrfachversand wird ein Filter ausgeführt, der die Datensätze einschränk und die Kommunikation auswählt. Beim Mehrfachversand wurde für jede einzelne Adresse die Adressinformation für die Variablenersetzung erneut mit den kompletten Bedingungen des Filters ausgelesen. Das führte bei komplexeren Filtern dazu, dass zwischen der Bearbeitung jeder E-Mail mehrere Sekunden vergehen konnten.

Beim Auslesen der Adressinformationen für die Variablenersetzung wird nur noch nach der Adress-ID aus dem bereits ausgeführtem Filter die Adresse ausgewählt. Dies ist um einiges schneller und führt - unabhängig von der Komplexität des Filters - zu einer konstanten Zeit je Adresse.

### Stammdaten

#### Parametermakro 0ArtVari

Das Parametermakro 0artvari dient dazu, nach dem Setzen eines Artikels bestimmte Symboltexte automatisch zu beschriften. Bei der Auswahl der Textformate fehlte die Möglichkeit Hilfsvariablen, Betriebsmittelkennzeichen und Kommentartexte zu selektieren. Zudem wurde das Eingabefeld in bestimmten Situationen mit einem Leerzeichen vorbelegt.
Um mehrere Symbolen mit identichen Symboltexten komfortabel zu beschriften dienen die Funktionen "Kopiern" und "Einfügen", die über Schaltflächen in der Toolbar aufgerufen werden können. Die Funktion "Kopieren" erzeugt eine Liste mit den Symboltexten und den anzutragenden Texten. Die Funktion "Einfügen" belegt für jeden in der Liste gefundenen Text die Spalte "beschriften mit" mit dem jeweiligen Inhalt der Liste vor. Mit der Funktion "Textablage" sollte die mit der Funktion "Kopieren" erzeugte Liste im eingestellten Editor bearbeitet werden können. Hierbei wurde allerdings die Liste in einem falschen Verzeichnis gesucht. 

Der Zugriff auf die Liste der kopierten Texte funktioniert wieder. Der Dialog "Mehrzeilige Texte bearbeiten" wird nun modal aufgerufen, d.h. er muss erst beendet werden, bevor ein neuer Text aus der Liste zum Bearbeiten ausgewählt werden kann.
Bei der Auswahl der Textformate können nun gezielt auch Hilfsvariablen, Betriebsmittelkennzeichen und Kommentartexte selektiert werden. Das Eingabefeld wird nicht mehr mit einem Leerzeichen vorbelegt. 
Die gefundenen Symboltexte werden sortiert nach Textformaten in folgender Reihenfolge angezeigt:

- Informationsvariablen
- Ergänzungsvariablen
- Hilfsvariablen
- Betriebsmittelkennzeichen
- Anschlusstexte
- Spiegeltexte
- Kommentarttexte

#### Leistungen, Dummys, Parametermakro wählen

Parametermakros unterscheiden sich von anderen Makros durch spezielle Funktionen. Bei der ersten Auwahl eines Parametermakros (oder durch die Funktion "Aktualisieren" im Dialog "Parametermakro wählen") wird eine Liste mit allen verfügbaren Parametermakros erstellt. Zu diesem Zweck werden alle Makros des Systems einmal geladen und entsprechend überprüft. Hierbei erschienen nacheinander mehrere Meldungen, dass bestimmte Makros nicht gelesen werden konnten.

Der Fehler ist korrigiert.

#### Dialog Parametermakro wählen

Bei einer geringen Auflösung wurde der Dialog Parametermakro wählen zu klein geöffnet. Die Mindesthöhe von diesen Dialogen entsprach einem 5tel (20 %) der verfügnaren Höhe des Bildschirms.

Die Mindesthöhe von diesen Dialogen beträgt nun ein 4tel (25 %) der verfügbaren Höhe des Bildschirms.

#### Schaltfläche Schaltplan Parameter/Schaltschrank Parameter

Artikeln können Parameter für den Schaltplan- bzw. Schaltschrank-Assistenten hinterlegt werden. Zu diesem Zweck kann ein Parameter-Makro ausgewählt werden. Die eingegebenen Parameter werden anschließend in dem jeweiligen Datensatz des Artikels gespeichert, d.h. der Artikel muss hierzu bereits in der Datenbank vorliegen. Bei der Neuanlage von Artikeln waren die beiden Schaltflächen deaktiviert, d.h. es musste zunächst ein Artikel angelegt werden. Erst im Anschluss daran konnten dann die Parameter über ein zugeordnetes Makro eingegeben werden.

Um die Neuanlage von Artikeln zu vereinfachen, können nun bereits beim Erfassen der Artikeldaten Parameter zugeordnet werden. Der Anwender wird hierbei aufgefordert den Datensatz zu speichern, damit die einzugebenden Parameter ein zu Hause haben.

#### Schaltfläche Schaltplan Parameter

Dummys können Parameter für den Schaltplan-Assistenten hinterlegt werden. Zu diesem Zweck kann ein Parameter-Makro ausgewählt werden. Die eingegebenen Parameter werden anschließend in dem jeweiligen Datensatz des Dummy gespeichert, d.h. der Dummy muss hierzu bereits in der Datenbank vorliegen. Bei der Neuanlage von Dummys war die Schaltfläche deaktiviert, d.h. es musste zunächst ein Dummy angelegt werden. Erst im Anschluss daran konnten dann die Parameter über ein zugeordnetes Makro eingegeben werden.

Um die Neuanlage von Dummy zu vereinfachen, können nun bereits beim Erfassen der Dummy-Daten Parameter zugeordnet werden. Der Anwender wird hierbei aufgefordert den Datensatz zu speichern.

#### Dummys anlegen

Dummys dienen im Treesoft CAD als Platzhalter für querverweisrelevante Bauteile. Über die Anzahl und die Art der tatsächlich zugeordneten Kontakte im Schaltplan ermittelt das System während der Auswertung den einzusetzenden Kontaktspiegel, indem es von den beim Dummy hinterlegten Kontaktkombinationen die optimale Kontaktkombination ermittelt und den jeweils zugeordneten Artikel in den Schaltplan einsetzt. Die Reihenfolge, in der die Kontaktkombinationen beim Dummy hinterlegt wurden, spielt dabei eine entscheidene Rolle. Aus diesem Grunde gibt es die Möglichkeit die Kontaktkombination sortieren zu lassen. Wurde diese Funktion bei der Neuanlage eines Dummys aufgerufen, wurden alle weiteren Eingabefelder gelöscht.

Der Fehler ist korrigiert.

#### Material, Leistung und Dummy

In den Stammdaten-Dialogen gab es die Schaltflächen "Makro wählen". Beim Betätigen dieser Schaltfläche wurden alle Makros des Systems zur Auswahl angeboten. Den Stammdaten können aber nur bestimmte Makros zugeordnet werden, sogenannte Parameter-Makros. Diese werden über die Schaltfläche "Schaltplan-Parameter" bzw. "Schaltschrank-Parameter" ausgewählt. 

Die oben genannten Schaltflächen wurden entfernt.

### Offene Posten Verwaltung

#### Auswahl eines Malings im Mahnlauf

Wir haben die Auswahl-Dialoge für Mailings, Filter und Texte neu entwickelt und in Treesoft Office integriert. Seit dieser Integration war beim Ausführen eines Mahnlaufs nicht mehr möglich über die Schaltfläche "..." ein Mailing zu wählen oder zu ändern. Die Änderung oder die Auswahl eines Mailings konnte nur noch in dem Optionen-Dialog > Grundlagen > Mahnwesen > Mahnlauf vorgenommen werden.

Ab sofort kann man auch in dem Fenster für den Mahnlauf ein Mailing auswählen.

### ERP Dokumente

#### Programmabbrüche bei Vorschau/Drucken und Buchen

Beim Aufruf der Vorschau/des Drucks und des Buchens eines Dokuments wurde das Programm in den meisten Fällen mit einer Fehlermeldung abgebrochen.

Wir haben die letzten Änderungen erstmal wieder aus dem ERP entfernt und werden den Programmabbruch genauer analysieren. Damit funktioniert die Vorschau/der Druck und das Buchen von ERP-Dokumenten wieder wie vorher.

### Installation

#### Synchronisation bleibt hängen, wenn eine Datei ohne Dateiendung gefunden wird

Die Synchronisation der lokalen Netzwerkinstallation konnte hängen bleiben, falls eine Datei mit einer leeren Dateiendung über einem UNC-Pfad abgerufen wurde.

Die Synchronisation erkennt nun auch Dateien ohne Dateiendung und wird wie erwartet ausgeführt.

### System

#### Globale Tastenkombinationen

Im TreesoftOffice gibt es einige globale Tastenkombinationen, die einen schnellen Wechsel zwischen verschiedenen Fenstern/Funktionen der Software erlauben. Im CAD waren nur wenige davon implementiert. Hier bestand nur die Möglichkeit, die Funktionen über das Menü "Fenster" aufzurufen.

Nachfolgend eine Liste der im CAD implementierten globalen Tastenkombinationen:

- [Umschalt]+[Strg]+[F3] = Startcenter
- [Umschalt]+[Strg]+[P] = Projekte
- [Umschalt]+[Strg]+[A] = Adressen
- [Umschalt]+[Strg]+[H] = Historie
- [Umschalt]+[Strg]+[D] = Termine
- [Umschalt]+[Strg]+[T] = Aufgaben
- [Umschalt]+[Strg]+[C] = Kalender
- [Umschalt]+[Strg]+[E] = E-Akte
- [Umschalt]+[Strg]+[L] = Fensterliste

#### Erkennung von Windows 10

Ab den 29.07.2015 stellt Microsoft das Betriebssystem Windows 10 zur Verfügung.

Solange wir Treesoft Office noch nicht offiziell für Windows 10 freigegeben haben erscheint beim Programmstart ein Hinweis.

### Mobile Anbindung

#### Suche im Tagesplaner

Im Tagesplaner gibt es eine Suchfunktion zum Filtern der angezeigten Daten, wie in allen anderen Listen der App auch. Hier wurde aber die Suche nicht durchgeführt, weshalb es keine sichtbare Veränderung an der Liste gab.

Es ist nun möglich, im Tagesplaner wie gewohnt zu suchen.

#### Rückmeldung über Ergebnismengen in den Suchfunktionen

Die Suchfunktionen haben keine anständige Rückmeldung über die Ergebnismenge gegeben, wenn es keine Übereinstimmung gefunden wurde.

Es wird nun in der Mitte der Liste eine Meldung mit "Keine Daten" angezeigt, sobald keine Ergebnisse zu dem Suchmuster geliefert werden.

#### Volltextsuche

Bei jedem Tastendruck wurde eine Suchanfrage geschickt, bei zu schnellem Tippen wurde der Benutzer ggf. in den Login Bildschirm gebracht.

Die Volltextsuche wird nun erst nach 0.5 Sekunden nach dem Aufhören des Tippens ausgeführt, wie man es in TreesoftOffice auch gewohnt ist.

#### Nachladen der Adressen in der Volltextsuche

In der Volltextsuche war fest vorgegeben, dass vom Suchergebnis nur die ersten 25 Ergebnisse angezeigt werden.

Es ist nun möglich in der Volltextsuche, die Ergebnisse der Suche nachzuladen und somit nicht nur die ersten 25 Ergebnisse anzeigen zu lassen.

### Treesoft Backup Manager

#### Validierung der Datenbank-Sicherung

Bisher wurden bei der Datenbank-Sicherung mit dem Treesoft Backup Manager die Datenbank über Firebird gesichert. Eine Validierung der erstellten Sicherung gab es nicht.

Ab der Version 6.4 wird bei der Erstellung einer Datenbank-Sicherung direkt eine Validierung der Datenbank-Sicherung durchgeführt. Damit ist sichergestellt, dass für den Fall einer Wiederherstellung die erstellte Sicherung bereits einmal getestet wurde und funktioniert.

### Plug-in Manager

#### Überprüfung ob ein Plug-in kompatibel ist

Bisher war es unabhängig von der Treesoft Office Version in der ein Plug-in erstellt wurde, möglich ein Plug-in in jede Treesoft Office 6.x Version zu installieren. Das ist zwar eins der größten Vorteile aber auch gleichzeitig ein sehr großes Fehlerpotenzial. Mit der Version 6.4 läßt sich kein einziges Plug-in, dass in einer früheren Version erstellt wurde importieren, da der Firebird-Server das Encoding sehr genau nimmt und alle älteren Plug-ins hier einiges durcheinander gebracht haben.

Der Treesoft Plug-in Manager prüft nun ob das Plug-in von der Version kompatibel ist. Wenn man in der Version 6.4 versucht ein Plug-in zu importieren, dass mit einer vorherigen Version erstellt wurde, dann wird das Import verhindert.

## 6.4.15

### CAD Konverter

#### Anlage von Exportbereich nicht möglich

Es konnte vorkommen, dass die Anlage eines Exportbereiches im Model Space Layout mit der Meldung "Es können keine Exportbereiche in einem Paper Space Layout angelegt werden." verweigert wurde.

Das Model Space Layout wird nun auch als solches erkannt.

### Adressverwaltung

#### Steuerkennzeichen und Zahlungsbedingung aus Kundenstamm übernehmen

Auf dem Kundeninformationen-Register in einer Adresse kann ein Benutzer für das Steuerkennzeichen und die Zahlungsbedingungen über ein Optionsfeld hinterlegen, dass diese bei der Anlage eines ERP-Dokuments Standardmäßig ausgewählt ist. Bisher konnte man das Optionsfeld auch aktivieren, wenn kein Steuerkennzeichen oder keine Zahlungsbedingung ausgewählt wurde. Das führte dann bei der Anlage eines ERP-Dokuments in einigen Fällen zu einem unerwarteten Programmabbruch.

Beim Aktivieren dieser Optionsfelder für Steuerkennzeichen und Zahlungsbedingungen stellen wir nun sicher, dass vorher ein Steuerkennzeichen oder eine Zahlungsbedingung ausgewählt wurde.

#### Anzeige des Betreffs des Termins oder der Aufgabe in den Wiedervorlagen

In den Wiedervorlagen der Adressen wurde das Beginnt am, die Hauptgruppe und Gruppe der Aufgabe oder des Termins angezeigt. Für den besseren Überblick bei Adressen mit mehreren Aufgaben oder Terminen fehlte die Anzeige des Betreffs der jeweiligen Aufgabe oder des Termins.

In der Wiedervorlage der Adressen wird für die bessere Übersicht nun auch noch die Spalte "Betreff" der Aufgabe oder des Termins angezeigt. Da durch diese neue Spalte die ausgelieferte Spaltensortierung angepasst werden muss, wird die Spaltensortierung der Adressliste mit diesem Update auf den Auslieferungszustand zurückgesetzt. Der Benutzer kann bei Bedarf aber die Spaltenreihenfolge nach dem Update wieder definieren.

#### Einträge duplizieren

Aus den Listen in der Adressverwaltung ist es möglich einen Eintrag zur aktuellen, einer anderen oder zu einem Projekt zu duplizieren. Im Hauptmenü zu den Einträgen in der Adressverwaltung fehlt dieser Eintrag. Hier ist es nur möglich einen Historien-Eintrag zu duplizieren, aber nicht Termine und Aufgaben.

Das Hauptmenü in der Adressverwaltung zu den Einträgen wurde erweitert. Es ist nun möglich, Einträge genauso wie aus den Listen heraus zu duplizieren.

### ERP

#### Programmabbruch beim Aufruf der Dokumenten- oder Positions-Einstellungen

Im Treesoft Office kann man in dem Kundeninformationen zu einer Adresse Standard-Einstellungen für Zahlungsbedingungen und Steuerkennzeichen festlegen. Wenn man bei der Anlage eines Dokuments die Optionen "Zahlungsbedingungen vom Kunden übernehmen" oder "Steuerkennzeichen vom Kunden übernehmen" ausgewählt hat und in den Kundeninformationen der Adresse waren keine hinterlegt, dann führte es bei dem Hinzufügen von Positionen und beim Aufruf der Einstellungen von einer Position und dem Dokument zu einem unerwarteten Programmabbruch.

Bei der Auswahl der Optionen wird nun geprüft, ob die Informationen bei der jeweiligen Adresse hinterlegt sind. Wenn nicht dann hat der Benutzer die Möglichkeit zur Adresse zu wechseln und das zu Ändern oder diese Option nicht zu verwenden.

### Einträge

#### Aktualisieren des Kalenders nach Änderung in einem Termin oder einer Aufgabe

Der Kalender hat sich nicht automatisch aktualisiert, wenn eine Aufgabe oder ein Termin aus einer anderen Programmstelle heraus bearbeitet wurde.

Der Kalender aktualisiert sich beim Speichern von Aufgaben und Terminen nun automatisch und zeigt die Aufgaben und Termine korrekt an.

### ERP-Schnittstelle

#### Unterstützung der Sage New Classic 2016

Es wurde die Sage New Classic 2016 (Version 5.3.4) per Live-Update zur Verfügung gestellt.

Treesoft Office unterstützt als ERP-Schnittstelle jetzt auch die Version 2016.

## 6.4.14

### Mailing

#### Namen der Dateianhänge in E-Mails

Beim Versenden von E-Mails über den E-Mail-Editor kann man Dateien von der Festplatte auswählen und die als Anhang der E-Mail zuordnen. Bisher konnte es passieren, dass der Dateiname in der versendeten E-Mail aber anders lautete wie der im E-Mail-Editor angezeigt wurde. Der Inhalt der Datei war aber immer richtig.

Wir stellen nun sicher, dass die Namen die im E-Mail-Editor für Dateianhänge angezeigt werden, auch tatsächlich beim Verschicken verwendet werden.

### Stammdaten

#### Aufbauzeit der Materialliste

Seit der Umstellung des Datenbankservers auf Firebird 2.5 kam es bei Kunden mit Materialkatalogen von ca. 400.000 Datensätzen zu einer spürbaren Verlängerung der Aufbauzeit der Liste.

Der Aufbau der Liste wurde durch eine Optimierung am SQL-Statement beschleunigt, und ist nun messbar schneller als mit Firebird 2.1.

### Start-Center

#### Einstellungen der Widgets gehen verloren

Die Spalteneinstellungen der Widgets im Start-Center konnten verloren gehen und wurden auf einen Default zurückgesetzt.

Die Spalteneinstellungen der Widgets im Start-Center werden nun korrekt gespeichert und wiederhergestellt.

## 6.4.13

### CAD Konverter

#### Absturz beim Export nach ZNG

Unendliche Linien (Xlines) konnten beim Export von DWG-/DXF-Zeichnungen nach ZNG zum Absturz der Software führen.

Xlines werden nun beim Export berücksichtigt und führen nicht mehr zum Absturz der Software.

### Notifier

#### Datumsanzeige von Aufgaben und Terminen

Die Bezeichnung des Datums im Notifier von Aufgaben und Termine führte in einigen Fällen zur Verwirrung. Es war nicht direkt ersichtlich, ob sich das Datum auf das Erstellungsdatum oder dem Beginnt-Am Datum der Aufgabe bezieht.

Die Bezeichner für Aufgaben und Termine wurden überarbeitet. Die ToolTips wurden ebenfalls um weitere Informationen ergänzt.

#### Verknüpfte Adressen zu Aufgaben werden nicht angezeigt

Wenn sich Adressen außerhalb vom Notifier verändern, kann es dazu führen, dass die Anzeige im Notifier nicht korrekt aktualisiert wird.

Der Notifier versucht nun, für ihn alle bekannten Informationen zu überwachen und alle Änderungen live anzuzeigen. Aufgrund von zeitkritischen Umständen kann es in Einzelfällen immer noch dazu führen, dass eine geänderte Adresse immer noch mit der alten Bezeichnung angezeigt wird. Nach einem einmaligen Aktualisieren sind die Informationen in jedem Fall aktuell und es bedarf kein Neustart des Notifiers mehr zum Lösen dieses Umstandes.

### Einträge

#### E-Mail Eingang und E-Mail Ausgang

In vereinzelten Fällen konnte es dazu führen, dass die Liste der E-Mails leer ist, aber ein Datensatz im Vorschaufenster angezeigt wurde.

Die Liste der E-Mails und das Vorschaufenster verhalten sich nun synchron zueinander und zeigt keine falschen Datensätze an.

### ERP

#### Übernahme von vorgeschlagenen Rechnungsbeträgen

Wurde eine Rechnung mit Skonto erstellt, und sollte der vorgeschlagene Zahlungseingang ohne Skonto übernommen werden, obwohl der Skontoabzug möglich war, wurde trotzdem der Skonto immer abgezogen.

Jetzt werden die bei der Übernahme angeklickten Werte aus der vorgeschlagenen Zeile korrekt übernommen.

### Mobile Anbindung

#### HTTP Verbindung

Durch ein iOS Update wurden die Standard-Richtlinien bezüglich Verbindungen zu Servern geändert. Standardmäßig werden nun HTTP-Verbindungen blockiert und nur HTTPS zugelassen.

Es ist nun wieder möglich, eine Verbindung über das HTTP-Protokoll herzustellen.

## 6.4.12

### CAD Schaltplan-Assistent

#### Artikel mit dem Parametermakro 0artvari zuordnen

Das Parametermakro 0artvari dient dazu, nach der Auswahl eines Artikels bestimmte Symboltexte automatisch zu beschriften. Wenn die Funktion "Artikel einzeln zuordnen" aus dem Menü gewählt wurde und aus der anschließend angezeigten Auswahlliste ein Artikel mit einem Doppelklick ausgewählt wurde, dem das Makro 0artvari zugeordnet ist, wurden keine Symboltexte beschriftet.

Der Fehler ist korrigiert.

### CAD Konverter

#### Fehler beim Import von ZNG Zeichnung

Der Import von ZNG Zeichnungen wurde mit einer Fehlermeldung abgebrochen, wenn die Zeichnung Texte mit negativer Höhe enthielt.

Texte mit negativer Höhe führen nicht mehr zum Abbruch des Imports. Zusätzlich besteht nun die Möglichkeit einzustellen ob Texte mit negativer Höhe exportiert werden sollen.

### Einträge

#### Rechte bei Einträgen

Mit der Rechteverwaltung von Treesoft Office kann man die Sichtbarkeit von Einträgen einschränken. Wenn man den Historien-Eintrag über den Bearbeiten-Stift im Treesoft Notifier oder den Anrufdialog in der Adressverwaltung erstellt hat, dann wurden keine Rechte für den Eintrag gesetzt, sodass dieser Eintrag für jeden sichtbar war.

Bei dem Protokollieren von Gesprächen über den Anrufdialog oder dem Treesoft Notifier werden nun die Rechte nach der folgenden Regel gesetzt. Es werden die Default-Rechte der Adressen mit der Rufnummer additiv zusammengesetzt, und wenn sich der aktuelle Benutzer in einem der Rechte explizit oder in einer Gruppe befindet, dann werden die kumulierte Default-Rechte gesetzt, ansonsten ist der Eintrag öffentlich und für jeden sichtbar.

### Mailing

#### Rechte beim E-Mail-Eingang

Mit der Rechteverwaltung von Treesoft Office kann man die Sichtbarkeit von Einträgen einschränken. In einigen Umständen wurden die Rechte für die E-Mails nicht wie erwartet und definiert gesetzt, sodass diese Einträge für jeden sichtbar waren.

Bei dem E-Mail-Eingang werden nun die Rechte nach der folgenden Regel gesetzt. Wenn es Default-Rechte bei den Adressen mit der Absender-E-Mail-Adresse gibt, dann werden diese und die Benutzer die in AN und CC benannt wurden additiv zusammengesetzt und der E-Mail zugewiesen. Wenn es keine Default-Rechte bei den Adressen gibt, dann bleibt die E-Mail öffentlich. Nur wenn keine Adresse im CRM gefunden wird, dann wird das Default-Recht des E-Mail-Kontos ausgelesen und wenn es nicht öffentlich ist dann additiv mit den Benutzern in AN und CC der E-Mail zusammengesetzt und der E-Mail zugewiesen, ansonsten ist die E-Mail öffentlich.

## 6.4.11

### CAD Konverter

#### Nur ein Exportbereich einer Zeichnung wird exportiert

Es wurde immer nur ein Exportbereich einer Zeichnung exportiert, egal wie viele Exportbereiche angelegt wurden.

Es werden nun wieder alle angelegten Exportbereiche exportiert.

#### Fehlerhafter Export/Import von mehrzeiligen Texten

Bisher wurde die Position von mehrzeiligen Texten sowohl beim Import als auch beim Export nicht angepasst. Dadurch konnte es vorkommen, dass Zeilenvorschübe nach oben, Ausrichtung links/rechts unten oder Drehungen die Darstellung von Texten nach der Konvertierung verändern.

Nach der Konvertierung von und zu DWG/DXF sollten mehrzeilige Texte nun optisch dem Original entsprechen.

#### Zeichnung auf Ausdehnung gezoomed öffnen

Wurde eine in das DWG/DXF Format konvertierte ZNG Datei in einem CAD-Programm eines Dritthersteller geöffnet, musste auf die Zeichnungsausdehnung gezoomed werden, um die Zeichnung betrachten zu können.

Bei der Konvertierung werden nun entsprechende Parameter gesetzt, sodass die ins DWG/DXF Format konvertiert Zeichnung in Dritthersteller Programmen direkt betrachtet werden können.

#### Fensterposition wird gespeichert

Bisher wurden keine Positionen von den Fenstern und Dialogen gespeichert.

Sowohl das Hauptfenster als auch der Exportdialog speichern und restaurieren nun die Positionen.

#### Mehr Arbeitsspeicher ansprechbar

Bisher konnte der CAD Konverter, selbst in einem 64 Bit Betriebssystem, nur bis zu 2 GiB des zur Verfügung stehenden Arbeitsspeichers ansprechen.

Der CAD Konverter kann nun bis zu 4 GiB des zur Verfügung stehenden Arbeitsspeichers, in einem 64 Bit Betriebssystem, ansprechen.

#### Fehlerhafte Positionierung bei bidirektionalem Import

Die Positionierung der Objekte konnte auf der Y-Achse abweichen, wenn die Konfigurationsdatei mit der Version 6.4.8 oder früher erstellt oder der exportierte Grundriss verschoben wurde.

In beiden Fällen werden die Objekte nun korrekt positioniert.

### Start-Center

#### Menü-Blöcke CAD/CRM/ERP via Einstellung im Optionendialog Ein-/Ausblenden

Im Startcenter waren die Hauptmenüs CAD, CRM und ERP immer eingeblendet.

Jeder Benutzer hat nun die Möglichkeit die einzelnen Menüs und Programmteile ein und auszublenden. Hierzu wurde im Optionen-Dialog im Bereich Grundlagen unter dem Zweig Start-Center eine Registerkarte hinzugefügt um die Menü-Blöcke, zu konfigurieren.

### Notifier

#### Aufruf eines Projekts

Der Notifier bietet keine Möglichkeit, ein Projekt aus einer angezeigten Aufgabe oder Termin aufzurufen.

Es ist nun mittels Kontext-Menü möglich, die verknüpften Projekte aus einer angezeigten Aufgabe oder Termin aufzurufen. Zudem ist es möglich, ein neues Projekt einer Aufgabe oder einem Termin zuzuweisen.

### Einträge

#### Anzeige der Kürzel in der Spalte IDs

In der Liste der Einträge werden in der Spalte IDs die Kürzel der zugewiesenen Ansprechpartner angezeigt. Hatten zwei Ansprechpartner das gleiche Kürzel wurde es nur einmal angezeigt, obwohl mehrere Ansprechpartner mit dem Eintrag verknüpft sind.

Es werden jetzt alle Kürzel der zugeordneten Ansprechpartner angezeigt, auch wenn sich diese dadurch doppeln. Dadurch kann man aber in der Liste leichter sehen ob einer oder mehrere Ansprechpartner verknüpft sind.

## 6.4.10

### Projektverwaltung

#### Programmende beim Verändern der Einstellungen eines Projektes

Bei Inaktivität oder bei einer längeren Bearbeitung der Einstellungen eines Projektes, konnte es dazu kommen, dass sich die Software automatisch mit der Fehlermeldung "invalid BLOB id." beendet.

Die Projektliste, sowie die Einstellungen eines Projektes werden nun aktuell gehalten, somit kann eine längere Bearbeitung der Einstellungen nicht mehr zu dem Zustand "invalid BLOB id." führen.

### Mobile Anbindung

#### Stabilität der Volltextsuche verbessert

Bei stark frequentierten oder parallelen Anfragen an die Volltextsuche konnte es vorkommen, dass der Mobile Agent Volltextsuchanfragen verweigerte.

Der Mobile Agent ist nun darauf vorbereitet, stark frequentierte und parallele Volltextsuchanfragen zu verarbeiten.

### CAD Plug-in

#### Neuer Treesoft CAD Symbolkatalog QIVICON

QIVICON ist eine Initiative der Deutschen Telekom AG mit führenden deutschen Industrieunternehmen. QIVICON ermöglicht die hersteller- und markenübergreifende Vernetzung eines Smart Homes.

Mit dem neuen Treesoft CAD Symbolkatalog Qivicon stellen wir Ihnen die Artikel und Symbole von Heimautomatisierungen des Herstellerkonsortiums QIVICON zur Projektierung in der Gebäudetechnik zur Verfügung.

## 6.4.9

### Notifier

#### Anzeige der Adressen bei Anrufen

Welche Informationen der gefundenen Adresse im Notifier angezeigt werden, kann man im Optionen-Dialog > Grundlagen > Computertelefonie einstellen, Standard ist Name1 und Ansprechpartner. Bei Anrufen - egal ob eingehend oder ausgehend - von Rufnummern die Personen-Adressen hinterlegt sind, wurde "Es ist keine Adresse mit diesem Eintrag verknüpft" angezeigt obwohl die Rufnummer bei einer Adresse hinterlegt war.

Mit diesem Update wird auch in dieser Konstellation der Name der Adresse wieder angezeigt.

### Mobile Anbindung

#### Gelöschte Adressen werden angezeigt

In der Volltextsuche, sowie bei den Adressen wurden gelöschte bzw. archivierte Adressen angezeigt.

Gelöschte bzw. archivierte Adressen werden nun nicht mehr in der Volltextsuche angezeigt.

#### Fehlerhafte Anzeige in den Kommunikationen/Info zu einem Ansprechpartner

Beim Auswählen eines Ansprechpartners, wurden von einem anderen Ansprechpartner die Daten zum jeweiligen Ansprechpartner angezeigt.

Es werden nun die richtigen Informationen zum Ansprechpartner angezeigt.

#### Benutzen der Volltextsuche

Beim Benutzen der Volltextsuche durch ein mobiles Endgerät konnte es bei zu vielen Suchergebnissen dazu kommen, dass der Mobile Agent auf keine weitere Anfrage eines Clients antwortete.

Der Fehler der dazu führte wurde korrigiert. Die Volltextsuche funktioniert nun auch bei vielen Ergebnissen im Mobile Agent.

### CAD Plug-in

#### Neuer Treesoft CAD Symbolkatalog Loxone Smart Home

Im Loxone Smart Home steuert ein zentrales Gerät - der intelligente Loxone Miniserver - alles. Von der Beschattung über die Musik bis hin zur Heizung.

Mit dem neuen Treesoft CAD Symbolkatalog Loxone Smart Home stellen wir Ihnen die Artikel und Symbole von Loxone Smart Home zur Projektierung in dem SPS-Assistenten zur Verfügung.

#### Neuer Treesoft CAD Symbolkatalog WAGO-I/O-System

Modulares WAGO-I/O-SYSTEM, IP20 (Serie 750/753). Das für vielfältigste Anwendungsgebiete zugelassene WAGO-I/O-SYSTEM trägt mit seinem feinmodularen und feldbusunabhängigen Design den Anforderungen an dezentrale Feldbussysteme besonders Rechnung.

Mit dem neuen Treesoft CAD Symbolkatalog WAGO-I/O-System stellen wir Ihnen die Artikel und Symbole zur Projektierung des modularen WAGO-I/O-Syxstems, IP20 (Serie 750/753) zur Verfügung.

## 6.4.8

### System

#### Unterstützung für Windows Server 2003 und Server 2003 R2 eingestellt

Am 14.07.2015 hat Microsoft den erweiterten Support für Windows Server 2003 und Windows Server 2003 R2 eingestellt.

Mit dem Ende des Supports von Microsoft beenden auch wir die Unterstützung für das Server-Betriebssystem.

## 6.4.7

### CAD Konverter

#### Öffnen des CAD-Konverters nach dem Hinzufügen mehrerer Dateien

Beim Hinzufügen von DWG-/DXF-Dateien zu einem Projekt wurde anschließend der CAD-Konverter mit diesen Dateien geöffnet. Wenn die zu öffnenden Dateien in einem Pfad mit Leerzeichen lagen, dann wurde zwar der CAD-Konverter gestartet, die hinzugefügten Dateien aber nicht geöffnet.

Nach dem Hinzufügen von DWG-/DXF-Dateien zu einem Projekt wird der CAD-Konverter auch bei Dateien in deren Pfad Leerzeichen vorkommen gestartet und die übergebenen Dateien direkt geöffnet.

### Projektliste

#### Sortieren nach Ersteller oder Benutzer

Mit der Version Treesoft Office 6.4 führte das Sortieren nach dem Ersteller oder Benutzer in der Projektliste dazu, dass keine Ergebnisse angezeigt wurden. Stattdessen wurde immer nur das "Einen Moment bitte..." angezeigt.

Ab sofort ist es, wieder möglich in der Projektliste auch nach dem Ersteller oder Benutzer zu sortieren.

### System

#### Aufruf der Funktion "Textformat"

Wenn in der Funktion "Fremdsprachenübersetzung" die Funktion "Textformat" gestartet und beendet worden ist, wurde dieser Dialog bei einer Bewegung des Fadenkreuzes immer wieder zur Anzeige gebracht.

Der Fehler ist korrigiert.

## 6.4.6

### Stammdaten

#### Leistungen: Parameter-Makro

Wenn einer neu angelegten Leistung ein Parameter-Makro zugeordnet wurde, wurde dieses nicht gespeichert.

Der Fehler ist korrigiert.

## 6.4.3

### CAD Schaltplan-Assistent

#### Maximale Aderanzahl bei Kabeldefinitionen

Bisher konnten nur Kabel mit maximal 120 Adern definiert werden.

Die maximale Aderanzahl je Kabeldefinition wurde auf 500 erhöht.

## 6.4.2

### System

#### Treesoft Office an Taskleiste in Windows anheften

Für einen schnelleren Start von Programmen werden in Windows gerne die häufig genutzten Programme an die Taskleiste angeheftet. Auf einem Arbeitsplatz einer Client-\Server-Installation von Treesoft Office war das aber nicht möglich, das Kontextmenü zeigte ausschließlich den Punkt "Fenster schließen" an. War Treesoft Office aber auf einem Einzelplatz installiert, konnte man Treesoft Office an die Taskleiste anheften.

Ab dieser Version ist es nun auch auf einem Arbeitsplatz im Client-\Server-Betrieb möglich, Treesoft Office an die Taskleiste anzuheften.
