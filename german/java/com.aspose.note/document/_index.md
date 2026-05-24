---
title: "Document"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt ein Aspose.Note-Dokument dar."
type: docs
weight: 20
url: /de/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Stellt ein Aspose.Note-Dokument dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Document()](#Document--) | Initialisiert eine neue Instanz der `Document`-Klasse. |
| [Document(String filePath)](#Document-java.lang.String-) | Initialisiert eine neue Instanz der `Document`-Klasse. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Initialisiert eine neue Instanz der `Document`-Klasse. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Initialisiert eine neue Instanz der `Document`-Klasse. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Initialisiert eine neue Instanz der `Document`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Erkennt alle Änderungen am Dokumentlayout seit dem vorherigen Aufruf von `DetectLayoutChanges`. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Liest einen Wert, der angibt, ob Aspose.Note die Erkennung von Layoutänderungen automatisch durchführt. |
| [getColor()](#getColor--) | Liest die Farbe. |
| [getCreationTime()](#getCreationTime--) | Liest die Erstellungszeit. |
| [getDisplayName()](#getDisplayName--) | Liest den Anzeigenamen. |
| [getFileFormat()](#getFileFormat--) | Liefert das Dateiformat (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Liefert die global eindeutige ID des Objekts. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Liefert die `PageHistory`, die die vollständige Historie für jede im Dokument dargestellte Seite enthält (die früheste bei Index 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. |
| [print()](#print--) | Druckt das Dokument mit dem Standarddrucker. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Druckt das Dokument mit dem Standarddrucker. |
| [print(String printerName)](#print-java.lang.String-) | Druckt das Dokument mit dem Standarddrucker. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Druckt das Dokument mit dem Standarddrucker. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Speichert das OneNote‑Dokument in einen Stream. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Speichert das OneNote‑Dokument in einen Stream unter Verwendung der angegebenen Speicheroptionen. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Speichert das OneNote‑Dokument in einen Stream im angegebenen Format. |
| [save(String fileName)](#save-java.lang.String-) | Speichert das OneNote‑Dokument in einer Datei. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Speichert das OneNote‑Dokument in einer Datei unter Verwendung der angegebenen Speicheroptionen. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Speichert das OneNote‑Dokument in einer Datei im angegebenen Format. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Setzt einen Wert, der angibt, ob Aspose.Note die Erkennung von Layoutänderungen automatisch durchführt. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Setzt die Farbe. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Setzt die Erstellungszeit. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Setzt den Anzeigenamen. |
### Document() {#Document--}
```
public Document()
```


Initialisiert eine neue Instanz der `Document`-Klasse. Erstellt ein leeres OneNote-Dokument.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Initialisiert eine neue Instanz der `Document`-Klasse. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der `Document`-Klasse. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei. Ermöglicht die Angabe zusätzlicher Optionen wie ein Verschlüsselungspasswort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Optionen zum Laden eines Dokuments. Kann null sein. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Initialisiert eine neue Instanz der `Document`-Klasse. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inStream | java.io.InputStream | Der Stream. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der `Document`-Klasse. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream. Ermöglicht die Angabe zusätzlicher Optionen wie ein Verschlüsselungspasswort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inStream | java.io.InputStream | Der Stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Optionen zum Laden eines Dokuments. Kann null sein. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer Klasse, die von `DocumentVisitor` abgeleitet ist. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Erkennt alle Änderungen am Dokumentlayout seit dem vorherigen Aufruf von `DetectLayoutChanges`. Falls `AutomaticLayoutChangesDetectionEnabled` auf true gesetzt ist, wird es automatisch zu Beginn des Dokumentexports verwendet.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Liefert einen Wert, der angibt, ob Aspose.Note die Erkennung von Layoutänderungen automatisch durchführt. Standardwert ist `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Liest die Farbe.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Liest die Erstellungszeit.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Liest den Anzeigenamen.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Liefert das Dateiformat (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Liefert die global eindeutige ID des Objekts.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


Liefert die `PageHistory`, die die vollständige Historie für jede im Dokument dargestellte Seite enthält (die früheste bei Index 0). Auf die aktuelle Seitenrevision kann über `PageHistory.current` zugegriffen werden und sie ist separat von der Sammlung historischer Versionen enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Die aktuelle Revision einer Seite. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu prüfen, muss das Dokument vollständig geladen werden. Daher kann diese Methode zu Leistungseinbußen führen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.InputStream | Der Stream. |
| document | [Document\[\]](../../com.aspose.note/document) | Das geladene Dokument. |

**Returns:**
boolean - Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu prüfen, muss das Dokument vollständig geladen werden. Daher kann diese Methode zu Leistungseinbußen führen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.InputStream | Der Stream. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Die Ladeoptionen. |
| document | [Document\[\]](../../com.aspose.note/document) | Das geladene Dokument. |

**Returns:**
boolean - Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu prüfen, muss das Dokument vollständig geladen werden. Daher kann diese Methode zu Leistungseinbußen führen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.InputStream | Der Stream. |
| password | java.lang.String | Das Passwort zum Entschlüsseln eines Dokuments. |
| document | [Document\[\]](../../com.aspose.note/document) | Das geladene Dokument. |

**Returns:**
boolean - Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu prüfen, muss das Dokument vollständig geladen werden. Daher kann diese Methode zu Leistungseinbußen führen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |
| document | [Document\[\]](../../com.aspose.note/document) | Das geladene Dokument. |

**Returns:**
boolean - Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu prüfen, muss das Dokument vollständig geladen werden. Daher kann diese Methode zu Leistungseinbußen führen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Die Ladeoptionen. |
| document | [Document\[\]](../../com.aspose.note/document) | Das geladene Dokument. |

**Returns:**
boolean - Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu prüfen, muss das Dokument vollständig geladen werden. Daher kann diese Methode zu Leistungseinbußen führen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |
| password | java.lang.String | Das Passwort zum Entschlüsseln eines Dokuments. |
| document | [Document\[\]](../../com.aspose.note/document) | Das geladene Dokument. |

**Returns:**
boolean - Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.
### print() {#print--}
```
public void print()
```


Druckt das Dokument mit dem Standarddrucker.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Druckt das Dokument mit dem Standarddrucker.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Optionen zum Drucken eines Dokuments. Kann null sein. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Druckt das Dokument mit dem Standarddrucker.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Druckt das Dokument mit dem Standarddrucker.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Speichert das OneNote‑Dokument in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.OutputStream | Der System.iO.stream, in dem das Dokument gespeichert wird. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Speichert das OneNote‑Dokument in einen Stream unter Verwendung der angegebenen Speicheroptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.OutputStream | Der System.iO.stream, in dem das Dokument gespeichert wird. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Gibt die Optionen an, wie das Dokument im Stream gespeichert wird. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Speichert das OneNote‑Dokument in einen Stream im angegebenen Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.OutputStream | Der System.iO.stream, in dem das Dokument gespeichert wird. |
| format | int | Das Format, in dem das Dokument gespeichert werden soll. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Speichert das OneNote‑Dokument in einer Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der vollständige Name für die Datei. Wenn bereits eine Datei mit dem angegebenen vollständigen Namen existiert, wird die vorhandene Datei überschrieben. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Speichert das OneNote‑Dokument in einer Datei unter Verwendung der angegebenen Speicheroptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der vollständige Name für die Datei. Wenn bereits eine Datei mit dem angegebenen vollständigen Namen existiert, wird die vorhandene Datei überschrieben. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Gibt die Optionen an, wie das Dokument in einer Datei gespeichert wird. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Speichert das OneNote‑Dokument in einer Datei im angegebenen Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der vollständige Name für die Datei. Wenn bereits eine Datei mit dem angegebenen vollständigen Namen existiert, wird die vorhandene Datei überschrieben. |
| format | int | Das Format, in dem das Dokument gespeichert werden soll. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Setzt einen Wert, der angibt, ob Aspose.Note die Erkennung von Layoutänderungen automatisch durchführt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Neuer Wert. Kann null sein. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Setzt die Farbe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color | Farbwert. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Setzt die Erstellungszeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | DateTime-Wert. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Setzt den Anzeigenamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | DateTime-Wert. |

