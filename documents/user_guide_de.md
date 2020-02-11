
# User Guide für das idealo 2.0 Plugin

<div class="container-toc"></div>


## 1 Über idealo

Im Jahr 2000 mit der Mission gestartet, Nutzern zu helfen, richtige Kaufentscheidungen zu treffen, zählt idealo mit 50.000 Händlern und rund 18 Millionen Nutzern pro Monat zu den relevantesten deutschen E-Commerce-Websites.<br/>

Mit idealo Direktkauf bietet idealo einen starken Vertriebskanal. Der "Zum Kauf"-Button ermöglicht es Nutzern, das Produkt direkt über eine vollintegrierte Checkout-Funktion über idealo zu bestellen. Vertragspartner sind dabei stets die Händler selbst, die auch wie gewohnt das Fulfillment übernehmen.<br/>

#### idealo Preisvergleich und idealo Direktkauf

Mit plentymarkets können sowohl der idealo Preisvergleich als auch idealo Direktkauf genutzt werden. Mit idealo Direktkauf können Kund*innen deine Produkte direkt bei idealo kaufen, ohne in deinen Webshop zu wechseln.


## 2 Bei idealo registrieren

Um idealo in plentymarkets einrichten zu können, registriere dich zunächst bei idealo als Händler.

<div class="alert alert-warning" role="alert">
<b>Hinweis: Artikeldatenexport</b><br/> Kläre vor der Einrichtung in plentymarkets mit idealo, wie Artikeldaten übertragen werden sollen (Erstellung, Aktualisierung und Löschen von Artikeln auf idealo). Artikeldaten können mit einer CSV-Datei oder per API (PWS 2.0-Schnittstelle) exportiert werden.<br/>
Wenn du PWS 2.0 für den Artikelexport nutzt, werden Artikel einmal täglich auf idealo erstellt und gelöscht. Preise und Bestände werden alle 15 Minuten aktualisiert.<br/>
Wenn du Artikel mit einer CSV-Datei über den elastischen Export zu idealo überträgst, können Artikel über eine URL von idealo abgerufen werden.
 </ul>
</div>


#### 2.1 Plugin Elastischer Export installieren

