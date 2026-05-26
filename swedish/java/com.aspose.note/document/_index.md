---
title: "Document"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar ett Aspose.Note-dokument."
type: docs
weight: 20
url: /sv/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Representerar ett Aspose.Note-dokument.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Document()](#Document--) | Initierar en ny instans av klassen `Document`. |
| [Document(String filePath)](#Document-java.lang.String-) | Initierar en ny instans av klassen `Document`. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Initierar en ny instans av klassen `Document`. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Initierar en ny instans av klassen `Document`. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Initierar en ny instans av klassen `Document`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Detekterar alla ändringar som gjorts i dokumentlayouten sedan föregående anrop av `DetectLayoutChanges`. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Hämtar ett värde som indikerar om Aspose.Note automatiskt utför detektering av layoutändringar. |
| [getColor()](#getColor--) | Hämtar färgen. |
| [getCreationTime()](#getCreationTime--) | Hämtar skapandetiden. |
| [getDisplayName()](#getDisplayName--) | Hämtar visningsnamnet. |
| [getFileFormat()](#getFileFormat--) | Hämtar filformat (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Hämtar objektets globalt unika ID. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Hämtar `PageHistory` som innehåller full historik för varje sida som presenteras i ett dokument (den tidigaste på index 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Kontrollerar om ett dokument från en ström är krypterat. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Kontrollerar om ett dokument från en ström är krypterat. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Kontrollerar om ett dokument från en ström är krypterat. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Kontrollerar om ett dokument från en fil är krypterat. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Kontrollerar om ett dokument från en fil är krypterat. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Kontrollerar om ett dokument från en fil är krypterat. |
| [print()](#print--) | Skriver ut dokumentet med standardskrivaren. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Skriver ut dokumentet med standardskrivaren. |
| [print(String printerName)](#print-java.lang.String-) | Skriver ut dokumentet med standardskrivaren. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Skriver ut dokumentet med standardskrivaren. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Sparar OneNote-dokumentet till en ström. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Sparar OneNote-dokumentet till en ström med de angivna sparalternativen. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Sparar OneNote-dokumentet till en ström i det angivna formatet. |
| [save(String fileName)](#save-java.lang.String-) | Sparar OneNote-dokumentet till en fil. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Sparar OneNote-dokumentet till en fil med de angivna sparalternativen. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Sparar OneNote-dokumentet till en fil i det angivna formatet. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Anger ett värde som visar om Aspose.Note automatiskt utför detektering av layoutändringar. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Anger färgen. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Anger skapandetiden. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Anger visningsnamnet. |
### Document() {#Document--}
```
public Document()
```


Initierar en ny instans av klassen `Document`. Skapar ett tomt OneNote‑dokument.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Initierar en ny instans av klassen `Document`. Öppnar ett befintligt OneNote‑dokument från en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Initierar en ny instans av klassen `Document`. Öppnar ett befintligt OneNote‑dokument från en fil. Tillåter att ange ytterligare alternativ, såsom ett krypteringslösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Alternativ som används för att läsa in ett dokument. Kan vara null. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Initierar en ny instans av klassen `Document`. Öppnar ett befintligt OneNote‑dokument från en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inStream | java.io.InputStream | Strömmen. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Initierar en ny instans av klassen `Document`. Öppnar ett befintligt OneNote‑dokument från en ström. Tillåter att ange ytterligare alternativ, såsom ett krypteringslösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inStream | java.io.InputStream | Strömmen. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Alternativ som används för att läsa in ett dokument. Kan vara null. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Detekterar alla ändringar som gjorts i dokumentets layout sedan föregående anrop av `DetectLayoutChanges`. Om `AutomaticLayoutChangesDetectionEnabled` är satt till true används den automatiskt i början av dokumentexporten.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Hämtar ett värde som visar om Aspose.Note automatiskt utför detektering av layoutändringar. Standardvärdet är `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Hämtar färgen.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Hämtar skapandetiden.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Hämtar visningsnamnet.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Hämtar filformat (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Hämtar objektets globalt unika ID.

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


Hämtar `PageHistory` som innehåller full historik för varje sida som presenteras i ett dokument (den tidigaste på index 0). Den aktuella sidrevisionen kan nås som `PageHistory.current` och lagras separat från samlingen av historiska versioner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Den aktuella revisionen av en sida. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi läsa in hela dokumentet. Så kan denna metod leda till prestandapåverkan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen. |
| document | [Document\[\]](../../com.aspose.note/document) | Det inlästa dokumentet. |

**Returns:**
boolean – Returnerar true om dokumentet är krypterat, annars false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi läsa in hela dokumentet. Så kan denna metod leda till prestandapåverkan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Laddningsalternativen. |
| document | [Document\[\]](../../com.aspose.note/document) | Det inlästa dokumentet. |

**Returns:**
boolean – Returnerar true om dokumentet är krypterat, annars false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi läsa in hela dokumentet. Så kan denna metod leda till prestandapåverkan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen. |
| password | java.lang.String | Lösenordet för att dekryptera ett dokument. |
| document | [Document\[\]](../../com.aspose.note/document) | Det inlästa dokumentet. |

**Returns:**
boolean – Returnerar true om dokumentet är krypterat, annars false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi läsa in hela dokumentet. Så kan denna metod leda till prestandapåverkan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |
| document | [Document\[\]](../../com.aspose.note/document) | Det inlästa dokumentet. |

**Returns:**
boolean – Returnerar true om dokumentet är krypterat, annars false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi läsa in hela dokumentet. Så kan denna metod leda till prestandapåverkan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Laddningsalternativen. |
| document | [Document\[\]](../../com.aspose.note/document) | Det inlästa dokumentet. |

**Returns:**
boolean – Returnerar true om dokumentet är krypterat, annars false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi läsa in hela dokumentet. Så kan denna metod leda till prestandapåverkan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |
| password | java.lang.String | Lösenordet för att dekryptera ett dokument. |
| document | [Document\[\]](../../com.aspose.note/document) | Det inlästa dokumentet. |

**Returns:**
boolean – Returnerar true om dokumentet är krypterat, annars false.
### print() {#print--}
```
public void print()
```


Skriver ut dokumentet med standardskrivaren.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Skriver ut dokumentet med standardskrivaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Alternativ som används för att skriva ut ett dokument. Kan vara null. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Skriver ut dokumentet med standardskrivaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Skriver ut dokumentet med standardskrivaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Sparar OneNote-dokumentet till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.OutputStream | System.iO.stream där dokumentet kommer att sparas. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Sparar OneNote-dokumentet till en ström med de angivna sparalternativen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.OutputStream | System.iO.stream där dokumentet kommer att sparas. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Anger alternativen för hur dokumentet sparas i strömmen. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Sparar OneNote-dokumentet till en ström i det angivna formatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.OutputStream | System.iO.stream där dokumentet kommer att sparas. |
| format | int | Formatet i vilket dokumentet ska sparas. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Sparar OneNote-dokumentet till en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Det fullständiga namnet för filen. Om en fil med det angivna fullständiga namnet redan finns, skrivs den befintliga filen över. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Sparar OneNote-dokumentet till en fil med de angivna sparalternativen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Det fullständiga namnet för filen. Om en fil med det angivna fullständiga namnet redan finns, skrivs den befintliga filen över. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Anger alternativen för hur dokumentet sparas i filen. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Sparar OneNote-dokumentet till en fil i det angivna formatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Det fullständiga namnet för filen. Om en fil med det angivna fullständiga namnet redan finns, skrivs den befintliga filen över. |
| format | int | Formatet i vilket dokumentet ska sparas. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Anger ett värde som visar om Aspose.Note automatiskt utför detektering av layoutändringar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | Nytt värde. Kan vara null. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Anger färgen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color | Färgens värde. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Anger skapandetiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | DateTime:s värde. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Anger visningsnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | DateTime:s värde. |

