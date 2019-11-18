
# User Guide für das idealo 2.0 Plugin

<div class="container-toc"></div>


## 1 Über idealo

Im Jahr 2000 mit der Mission gestartet, Nutzern zu helfen, richtige Kaufentscheidungen zu treffen, zählt idealo mit 50.000 Händlern und rund 18 Millionen Nutzern pro Monat zu den relevantesten deutschen E-Commerce-Websites.<br/>

Mit idealo Direktkauf bietet idealo einen starken Vertriebskanal. Der "Zum Kauf"-Button ermöglicht es Nutzern, das Produkt direkt über eine vollintegrierte Checkout-Funktion über idealo zu bestellen. Vertragspartner sind dabei stets die Händler selbst, die auch wie gewohnt das Fulfillment übernehmen.<br/>

Weitere Informationen zu idealo findest du auf der Handbuchseite [idealo Direktkauf einrichten](https://knowledge.plentymarkets.com/maerkte/idealo/idealo-einrichten).<br/>


## 2 Bei idealo registrieren

Um das Plugin für idealo einzurichten, registriere dich zunächst als Händler.

→ **Hinweis:** Kläre vor der Einrichtung in plentymarkets mit idealo, wie Artikeldaten übertragen werden sollen (Erstellung, Aktualisierung und Löschen von Artikeln auf idealo). Artikeldaten können mit einer CSV-Datei oder über eine PWS 2.0-Schnittstelle exportiert werden.<br/>
Wenn du PWS 2.0 für den Artikelexport nutzt, werden Artikel einmal täglich auf idealo erstellt und gelöscht. Preise und Bestände werden alle 15 Minuten aktualisiert.<br/>
Wenn du Artikel mit einer CSV-Datei über den elastischen Export zu idealo überträgst, können Artikel über die URL von idealo abgerufen werden.


## 3 Assistent durchlaufen

Durchlaufe zunächst den **idealo-Assistenten**, um die Grundeinstellungen für idealo in plentymarkets vorzunehmen. Mit dem **idealo-Assistenten** richtest du dein idealo-Konto in plentymarkets ein und nimmst Einstellungen für den Artikeldatenxport zu idealo und Auftragsimport von idealo Direktkauf vor.<br/>

Den **idealo-Assistenten** findest du im Menü **System » Assistenten** im **Omni-Channel**-Ordner. Klicke auf den Assistenten, um den Assistenten zu starten.

→ **Hinweis:** Es ist zwingend erforderlich, den **idealo-Assistenten** zu durchlaufen, wenn du deine Artikel über PWS 2.0 exportierst, da der automatische Artikelexport nur im idealo-Assistenten eingestellt werden kann.


## 4 Auftragsherkunft aktivieren

Damit du Artikel, Merkmale etc. mit dem idealo Preisvergleich verknüpfen kannst, muss im Menü **System » Systemeinstellungen » Aufträge » Auftragsherkunft** die Auftragsherkunft **idealo** aktiviert werden.

#### Auftragsherkunft für idealo Preisvergleich aktivieren:

1. Öffne das Menü **System » Systemeinstellungen » Aufträge » Auftragsherkunft**.
2. Setze ein Häkchen bei **idealo**.
3. **Speichere** die Einstellungen.

Wenn du idealo Direktkauf nutzen möchtest, aktiviere zusätzlich die Auftragsherkunft **idealo Direktkauf**.


## 5 Artikelverfügbarkeit einstellen

Artikel, die du auf idealo verkaufen möchtest, müssen im Menü **Artikel » Artikel bearbeiten » Artikel öffnen » Tab: Varianten-ID** im Tab **Verfügbarkeit** aktiviert werden. Stelle die Artikelverfügbarkeit für idealo ein wie im Folgenden beschrieben.

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

Gehe wie im Folgenden beschrieben vor, um für die Auftragsherkunft idealo einen Verkaufspreis festzulegen. Dieser Preis wird auf idealo angezeigt und ist für den idealo Preisvergleich und idealo Direktkauf gültig.

#### Verkaufspreis für idealo festlegen:

1. Öffne das Menü **System » Systemeinstellungen » Artikel » Verkaufspreise » Verkaufspreis öffnen » Tab: Einstellungen**.<br/>
→ Wenn du noch keinen Verkaufspreis angelegt hast, klicke auf **Neu**, um einen Verkaufspreis zu erstellen.
2. Setze ein Häkchen bei der Herkunft **idealo**.
3. **Speichere** die Einstellungen.

→ **Hinweis:** Wenn du für idealo einen Mindestpreis angeben möchtest, musst du mindestens zwei Verkaufspreise für idealo festlegen, einen Mindestpreis und einen normalen Verkaufspreis. Außerdem muss der Mindestpreis vom Typ **Aktionspreis** sein und mit der Herkunft **idealo Direktkauf** verknüpft werden.<br/>
Welcher Preis als Mindestpreis an idealo übertragen werden soll, legst du im idealo-Assistenten im Schritt **Artikeldaten** mit der Einstellung **Welcher Preis soll als Mindestpreis an idealo übertragen werden?** fest.


## 7 SKU manuell festlegen

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


## 8 Artikelexport einrichten

Artikel werden entweder mit dem automatischen Artikelexport über eine PWS 2.0-Schnittstelle oder mit einer CSV-Datei über den elastischen Export zu idealo übertragen.<br/>

→ **Hinweis:** Kläre vor der Einrichtung in plentymarkets mit idealo, wie Artikeldaten übertragen werden sollen (Erstellung, Aktualisierung und Löschen von Artikeln auf idealo). Artikeldaten können mit einer CSV-Datei oder über eine PWS 2.0-Schnittstelle exportiert werden.<br/>
Wenn du PWS 2.0 für den Artikelexport nutzt, werden Artikel einmal täglich auf idealo erstellt und gelöscht. Preise und Bestände werden alle 15 Minuten aktualisiert.<br/>
Wenn du Artikel mit einer CSV-Datei über den elastischen Export zu idealo überträgst, können Artikel über die URL von idealo abgerufen werden.
 
Wenn du PWS 2.0 zur automatischen Artikelübertragung verwendest, aktiviere den automatischen Artikelexport im **idealo-Assistenten**. Für den automatischen Artikelexport sind außerhalb des idealo-Assistenten keine weiteren Einstellungen nötig.<br/>

Wenn du Artikel über den elastischen Export mit dem IdealoDE-Plugin zu idealo exportierst, müssen im Menü **Daten » Elastischer Export** weitere Einstellungen vorgenommen werden. Als Voraussetzung muss neben dem **ElasticExportIdealoDE**-Plugin auch das Plugin [Elastischer Export](https://marketplace.plentymarkets.com/plugins/channels/marktplaetze/elasticexport_4763) in deinem plentymarkets System installiert sein. Lege zunächst das Datenformat IdealoDE an und übermittele im Anschluss die URL zu idealo.

### 8.1 Das Format IdealoDE-Plugin in plentymarkets einrichten

→ **Hinweis:** Die in diesem Kapitel beschriebenen Einstellungen sind nur notwendig, wenn du Artikel über den elastischen Export zu idealo überträgst.

→ **Hinweis**: **idealo Produkt-CSV prüfen**<br/> Zurzeit sind in plentymarkets nicht alle Spalten der idealo Produkt-CSV verfügbar. Prüfe vor der Einrichtung, ob du Produktspalten benötigst, die in plentymarkets noch nicht verfügbar sind. In diesem Fall ist die Einrichtung von idealo zurzeit noch nicht möglich.<br/> Eine Übersicht der in plentymarkets verfügbaren Spalten erhältst du im Kapitel **Verfügbare Spalten der Exportdatei**.

Mit der Installation dieses Plugins erhältst du das Exportformat **IdealoDE-Plugin**, mit dem du Daten über den elastischen Export zu idealo überträgst. Um dieses Format für den elastischen Export nutzen zu können, installiere zunächst das Plugin **Elastic Export** aus dem plentyMarketplace, wenn noch nicht geschehen. 

Sobald beide Plugins in deinem System installiert sind, kann das Exportformat **IdealoDE-Plugin** erstellt werden. Weitere Informationen findest du auf der Handbuchseite [Elastischer Export](https://knowledge.plentymarkets.com/daten/daten-exportieren/elastischer-export).

Neues Exportformat erstellen:

1. Öffne das Menü **Daten » Elastischer Export**.
2. Klicke auf **Neuer Export**.
3. Nimm die Einstellungen vor. Beachte dazu die Erläuterungen in Tabelle 1.
4. **Speichere** die Einstellungen.
→ Eine ID für das Exportformat **IdealoDE-Plugin** wird vergeben und das Exportformat erscheint in der Übersicht **Exporte**.

In der folgenden Tabelle findest du Hinweise zu den einzelnen Formateinstellungen und empfohlenen Artikelfiltern für das Format **IdealoDE-Plugin**.

| **Einstellung**                                    | **Erläuterung** |
| :---                                               | :--- |
| **Einstellungen**                                  | |
| **Name**                                           | Name eingeben. Unter diesem Namen erscheint das Exportformat in der Übersicht im Tab **Exporte**. |
| **Typ**                                            | Typ **Artikel** aus der Dropdown-Liste wählen. |
| **Format**                                         | **IdealoDE-Plugin** wählen. |
| **Limit**                                          | Zahl eingeben. Wenn mehr als 9999 Datensätze an die Preissuchmaschine übertragen werden sollen, wird die Ausgabedatei wird für 24 Stunden nicht noch einmal neu generiert, um Ressourcen zu sparen. Wenn mehr mehr als 9999 Datensätze benötigt werden, muss die Option **Cache-Datei generieren** aktiv sein. |
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

### 8.2 Verfügbare Spalten der Exportdatei

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
| **fulfillmentType**     | **Voraussetzung**: checkoutApproved ist true.<br/> Merkmal vom Typ Kein und der Verknüpfung zum idealo Direktkauf-Merkmal **FulfillmentType > Spedition**, **FulfillmentType > Paketdienst** oder **FulfillmentType > Download**. |
| **twoManHandlingPrice** | **Voraussetzung**: checkoutApproved ist true und fulfillmentType ist Spedition.<br/> Merkmal vom Typ Text, Auswahl oder Kommazahl und der Verknüpfung zum idealo Direktkauf-Merkmal twoManHandlingPrice. |
| **disposalPrice**       | **Voraussetzung**: checkoutApproved ist true und fulfillmentType ist Spedition.<br/> Merkmal vom Typ Text, Auswahl oder Kommazahl und der Verknüpfung zum idealo Direktkauf-Merkmal disposalPrice. |
| **Zahlungsarten**       | **Pflichtfeld**: (Mindestens eine Zahlungsart)<br/> Es werden die Zahlungsarten gemäß der Formateinstellung **Versandkosten** in einer eigenen Spalte übermittelt. |

_Tab. 2: Spalten der Exportdatei_


## 9 Merkmale erstellen

Mit [Merkmalen](https://knowledge.plentymarkets.com/artikel/artikel-verwalten#480) verknüpfst du bestimmte Eigenschaften, die du für die Einrichtung des Marktplatzes idealo Direktkauf benötigst, mit deinen Artikeln. Mit Merkmalen überträgst du Artikeleigenschaften, Versandarten und Gebühren an idealo Direktkauf.

→ **Hinweis: Bestimmte Merkmale können nur mit Plugin-Version 2.0 verwendet werden**<br/>
Die Merkmale **DeliveryComment**, **DepositFee**, **DisposalPrice**, **EnergyClass**, **FreeReturnDays**, **Gender**, **Material** und **Replica** können nur verwendet werden, wenn die Plugin-Version 2.0 in deinem plentymarkets System installiert ist. Außerdem können diese Merkmale nur in Verbindung mit dem automatischen Artikelexport zu idealo Direktkauf übertragen werden. Den automatischen Artikelexport aktivierst du im **idealo-Assistenten** im Schritt **Automatische Datenübertragung**.<br/>
Wenn du den automatischen Artikelexport im idealo-Assistenten aktiviert hast, kannst du alle idealo-Merkmale übertragen.<br/>
Wenn du deine Artikel per CSV-Datei mit dem elastischen Export überträgst, kannst du nur das Merkmal **FulfillmentType** verwenden.

Wie du Merkmale für idealo Direktkauf erstellst und verknüpfst, ist im Kapitel [idealo Direktkauf: Merkmale erstellen](https://knowledge.plentymarkets.com/maerkte/idealo/idealo-einrichten#660) auf der Handbuchseite [idealo einrichten](https://knowledge.plentymarkets.com/maerkte/idealo/idealo-einrichten) beschrieben.


## 10 Lizenz

Das gesamte Projekt unterliegt der GNU AFFERO GENERAL PUBLIC LICENSE – weitere Informationen findest du in der [LICENSE.md](https://github.com/plentymarkets/plugin-elastic-export-idealo-de/blob/master/LICENSE.md).