Um das idealo-Plugin nutzen zu können, musst du zunächst das Plugin [Elastischer Export](https://marketplace.plentymarkets.com/plugins/sales/marktplaetze/elasticexport_4763) in deinem plentymarkets System installieren. Das Plugin erhältst du im [plentyMarketplace](https://marketplace.plentymarkets.com/).

## 3 idealo-Assistent durchlaufen

Durchlaufe zunächst den Assistenten **idealo Grundeinstellungen** im Menü **Einrichtung » Assistenten » Omni-Channel**, um die Grundeinstellungen für idealo in plentymarkets vorzunehmen. Mit diesem Assistenten richtest du dein idealo-Konto in plentymarkets ein und nimmst Einstellungen für den Artikeldatenxport zu idealo und Auftragsimport von idealo Direktkauf vor.<br/>

<div class="alert alert-warning" role="alert">
<b>Hinweis: Artikelexport per API</b><br/>Wenn du deine Artikel über PWS 2.0 exportierst, ist es zwingend erforderlich, den <b>idealo Grundeinstellungen</b>>-Assistenten zu durchlaufen, da der automatische Artikelexport nur im idealo-Assistenten eingestellt werden kann. 
 </ul>
</div>

#### idealo Preisvergleich und idealo Direktkauf nutzen

Je nachdem, ob du nur den idealo Preisvergleich nutzen möchtest oder deinen Kunden auch die Möglichkeit bieten möchtest, deine Artikel direkt bei idealo zu kaufen, ohne in deinen Webshop wechseln zu müssen, sind unterschiedliche Einstellungen nötig. Im Folgenden erhältst du eine Übersicht zu den nötigen Einstellungen für idealo Direktkauf.

→ **Einstellungen für idealo Direktkauf:**
- **Grundeinstellungen:** Durchlaufe im Menü **Einrichtung » Assistenten » Omni-Channel** den Assistenten **idealo Grundeinstellungen**.
- **Artikelexport:** Richte den [automatischen Artikelexport](#Artikelexport per API) oder den [Artikelexport per CSV-Datei](#Artikelexport mit elastischem Export) ein, je nachdem, wie du Artikel zu idealo übertragen möchtest.
- **Auftragsherkunft:** Aktiviere im Menü **Einrichtung » Aufträge » Auftragsherkunft** zusätzlich zur Auftragsherkunft **idealo** auch die [Auftragsherkunft](#Auftragsherkunft aktivieren) **idealo Direktkauf**.
- **Artikelverfügbarkeit:** Aktiviere im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Tab: Varianten-ID » Tab: Verfügbarkeit** im Bereich **Märkte** zusätzlich zur Option **idealo** auch die [Verfügbarkeit](#Artikelverfügbarkeit einstellen) **idealo Direktkauf**.
- **Verkaufspreis:** Richte einen [Verkaufspreis](#Verkaufspreis festlegen) ein.
- **SKU:** Füge marktplatzspezifische [SKUs](#SKU manuell festlegen) hinzu, wenn gewünscht.
- **Zahlungsart:** Richte die [Zahlungsart](#Zahlungsart idealo Direktkauf aktivieren) **idealo Direktkauf** ein.
- **Merkmale:** Erstelle [Merkmale](#Merkmale erstellen) für idealo Direktkauf. Mit Merkmalen überträgst du Artikeleigenschaften, Versandarten und Gebühren an idealo Direktkauf.
- **Ereignisaktionen:** Richte [Ereignisaktionen](#Ereignisaktionen einrichten) ein, um Änderungen am Auftragsstatus automatisch an idealo Direktkauf zu senden.


## 4 Auftragsherkunft aktivieren
<a name="Auftragsherkunft aktivieren"></a>

Damit du Artikel, Merkmale etc. mit dem idealo Preisvergleich verknüpfen kannst, muss im Menü **Einrichtung » Aufträge » Auftragsherkunft** die Auftragsherkunft **idealo** aktiviert werden.

#### Auftragsherkunft für idealo Preisvergleich aktivieren:

1. Öffne das Menü **Einrichtung » Aufträge » Auftragsherkunft**.
2. Setze ein Häkchen bei **idealo**.
3. **Speichere** die Einstellungen.

Wenn du idealo Direktkauf nutzen möchtest, aktiviere zusätzlich die Auftragsherkunft **idealo Direktkauf**. Wenn du die Auftragsherkunft **idealo Direktkauf** aktivierst, wird in der über den elastischen Export generierten CSV-Datei die Spalte **checkout_approved** auf **true** gesetzt.


## 5 Artikelverfügbarkeit einstellen
<a name="Artikelverfügbarkeit einstellen"></a>

Artikel, die du auf dem idealo-Preisvergleichsportal anbieten möchtest, müssen im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Tab: Varianten-ID** im Tab **Verfügbarkeit** aktiviert werden. Stelle die Artikelverfügbarkeit für idealo ein wie im Folgenden beschrieben.

#### Artikelverfügbarkeit für idealo Preisvergleich einstellen:

1. Öffne das Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Tab: Varianten-ID » Tab: Einstellungen**.
2. Aktiviere die Hauptvariante im Bereich **Verfügbarkeit**.
3. Wechsele in das Tab **Verfügbarkeit**.
4. Klicke im Bereich **Märkte** in das Auswahlfeld.<br/>
→ Eine Liste mit allen verfügbaren Märkten wird angezeigt.
5. Aktiviere die Option **idealo**.
6. Aktiviere die Option **Web-API**.
7. Klicke auf **Hinzufügen**.<br/>
→ Der Marktplatz wird hinzugefügt.
8. **Speichere** die Einstellungen.

Die Verfügbarkeit für Varianten kann im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Tab: Varianten » Variante öffnen » Tab: Varianten-ID » Tab: Verfügbarkeit** angepasst werden.

Wenn du idealo Direktkauf nutzen möchtest, aktiviere im Bereich **Märkte** zusätzlich die Option **idealo Direktkauf**.


## 6 Verkaufspreis festlegen
<a name="Verkaufspreis festlegen"></a>

Gehe wie im Folgenden beschrieben vor, um für die Auftragsherkunft idealo einen Verkaufspreis festzulegen. Dieser Preis wird auf idealo angezeigt und ist für den idealo Preisvergleich und idealo Direktkauf gültig.

#### Verkaufspreis für idealo festlegen:

1. Öffne das Menü **Einrichtung » Artikel » Verkaufspreise » Verkaufspreis öffnen » Tab: Einstellungen**.<br/>
→ Wenn du noch keinen Verkaufspreis angelegt hast, klicke auf **Neu**, um einen Verkaufspreis zu erstellen.
2. Setze ein Häkchen bei der Herkunft **idealo**.
3. **Speichere** die Einstellungen.

<div class="alert alert-warning" role="alert">
<b>Hinweis: Mindestpreis</b><br/>Wenn du für die idealo-Preisspanne einen Mindestpreis angeben möchtest, musst du mindestens zwei Verkaufspreise für idealo festlegen, einen Mindestpreis und einen normalen Verkaufspreis. Außerdem muss der Mindestpreis vom Typ <b>Aktionspreis</b> sein und mit der Herkunft <b>idealo Direktkauf</b> verknüpft werden.<br/>
Welcher Preis als Mindestpreis für die idealo-Preisspanne an idealo übertragen werden soll, legst du im idealo-Assistenten im Schritt <b>Artikeldaten</b> mit der Einstellung <b>Welcher Preis soll als Mindestpreis an idealo übertragen werden?</b> fest. 
 </ul>
</div>


## 7 SKU manuell festlegen
<a name="SKU manuell festlegen"></a>

Im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Tab: Varianten-ID im Tab Verfügbarkeit** fügst du, wenn nötig, marktplatzspezifische SKUs hinzu.

#### SKU hinzufügen:

1. Öffne das Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Tab: Varianten-ID » Tab: Einstellungen**.
2. Wechsele in das Tab **Verfügbarkeit**.
3. Klicke im Bereich **SKU** auf **Hinzufügen**.<br/>
→ Das Bearbeitungsfenster **Neue SKU** wird angezeigt.
4. Wähle die Herkunft **idealo**.
5. Gib die SKU ein.
6. Klicke auf **Hinzufügen**.<br/>
→ Die SKU wird gespeichert und angezeigt.

Wenn du idealo Direktkauf nutzen möchtest, füge zusätzlich SKUs mit der Herkunft **idealo Direktkauf** hinzu.


## 8 Artikelexport einrichten

Artikel werden entweder mit dem automatischen Artikelexport über eine API (PWS 2.0-Schnittstelle) oder mit einer CSV-Datei über den elastischen Export zu idealo übertragen. Je nachdem, welche Art der Datenübertragung du wählst, sind verschiedene Einstellungen notwendig.<br/>

→ **Hinweis:** Kläre vor der Einrichtung in plentymarkets mit idealo, wie Artikeldaten übertragen werden sollen.

Informationen zu den verschiedenen Arten der Datenübertragung findest du in der folgenden Tabelle.

_Tab. 1: Datenübertragung bei idealo_

|**Artikelexport per API**                    |**Artikelexport mit elastischem Export** |
|:---                                         |:--- |
|Artikeldatenübertragung per Schnittstelle    |Artikeldatenübertragung per CSV-Datei |
|tägliche Aktualisierung von Artikeln         |Abruf von Artikeldaten per URL, die bei idealo hinterlegt wird |
|Aktualisierung von Preisen alle 15 Minuten   |Intervall, in dem Artikeldaten abgerufen werden, wird von idealo festgelegt |
|Aktualisierung von Beständen alle 15 Minuten | |


### 8.1 Artikelexport per API (PWS 2.0-Schnittstelle)
<a name="Artikelexport per API"></a>

Wenn du deine Artikel per Schnittstelle automatisch zu idealo übertragen möchtest, durchlaufe den Assistenten **idealo Grundeinstellungen** im Menü **Einrichtung » Assistenten » Omni-Channel** und aktiviere den automatischen Artikeldatenexport. Für den automatischen Artikelexport sind außerhalb des idealo-Assistenten keine weiteren Einstellungen in plentymarkets nötig.<br/>

Mit dieser Art der Datenübertragung werden Artikel einmal täglich auf idealo erstellt und gelöscht. Preise und Bestände werden alle 15 Minuten aktualisiert.


### 8.2 Artikelexport mit elastischem Export
<a name="Artikelexport mit elastischem Export"></a>

Wenn du Artikel über den elastischen Export zu idealo überträgst, müssen im Menü **Daten » Elastischer Export** Einstellungen vorgenommen werden, um das Exportformat einzurichten. Als Voraussetzung muss das Plugin [Elastischer Export](https://marketplace.plentymarkets.com/plugins/sales/marktplaetze/elasticexport_4763) in deinem plentymarkets System installiert sein. Damit idealo deine Artikeldaten abrufen kann, lege zunächst das Datenformat IdealoDE an und hinterlege im Anschluss die URL bei idealo.<br/>

Wie du den Artikelexport über den elastischen Export in plentymarkets einrichtest, ist in den folgenden Kapiteln [Das Format IdealoDE-Plugin in plentymarkets einrichten](#Das Format IdealoDE-Plugin in plentymarkets einrichten) und [Verfügbare Spalten der Exportdatei](#Verfügbare Spalten der Exportdatei) beschrieben.


### 8.2.1 Das Format IdealoDE-Plugin in plentymarkets einrichten
<a name="Das Format IdealoDE-Plugin in plentymarkets einrichten"></a>

<div class="alert alert-warning" role="alert">
<b>Hinweis: Einstellungen nur für elastischen Export relevant</b><br/>Die in diesem Kapitel beschriebenen Einstellungen sind nur notwendig, wenn du Artikel über den elastischen Export zu idealo überträgst.
 </ul>
</div>

<div class="alert alert-warning" role="alert">
<b>Hinweis: idealo Produkt-CSV prüfen</b><br/>Zurzeit sind in plentymarkets nicht alle Spalten der idealo Produkt-CSV verfügbar. Prüfe vor der Einrichtung, ob du Produktspalten benötigst, die in plentymarkets noch nicht verfügbar sind. In diesem Fall ist die Einrichtung von idealo zurzeit noch nicht möglich.<br/> Eine Übersicht der in plentymarkets verfügbaren Spalten erhältst du im Kapitel <b>Verfügbare Spalten der Exportdatei</b>.
 </ul>
</div>

Damit deine Artikel mit dem elastischen Export zu idealo übertragen werden können, musst du das Exportformat **IdealoDE** einrichten. Weitere Informationen zum elastischen Export findest du auf der Handbuchseite [Elastischer Export](https://knowledge.plentymarkets.com/daten/daten-exportieren/elastischer-export).

#### Neues Exportformat erstellen:

1. Öffne das Menü **Daten » Elastischer Export**.
2. Klicke auf **Neuer Export**.
3. Nimm die gewünschten Einstellungen vor. Beachte dazu die Erläuterungen in Tabelle 1.
4. **Speichere** die Einstellungen.<br/>
→ Eine ID für das Exportformat **IdealoDE-Plugin** wird vergeben und das Exportformat erscheint in der Übersicht **Exporte**.

In der folgenden Tabelle findest du Hinweise zu den einzelnen Formateinstellungen und empfohlenen Artikelfiltern für das Format **IdealoDE-Plugin**.

_Tab. 2: Formateinstellungen für **IdealoDE**_

| **Einstellung**                                    | **Erläuterung** |
| :---                                               | :--- |
| **Einstellungen**                                  | |
| **Name**                                           | Name eingeben. Unter diesem Namen erscheint das Exportformat in der Übersicht im Tab **Exporte**. |
| **Typ**                                            | Typ **Artikel** aus der Dropdown-Liste wählen. |
| **Format**                                         | **IdealoDE-Plugin** wählen. |
| **Limit**                                          | Zahl eingeben. Wenn mehr als 9999 Datensätze an die Preissuchmaschine übertragen werden sollen, wird die Ausgabedatei wird für 24 Stunden nicht noch einmal neu generiert, um Ressourcen zu sparen. Wenn mehr als 9999 Datensätze benötigt werden, muss die Option **Cache-Datei generieren** aktiv sein.<br/> **Oder:** Wenn du mehr als 9999 Datensätze an idealo übertragen möchtest, kannst du als Alternative auch Version 2.0 des idealo-Plugins installieren. |
| **Cache-Datei generieren**                         | Häkchen setzen, wenn mehr als 9999 Datensätze an die Preissuchmaschine übertragen werden sollen. Um eine optimale Performance des elastischen Exports zu gewährleisten, darf diese Option bei maximal 20 Exportformaten aktiv sein. |
| **Bereitstellung**                                 | **URL** wählen. |
| **Dateiname**                                      | Der Dateiname muss auf **.csv** oder **.txt** enden, damit idealo die Datei erfolgreich importieren kann. |
| **Token, URL**                                     | Wenn unter **Bereitstellung** die Option **URL** gewählt wurde, auf **Token generieren** klicken. Der Token wird dann automatisch eingetragen. Die URL wird automatisch eingetragen, wenn unter **Token** der Token generiert wurde. |
| **Artikelfilter**                                  | |
| **Artikelfilter hinzufügen**                       | Artikelfilter aus der Dropdown-Liste wählen und auf **Hinzufügen** klicken. Standardmäßig sind keine Filter voreingestellt. Es ist möglich, alle Artikelfilter aus der Dropdown-Liste nacheinander hinzuzufügen.<br/> **Varianten** = **Alle übertragen** oder **Nur Hauptvarianten übertragen** wählen.<br/> **Märkte** = **idealo** wählen.<br/> **Währung** = Währung wählen.<br/> **Kategorie** = Aktivieren, damit der Artikel mit Kategorieverknüpfung übertragen wird. Es werden nur Artikel, die dieser Kategorie zugehören, übertragen.<br/> **Bild** = Aktivieren, damit der Artikel mit Bild übertragen wird. Es werden nur Artikel mit Bildern übertragen.<br/> **Mandant** = Mandant wählen.<br/> **Bestand** = Wählen, welche Bestände exportiert werden sollen.<br/> **Markierung 1 - 2** = Markierung wählen.<br/> **Hersteller** = Einen, mehrere oder **ALLE** Hersteller wählen.<br/> **Aktiv** = Nur aktive Varianten werden übertragen. |
| **Formateinstellungen**                            | |
| **Produkt-URL**                                    | Wählen, ob die URL des Artikels oder der Variante an das Preisportal übertragen wird. Varianten URLs können nur in Kombination mit dem Ceres Webshop übertragen werden. |
| **Mandant**                                        | Mandant wählen. Diese Einstellung wird für den URL-Aufbau verwendet. |
| **URL-Parameter**                                  | Suffix für die Produkt-URL eingeben, wenn dies für den Export erforderlich ist. Die Produkt-URL wird dann um die eingegebene Zeichenkette erweitert, wenn weiter oben die Option **übertragen** für die Produkt-URL aktiviert wurde. |
| **Auftragsherkunft**                               | Die Auftragsherkunft **Idealo** wählen. |
| **Marktplatzkonto**                                | Marktplatzkonto aus der Dropdown-Liste wählen. Die Produkt-URL wird um die gewählte Auftragsherkunft erweitert, damit die Verkäufe später analysiert werden können. |
| **Sprache**                                        | Sprache aus der Dropdown-Liste wählen. |
| **Artikelname**                                    | **Name 1**, **Name 2** oder **Name 3** wählen. Die Namen sind im Tab **Texte** eines Artikels gespeichert. Im Feld **Maximale Zeichenlänge (def. Text)** optional eine Zahl eingeben, wenn die Preissuchmaschine eine Begrenzung der Länge des Artikelnamen beim Export vorgibt. |
| **Vorschautext**                                   | Wählen, ob und welcher Text als Vorschautext übertragen werden soll.<br/> Im Feld **Maximale Zeichenlänge (def. Text)** optional eine Zahl eingeben, wenn die Preissuchmaschine eine Begrenzung der Länge des Vorschautextes beim Export vorgibt.<br/> Option **HTML-Tags entfernen** aktivieren, damit die HTML-Tags beim Export entfernt werden.<br/> Im Feld **Erlaubte HTML-Tags, kommagetrennt (def. Text)** optional die HTML-Tags eingeben, die beim Export erlaubt sind. Wenn mehrere Tags eingegeben werden, mit Komma trennen. |
| **Beschreibung**                                   | Wählen, welcher Text als Beschreibungstext übertragen werden soll.<br/> Im Feld **Maximale Zeichenlänge (def. Text)** optional eine Zahl eingeben, wenn die Preissuchmaschine eine Begrenzung der Länge der Beschreibung beim Export vorgibt.<br/> Option **HTML-Tags entfernen** aktivieren, damit die HTML-Tags beim Export entfernt werden.<br/> Im Feld **Erlaubte HTML-Tags, kommagetrennt (def. Text)** optional die HTML-Tags eingeben, die beim Export erlaubt sind. Wenn mehrere Tags eingegeben werden, mit Komma trennen. |
| **Zielland**                                       | Zielland aus der Dropdown-Liste wählen. |
| **Barcode**                                        | ASIN, ISBN oder eine EAN aus der Dropdown-Liste wählen. Der gewählte Barcode muss mit der oben gewählten Auftragsherkunft verknüpft sein. Andernfalls wird der Barcode nicht exportiert. |
| **Bild**                                           | **Position 0** oder **Erstes Bild** wählen, um dieses Bild zu exportieren.<br/> **Position 0** = Ein Bild mit der Position 0 wird übertragen.<br/> **Erstes Bild** = Das erste Bild wird übertragen. |
| **Bildposition des Energieetiketts**               | Position des Energieetikettes eintragen. Alle Bilder die als Energieetikette übertragen werden sollen, müssen diese Position haben. |
| **Bestandspuffer**                                 | Der Bestandspuffer für Varianten mit der Beschränkung auf den Netto-Warenbestand. |
| **Bestand für Varianten ohne Bestandsbeschräkung** | Der Bestand für Varianten ohne Bestandsbeschränkung. |
| **Bestand für Varianten ohne Bestandsführung**     | Der Bestand für Varianten ohne Bestandsführung. |
| **Währung live umrechnen**                         | Aktivieren, damit der Preis je nach eingestelltem Lieferland in die Währung des Lieferlandes umgerechnet wird. Der Preis muss für die entsprechende Währung freigegeben sein. |
| **Verkaufspreis**                                  | Brutto- oder Nettopreis aus der Dropdown-Liste wählen. |
| **Angebotspreis**                                  | Diese Option ist für dieses Format nicht relevant. |
| **UVP**                                            | Aktivieren, um den UVP zu übertragen. |
| **Versandkosten**                                  | Im Gegensatz zu anderen Formaten spielt hier die Auswahl einer Zahlungsart keine Rolle. Es werden alle Zahlungsarten der gewählten Konfiguration exportiert.<br/> Wenn keine Konfiguration gewählt wurde, werden alle Konfigurationen und alle Zahlungsarten exportiert.<br/> Wenn **Pauschale Versandkosten übertragen** gewählt wurde, wird nur Vorkasse als Zahlungsart übermittelt. |
| **MwSt.Hinweis**                                   | Diese Option ist für dieses Format nicht relevant. |
| **Artikelverfügbarkeit**                           | Option **überschreiben** aktivieren und in die Felder **1** bis **10**, die die ID der Verfügbarkeit darstellen, Artikelverfügbarkeiten eintragen. Somit werden die Artikelverfügbarkeiten, die im Menü **System » Artikel » Verfügbarkeit** eingestellt wurden, überschrieben. |

_Tab. 1: Einstellungen für das Exportformat IdealoDE_

### 8.2.2 Verfügbare Spalten der Exportdatei
<a name="Verfügbare Spalten der Exportdatei"></a>

_Tab. 3: Spalten der Exportdatei_

| **Spaltenbezeichnung**  | **Erläuterung** |
| :---                    | :--- |
| **article_id**          | **Pflichtfeld**<br/> Die SKU des Artikels. Bei Artikeln, die für idealo Direktkauf freigegeben wurden, wird hier eine SKU für idealo Direktkauf ausgegeben. |
| **deeplink**            | **Pflichtfeld**<br/> Der URL-Pfad des Artikels abhängig vom gewählten Mandanten in den Formateinstellungen.|
| **name**                | **Pflichtfeld**<br/> Entsprechend der Formateinstellung Artikelname.|
| **short_description**   | Entsprechend der Formateinstellung Vorschautext. |
| **description**         | **Beschränkung**: max. 1000 Zeichen<br/> Entsprechend der Formateinstellung Beschreibung. |
| **article_no**          | Die Variantennr. unter **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Einstellungen » Grundeinstellungen**. |
| **producer**            | Der Name des Herstellers des Artikels. Der Externe Name unter **Einstellungen » Artikel » Hersteller** wird bevorzugt, wenn vorhanden. |
| **model**               | Das Modell unter **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Einstellungen » Grundeinstellungen**. |
| **availability**        | **Pflichtfeld**<br/> Der Name der Artikelverfügbarkeit unter **System » Systemeinstellungen » Artikel » Verfügbarkeit** oder die Übersetzung gemäß der Formateinstellung **Artikelverfügbarkeit überschreiben**.<br/> Bei idealo muss die Lieferzeit in Tagen angegeben werden. |
| **ean**                 | Entsprechend der Formateinstellung **Barcode**. |
| **isbn**                | Entsprechend der Formateinstellung **Barcode**. |
| **fedas**               | Der Amazon-Produkttyp unter **Artikel » Artikel bearbeiten » Artikel öffnen » Multi-Channel » Amazon**. |
| **warranty**            | Aktuell nicht gepflegt. |
| **price**               | **Pflichtfeld**<br/> Der Verkaufspreis der Variante. |
| **price_old**           | Der Verkaufspreis vom Typ UVP der Variante, wenn in den Formateinstellungen aktiviert. |
| **weight**              | Gewicht brutto in Gramm unter **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Einstellungen » Maße**. |
| **category1-6**         | Der Name der Kategorieebene des Kategoriepfads der Standard-Kategorie für den in den Formateinstellungen definierten Mandanten. |
| **category_concat**     | Kategoriepfad der Standard-Kategorie für den in den Formateinstellungen definierten Mandanten. |
| **image_url_preview**   | URL zu einer für die Vorschau skalierten Version des Bildes gemäß der Formateinstellung **Bild**. |
| **image_url**           | **Pflichtfeld**<br/> URL zu dem Bild gemäß der Formateinstellung **Bild**. |
| **base_price**          | Die Grundpreisinformation im Format "Preis / Einheit". (Beispiel: 10,00 EUR / Kilogramm) |
| **free_text_field**     | Der Wert eines Merkmals vom Typ Text oder Auswahl mit der Verknüpfung zu idealo. |
| **checkoutApproved**    | Wird true gesetzt, wenn entweder die Auftragsherkunft idealo Direktkauf unter **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Verfügbarkeit » Märkte** aktiviert wurde oder ein Merkmal vom Typ Kein und der Verknüpfung zum idealo Direktkauf-Merkmal checkoutApproved gesetzt wurde. |
| **itemsInStock**        | **Voraussetzung**: checkoutApproved ist true.<br/> Der Nettowarenbestand der Variante. Bei Artikeln, die nicht auf den Nettowarenbestand beschränkt sind, wird 999 übertragen. |
| **fulfillmentType**     | **Voraussetzung**: checkoutApproved ist true.<br/> Merkmal vom Typ **Kein** und der Verknüpfung zum idealo Direktkauf-Merkmal **FulfillmentType > Spedition**, **FulfillmentType > Paketdienst**, **FulfillmentType > Brief** oder **FulfillmentType > Download**. |
| **twoManHandlingPrice** | **Voraussetzung**: checkoutApproved ist true und fulfillmentType ist Spedition.<br/> Merkmal vom Typ Text, Auswahl oder Kommazahl und der Verknüpfung zum idealo Direktkauf-Merkmal twoManHandlingPrice. |
| **disposalPrice**       | **Voraussetzung**: checkoutApproved ist true und fulfillmentType ist Spedition.<br/> Merkmal vom Typ Text, Auswahl oder Kommazahl und der Verknüpfung zum idealo Direktkauf-Merkmal disposalPrice. |
| **Zahlungsarten**       | **Pflichtfeld**: (Mindestens eine Zahlungsart)<br/> Es werden die Zahlungsarten gemäß der Formateinstellung **Versandkosten** in einer eigenen Spalte übermittelt. |


## 9 Zahlungsart **idealo Direktkauf** aktivieren
<a name="Zahlungsart idealo Direktkauf aktivieren"></a>

Damit Zahlungen für Aufträge von idealo Direktkauf durchgeführt und in deinem plentymarkets System angezeigt werden, aktiviere die Zahlungsart **idealo Direktkauf**.

<div class="alert alert-warning" role="alert">
<b>Hinweis: Zahlungsart nur für idealo Direktkauf</b><br/> Die Zahlungsart <b>idealo Direktkauf</b> muss nur aktiviert werden, wenn du idealo Direktkauf nutzt.
 </ul>
</div>

#### idealo-Zahlungsart aktivieren:

1. Öffne das Menü **Einrichtung » Aufträge » Zahlung » Zahlungsarten**.
2. Aktiviere die Einstellung **Auch inaktive zeigen**.
3. Öffne den Ordner **DE > idealo**.
4. Wähle die **idealo-Zahlungsart**.<br/>
→ Das Tab **Einstellungen** wird geöffnet.
5. Nimm die gewünschten Einstellungen vor. Beachte dazu die Erläuterungen in der folgenden Tabelle.
6. Setze ein Häkchen bei der Option **Aktiv**.
7. **Speichere** die Einstellungen.

_Tab. 4: Einstellungen für idealo-Zahlungsart_

|**Einstellung**                      |**Erläuterung** |
|:---                                 |:--- |
|**Sprache**                          |Folgende Optionen werden sprachabhängig gespeichert: **Name**, **Infoseite**, **Infoseite (Intern)**, **Logo** und **Logo hochladen**. Damit hast du die Möglichkeit, die Werte für diese Optionen in mehreren Sprachen einzugeben. Die Werte einer Sprache werden aktiviert, wenn ein Käufer im Webshop die Sprache wählt. |
|**Name**                             |Name eintragen, der im Webshop und auf Rechnungen etc. angezeigt werden soll. |
|**Infoseite**                        |Als Information zur Zahlungsart eine Kategorieseite vom Typ **Content** oder die URL einer Webseite eintragen. |
|**Infoseite (Extern)**               |Wenn unter **Infoseite** die Einstellung **Infoseite (Extern)** gewählt wurde, hier die URL der Infoseite eintragen. |
|**Lieferländer**                     |Kein Lieferland wählen.<br/> Du kannst die Zahlungsart nicht in deinem Webshop verwenden. Deshalb wird diese Zahlungsart in plentymarkets nur aktiviert, aber nicht vollständig eingerichtet. |
|**Logo**                             |Eine der folgenden Optionen für die Anzeige eines Logos wählen:<br/> **Standard-Logo anzeigen** = Das in plentymarkets für die Zahlungsart eingestellte Logo wird angezeigt.<br/> **Kein Logo anzeigen** = Das in plentymarkets für die Zahlungsart eingestellte Logo wird nicht angezeigt.<br/> **Upload-Logo anzeigen** = Blendet die Optionen **Logoansicht** und **Logo hochladen** ein. |
|**Logoansicht**                      |Wenn unter **Logo** die Option **Upload-Logo anzeigen** gewählt wurde, wird das hochgeladene Log hier angezeigt. |
|**Logo hochladen**                   |Wenn unter **Logo** die Option **Upload-Logo anzeigen** gewählt wurde, hier ein externes Logo hochladen.<br/> Auf **Dateien hochladen** klicken und das Logo wählen, das für die Zahlungsart hochgeladen werden soll. Erlaubte Datenformate: GIF, PNG und JPG. |
|**Priorität**                        |Priorität für die Anzeige der Zahlungsart im Webshop wählen. |
|**Kosten: Pauschal oder Prozentual** |Wenn bei der Zahlungsart zusätzliche Kosten berechnet werden, den Prozentwert oder Pauschalwert gemäß der Vertragskonditionen eintragen. **Wichtig:** Nicht in beide Felder einen Wert eintragen.<br/> Weitere Informationen findest du auf der Handbuchseite [Statistiken verwalten](https://knowledge.plentymarkets.com/basics/arbeiten-mit-plentymarkets/statistik/statistiken-verwalten). Ein Beispiel für pauschale und prozentuale Kosten findest du auf der Handbuchseite [Zahlungsarten verwalten](https://knowledge.plentymarkets.com/payment/zahlungsarten-verwalten#20). |

<div class="alert alert-warning" role="alert">
 <b>Zahlungsart in Kundenklassen erlauben</b><br/>
 Im Menü <b>Einrichtung » CRM » Kundenklassen</b> aktivierst oder deaktivierst du erlaubte Zahlungsarten.
 Weitere Informationen findest du im Kapitel [Zahlungsart in Kundenklasse erlauben](https://knowledge.plentymarkets.com/payment/zahlungsarten-verwalten#30).
 </ul>
</div>

Weitere Informationen findest du auf der Handbuchseite [Zahlungsarten verwalten](https://knowledge.plentymarkets.com/payment/zahlungsarten-verwalten).

<div class="alert alert-warning" role="alert">
 <b>Zahlungsart PayPal</b><br/>
 Wenn du PayPal als Zahlungsart anbietest, muss die Zahlungsart PayPal zwingend in deinem plentymarkets System hinterlegt und eingerichtet sein, damit die Zahlung korrekt importiert und dem Auftrag zugeordnet werden kann.
 </ul>
</div>


## 10 Merkmale erstellen
<a name="Merkmale erstellen"></a>
                                       
Mit [Merkmalen](https://knowledge.plentymarkets.com/artikel/einstellungen/eigenschaften#100) verknüpfst du bestimmte Eigenschaften, die du für die Einrichtung des Marktplatzes idealo Direktkauf benötigst, mit deinen Artikeln. Mit Merkmalen überträgst du Artikeleigenschaften, Versandarten und Gebühren an idealo Direktkauf.

→ **Hinweis: Bestimmte Merkmale können nur mit Plugin-Version 2.0 verwendet werden**<br/>
Die Merkmale **DeliveryComment**, **DepositFee**, **DisposalPrice**, **EnergyClass**, **FreeReturnDays**, **Gender**, **Material** und **Replica** können nur verwendet werden, wenn die Plugin-Version 2.0 in deinem plentymarkets System installiert ist. Außerdem können diese Merkmale nur in Verbindung mit dem automatischen Artikelexport zu idealo Direktkauf übertragen werden. Den automatischen Artikelexport aktivierst du im idealo-Assistenten im Schritt **Automatische Datenübertragung**.<br/>
Wenn du den automatischen Artikelexport im idealo-Assistenten aktiviert hast, kannst du alle idealo-Merkmale übertragen.<br/>
Wenn du deine Artikel per CSV-Datei mit dem elastischen Export überträgst, kannst du nur das Merkmal **FulfillmentType** verwenden.

### 10.1 Merkmal für Material und Zielgruppe/Geschlecht erstellen

Mit den Merkmalen Material und Gender überträgst du Informationen zu Material und Zielgruppe bzw. Geschlecht an idealo Direktkauf.

Im Folgenden wird beschrieben, wie du das Merkmal **Material** erstellst. Erstelle das Merkmal **Gender** auf die gleiche Weise, wähle jedoch den Merkmaltyp **Text**.

#### Merkmal für Material einrichten:

1. Öffne das Menü **Einrichtung » Artikel » Merkmale » Tab: Neues Merkmal**.
2. Gib den **Namen (intern)** ein.
3. Wähle als Merkmaltyp **kein** aus der Dropdown-Liste.
4. Wähle bei **idealo Direktkauf-Merkmal** das Merkmal **Material**.
5. **Speichere** die Einstellungen.

Im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Tab: Merkmale** verknüpfst du anschließend das Merkmal mit dem Artikel.

### 10.2 Merkmal für Versandarten erstellen

Wenn du idealo Direktkauf nutzt, findet der Verkauf direkt bei idealo statt und du musst Informationen zur Versandart an idealo Direktkauf übergeben. Versendest du deine Artikel mit einem Paketdienst, einer Spedition, per Brief oder Download, wird diese Pflichtinformation mit einem Merkmal angegeben und an idealo Direktkauf übergeben. Bei der Versandart **Spedition** wird beim Verkauf des Artikels die Telefonnummer des Käufers zur Abstimmung eines Liefertermins mit dem beauftragten Speditionsunternehmen erfragt.

Gehe wie im Folgenden beschrieben vor, um das Merkmal **FulfillmentType** anzulegen, mit dem du angibst, ob du die Versandart **Spedition**, **Paketdienst**, **Brief** oder **Download** verwendest.

#### Merkmal für Versandart erstellen:

1. Öffne das Menü **Einrichtung » Artikel » Merkmale » Tab: Neues Merkmal**.
2. Gib den **Namen (intern)** ein.
3. Wähle als Merkmaltyp **kein** aus der Dropdown-Liste.
4. Wähle bei **idealo Direktkauf-Merkmal** das Merkmal **FulfillmentType**.<br/>
→ Eine Dropdown-Liste erscheint.
5. Wähle je nach Versandart einen Wert aus der Dropdown-Liste. Die Werte **Spedition**, **Paketdienst**, **Brief** und **Download** sind verfügbar.
6. **Speichere** die Einstellungen.

Im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Tab: Merkmale** verknüpfst du anschließend das Merkmal mit dem Artikel.

#### Weitere Merkmale für Versandarten

Für Artikel mit der Versandart **Spedition** kann die zusätzliche Dienstleistung **Zwei-Mann-Lieferung bis zum Aufstellort** und **Altgeräteabholung** als Merkmal an idealo Direktkauf übergeben werden. Die Altgeräteabholung kann nur in Kombination mit der Zwei-Mann-Lieferung übergeben werden. Das heißt, du musst sowohl das Merkmal **Zwei-Mann-Lieferung (twoManHandlingPrice)** als auch das Merkmal **Altgeräteabholung (DisposalPrice)** anlegen und beide mit dem Artikel verknüpfen. Wähle in beiden Fällen als Merkmaltyp **Kommazahl**. Gib den Aufpreis am Artikel für die zusätzliche Dienstleistung mit zwei Dezimalstellen und mit Punkt als Dezimaltrenner (19.99) im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Tab: Merkmale** ein.

### 10.3 Merkmal für Kommentar zur Lieferung erstellen

Mit dem Merkmal **DeliveryComment** werden weitere Informationen zur Lieferung übermittelt.

Gehe wie im Folgenden beschrieben vor, um das Merkmal **DeliveryComment** zu erstellen.

#### Merkmal für Kommentar zur Lieferung erstellen:

1. Öffne das Menü **Einrichtung » Artikel » Merkmale » Tab: Neues Merkmal**.
2. Gib den **Namen (intern)** ein.
3. Wähle als Merkmaltyp **Text** aus der Dropdown-Liste.
4. Wähle bei **idealo Direktkauf-Merkmal** das Merkmal **DeliveryComment**.
5. **Speichere** die Einstellungen.

Im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Tab: Merkmale** verknüpfst du anschließend das Merkmal mit dem Artikel.

### 10.4 Merkmal für Energieeffizienzklasse erstellen

Mit dem Merkmal **EnergyClass** überträgst du Informationen zur Energieeffizienzklasse an idealo Direktkauf.

Gehe wie im Folgenden beschrieben vor, um das Merkmal **EnergyClass** zu erstellen.

#### Merkmal für Energieeffizienzklasse einrichten:

1. Öffne das Menü **Einrichtung » Artikel » Merkmale » Tab: Neues Merkmal**.
2. Gib den **Namen (intern)** ein.
3. Wähle als Merkmaltyp **kein** aus der Dropdown-Liste.
4. Wähle bei **idealo Direktkauf-Merkmal** das Merkmal **EnergyClass**.<br/>
→ Eine Dropdown-Liste erscheint.
5. Wähle je nach Energieeffizienzklasse einen Wert aus der Dropdown-Liste.
6. **Speichere** die Einstellungen.

Im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Tab: Merkmale** verknüpfst du anschließend das Merkmal mit dem Artikel.

### 10.5 Merkmal für kostenlose Rückgabe erstellen

Mit dem Merkmal **FreeReturnDays** überträgst du Informationen zur kostenlosen Rückgabefrist, d.h. die Frist, innerhalb der ein Artikel kostenlos zurückgegeben werden kann, an idealo Direktkauf.

Gehe wie im Folgenden beschrieben vor, um das Merkmal **FreeReturnDays** zu erstellen.

#### Merkmal für kostenlose Rückgabefrist einrichten:

1. Öffne das Menü **Einrichtung » Artikel » Merkmale » Tab: Neues Merkmal**.
2. Gib den **Namen (intern)** ein.
3. Wähle als Merkmaltyp **ganze Zahl** aus der Dropdown-Liste.
4. Wähle bei **idealo Direktkauf-Merkmal** das Merkmal **FreeReturnDays**.
5. **Speichere** die Einstellungen.

Im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Tab: Merkmale** verknüpfst anschließend das Merkmal mit dem Artikel.

### 10.6 Merkmal für Pfand erstellen

Mit dem Merkmal **DepositFee** überträgst du Informationen zum Pfand an idealo Direktkauf. Dieses Merkmal wird benötigt, wenn für einen Artikel Pfand gezahlt werden muss.

Gehe wie im Folgenden beschrieben vor, um das Merkmal **DepositFee** zu erstellen.

#### Merkmal für Pfand einrichten:

1. Öffne das Menü **Einrichtung » Artikel » Merkmale » Tab: Neues Merkmal**.
2. Gib den **Namen (intern)** ein.
3. Wähle als Merkmaltyp **Kommazahl** aus der Dropdown-Liste.
4. Wähle bei **idealo Direktkauf-Merkmal** das Merkmal **DepositFee**.
5. **Speichere** die Einstellungen.

Im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Tab: Merkmale** verknüpfst du anschließend das Merkmal mit dem Artikel.

### 10.7 Merkmal für Replika erstellen

Mit dem Merkmal **Replica** gibst du an, ob es sich bei dem Artikel um eine Replika handelt.

Gehe wie im Folgenden beschrieben vor, um das Merkmal **Replica** zu erstellen.

#### Merkmal für Replika einrichten:

1. Öffne das Menü **Einrichtung » Artikel » Merkmale » Tab: Neues Merkmal**.
2. Gib den **Namen (intern)** ein.
3. Wähle als Merkmaltyp **kein** aus der Dropdown-Liste.
4. Wähle bei **idealo Direktkauf-Merkmal** das Merkmal **Replica**.
5. **Speichere** die Einstellungen.

Im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Variante öffnen » Tab: Merkmale** verknüpfst du anschließend das Merkmal mit dem Artikel.


## 11 Ereignisaktionen einrichten
<a name="Ereignisaktionen einrichten"></a>

Richte Ereignisaktionen ein, um Änderungen am Auftragsstatus automatisch an idealo zu senden. Du kannst mit Ereignisaktionen Auftragsbestätigungen, Versandbestätigungen, Retouren und Stornierungen automatisch an idealo Direktkauf senden.

<div class="alert alert-warning" role="alert">
 <b>Hinweis: Ereignisaktionen für idealo Direktkauf</b><br/>
 Ereignisaktionen müssen nur eingerichtet werden, wenn du idealo Direktkauf nutzt.
 </ul>
</div>

### 11.1 Auftragsbestätigungen automatisch senden

Richte eine [Ereignisaktion](https://knowledge.plentymarkets.com/automatisierung/ereignisaktionen) ein, um nach Eingang eines Auftrags automatisch eine Auftragsbestätigung an idealo zu senden.

#### Ereignisaktion einrichten:

1. Öffne das Menü **Einrichtung » Aufträge » Ereignisse**.
2. Klicke auf **Ereignisaktion hinzufügen**.<br/>
→ Das Fenster **Neue Ereignisaktion erstellen** wird geöffnet.
3. Gib einen Namen ein.
4. Wähle das Ereignis gemäß Tabelle 3.
5. **Speichere** die Einstellungen.<br/>
→ Das Ereignis wird erstellt.
6. Nimm die weiteren Einstellungen gemäß Tabelle 3 vor.
7. Setze ein Häkchen bei **Aktiv**.
8. **Speichere** die Einstellungen.<br/>
→ Die Ereignisaktion wird gespeichert.

_Tab. 5: Ereignisaktion zum automatischen Senden von Auftragsbestätigungen an idealo_

|**Einstellung** |**Option**                                         |**Auswahl** |
|:---            |:---                                               |:--- |
|Ereignis        |**Auftragsanlage: Neuer Auftrag**                  | |
|Filter 1        |**Auftrag > Auftragstyp**                          |**Auftrag** |
|Filter 2        |**Auftrag > Herkunft**                             |**idealo Direktkauf** |
|Aktion          |**Auftrag > Auftragsbestätigung an idealo senden** | |

### 11.2 Versandbestätigungen automatisch senden

Richte eine [Ereignisaktion](https://knowledge.plentymarkets.com/automatisierung/ereignisaktionen) ein, um automatisch eine Versandbestätigung an idealo zu senden, nachdem ein Warenausgang gebucht wurde.

#### Ereignisaktion einrichten:

1. Öffne das Menü **Einrichtung » Aufträge » Ereignisse**.
2. Klicke auf **Ereignisaktion hinzufügen**.<br/>
→ Das Fenster **Neue Ereignisaktion erstellen** wird geöffnet.
3. Gib einen Namen ein.
4. Wähle das Ereignis gemäß Tabelle 4.
5. **Speichere** die Einstellungen.<br/>
→ Das Ereignis wird erstellt.
6. Nimm die weiteren Einstellungen gemäß Tabelle 4 vor.
7. Setze ein Häkchen bei **Aktiv**.
8. **Speichere** die Einstellungen.<br/>
→ Die Ereignisaktion wird gespeichert.

_Tab. 5: Ereignisaktion zum automatischen Senden von Versandbestätigungen an idealo_

|**Einstellung** |**Option**                                        |**Auswahl** |
|:---            |:---                                              |:--- |
|Ereignis        |**Auftragsänderung: Warenausgang gebucht**        | |
|Filter 1        |**Auftrag > Auftragstyp**                         |**Auftrag** |
|Filter 2        |**Auftrag > Herkunft**                            |**idealo Direktkauf** |
|Aktion          |**Versand > Versandbestätigung an idealo senden** | |

### 11.3 Retouren automatisch senden

Richte eine [Ereignisaktion](https://knowledge.plentymarkets.com/automatisierung/ereignisaktionen) ein, um idealo automatisch über Retouren zu informieren.

#### Ereignisaktion einrichten:

1. Öffne das Menü **Einrichtung » Aufträge » Ereignisse**.
2. Klicke auf **Ereignisaktion hinzufügen**.<br/>
→ Das Fenster **Neue Ereignisaktion erstellen** wird geöffnet.
3. Gib einen Namen ein.
4. Wähle das Ereignis gemäß Tabelle 5.
5. **Speichere** die Einstellungen.<br/>
→ Das Ereignis wird erstellt.
6. Nimm die weiteren Einstellungen gemäß Tabelle 5 vor.
7. Setze ein Häkchen bei **Aktiv**.
8. **Speichere** die Einstellungen.<br/>
→ Die Ereignisaktion wird gespeichert.

_Tab. 6: Ereignisaktion zum automatischen Senden von Retouren an idealo_

|**Einstellung** |**Option**                             |**Auswahl** |
|:---            |:---                                   |:--- |
|Ereignis        |**Auftragsanlage: Neue Retoure**       | |
|Filter 1        |**Auftrag > Auftragstyp**              |**Retoure** |
|Filter 2        |**Auftrag > Herkunft**                 |**idealo Direktkauf** |
|Aktion          |**Retoure > Retoure an idealo senden** | |

### 11.4 Stornierungen automatisch senden

Richte eine [Ereignisaktion](https://knowledge.plentymarkets.com/automatisierung/ereignisaktionen) ein, um idealo automatisch über Stornierungen zu informieren.

#### Ereignisaktion einrichten:

1. Öffne das Menü **Einrichtung » Aufträge » Ereignisse**.
2. Klicke auf **Ereignisaktion hinzufügen**.<br/>
→ Das Fenster **Neue Ereignisaktion erstellen** wird geöffnet.
3. Gib einen Namen ein.
4. Wähle das Ereignis gemäß Tabelle 6.
5. **Speichere** die Einstellungen.<br/>
→ Das Ereignis wird erstellt.
6. Nimm die weiteren Einstellungen gemäß Tabelle 6 vor.
7. Wähle einen Grund für die Stornierung.
8. Setze ein Häkchen bei **Aktiv**.
9. **Speichere** die Einstellungen.<br/>
→ Die Ereignisaktion wird gespeichert.

_Tab. 7: Ereignisaktion zum automatischen Senden von Stornierungen an idealo_

|**Einstellung** |**Option**                                |**Auswahl** |
|:---            |:---                                      |:--- |
|Ereignis        |**Statuswechsel: [8] Storniert**          | |
|Filter 1        |**Auftrag > Auftragstyp**                 |**Auftrag** |
|Filter 2        |**Auftrag > Herkunft**                    |**idealo Direktkauf** |
|Aktion          |**Auftrag: Stornierung an idealo senden** | |


## 12 API-Log abrufen

Im Menü **Daten » API-Log** findest du eine Historie über Vorgänge, die über die idealo-Schnittstelle ausgeführt wurden. Das Format idealoDirektkauf steht dir für idealo zur Verfügung.

#### API-Log abrufen:

1. Öffne das Menü **Daten » API-Log » Tab: API-Log**.
2. Wähle das Format **idealoDirektkauf** aus der Dropdown-Liste **Vorgang**.
3. Wähle ggf. ein Datum, um nur Einträge eines bestimmten Tages zu erhalten.
4. Wähle die Anzahl der Ergebnisse pro Seite.
5. Klicke auf **Suchen**, um die Ergebnisse anzuzeigen.


## 13 Lizenz

Das gesamte Projekt unterliegt der GNU AFFERO GENERAL PUBLIC LICENSE – weitere Informationen findest du in der [LICENSE.md](https://github.com/plentymarkets/plugin-elastic-export-idealo-de/blob/master/LICENSE.md).
