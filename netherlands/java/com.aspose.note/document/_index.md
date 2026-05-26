---
title: "Document"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een Aspose.Note-document voor."
type: docs
weight: 20
url: /nl/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Stelt een Aspose.Note-document voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Document()](#Document--) | Initialiseert een nieuw exemplaar van de `Document` klasse. |
| [Document(String filePath)](#Document-java.lang.String-) | Initialiseert een nieuw exemplaar van de `Document` klasse. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Initialiseert een nieuw exemplaar van de `Document` klasse. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de `Document` klasse. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Initialiseert een nieuw exemplaar van de `Document` klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Detecteert alle wijzigingen die zijn aangebracht in de documentindeling sinds de vorige `DetectLayoutChanges` oproep. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Haalt een waarde op die aangeeft of Aspose.Note automatisch detectie van indelingswijzigingen uitvoert. |
| [getColor()](#getColor--) | Haalt de kleur op. |
| [getCreationTime()](#getCreationTime--) | Haalt de creatietijd op. |
| [getDisplayName()](#getDisplayName--) | Haalt de weergavenaam op. |
| [getFileFormat()](#getFileFormat--) | Haalt het bestandsformaat op (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Haalt de wereldwijd unieke id van het object op. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Haalt de `PageHistory` op die de volledige geschiedenis bevat voor elke pagina die in een document wordt gepresenteerd (de vroegste op index 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Controleert of een document uit een stream versleuteld is. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Controleert of een document uit een stream versleuteld is. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Controleert of een document uit een stream versleuteld is. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Controleert of een document uit een bestand versleuteld is. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Controleert of een document uit een bestand versleuteld is. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Controleert of een document uit een bestand versleuteld is. |
| [print()](#print--) | Print het document met de standaardprinter. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Print het document met de standaardprinter. |
| [print(String printerName)](#print-java.lang.String-) | Print het document met de standaardprinter. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Print het document met de standaardprinter. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Slaat het OneNote-document op naar een stream. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Slaat het OneNote-document op naar een stream met de opgegeven opslagopties. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Slaat het OneNote-document op naar een stream in het opgegeven formaat. |
| [save(String fileName)](#save-java.lang.String-) | Slaat het OneNote-document op naar een bestand. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Slaat het OneNote-document op naar een bestand met de opgegeven opslagopties. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Slaat het OneNote-document op naar een bestand in het opgegeven formaat. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Stelt een waarde in die aangeeft of Aspose.Note automatisch detectie van lay-outwijzigingen uitvoert. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Stelt de kleur in. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Stelt de creatietijd in. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Stelt de weergavenaam in. |
### Document() {#Document--}
```
public Document()
```


Initialiseert een nieuw exemplaar van de `Document` klasse. Maakt een leeg OneNote-document aan.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Initialiseert een nieuw exemplaar van de `Document` klasse. Opent een bestaand OneNote-document uit een bestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de `Document` klasse. Opent een bestaand OneNote-document uit een bestand. Stelt toe om extra opties op te geven, zoals een encryptiewachtwoord.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opties die worden gebruikt om een document te laden. Kan null zijn. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Initialiseert een nieuw exemplaar van de `Document` klasse. Opent een bestaand OneNote-document uit een stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inStream | java.io.InputStream | De stream. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de `Document` klasse. Opent een bestaand OneNote-document uit een stream. Stelt toe om extra opties op te geven, zoals een encryptiewachtwoord.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inStream | java.io.InputStream | De stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opties die worden gebruikt om een document te laden. Kan null zijn. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Detecteert alle wijzigingen die zijn aangebracht in de documentlay-out sinds de vorige `DetectLayoutChanges`-aanroep. In het geval dat `AutomaticLayoutChangesDetectionEnabled` op true is ingesteld, wordt dit automatisch gebruikt aan het begin van de documentexport.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Haalt een waarde op die aangeeft of Aspose.Note automatisch detectie van lay-outwijzigingen uitvoert. Standaardwaarde is `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Haalt de kleur op.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Haalt de creatietijd op.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Haalt de weergavenaam op.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Haalt het bestandsformaat op (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Haalt de wereldwijd unieke id van het object op.

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


Haalt de `PageHistory` op die de volledige geschiedenis bevat voor elke pagina die in een document wordt gepresenteerd (de vroegste op index 0). De huidige paginarevisie kan worden benaderd als `PageHistory.current` en staat apart van de verzameling historische versies.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | De huidige revisie van een pagina. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Daarom kan deze methode leiden tot een prestatieverlies.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.InputStream | De stream. |
| document | [Document\[\]](../../com.aspose.note/document) | Het geladen document. |

**Returns:**
boolean - Retourneert true als het document versleuteld is, anders false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Daarom kan deze methode leiden tot een prestatieverlies.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.InputStream | De stream. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | De laadopties. |
| document | [Document\[\]](../../com.aspose.note/document) | Het geladen document. |

**Returns:**
boolean - Retourneert true als het document versleuteld is, anders false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Daarom kan deze methode leiden tot een prestatieverlies.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.InputStream | De stream. |
| password | java.lang.String | Het wachtwoord om een document te ontsleutelen. |
| document | [Document\[\]](../../com.aspose.note/document) | Het geladen document. |

**Returns:**
boolean - Retourneert true als het document versleuteld is, anders false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Daarom kan deze methode leiden tot een prestatieverlies.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |
| document | [Document\[\]](../../com.aspose.note/document) | Het geladen document. |

**Returns:**
boolean - Retourneert true als het document versleuteld is, anders false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Daarom kan deze methode leiden tot een prestatieverlies.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | De laadopties. |
| document | [Document\[\]](../../com.aspose.note/document) | Het geladen document. |

**Returns:**
boolean - Retourneert true als het document versleuteld is, anders false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Daarom kan deze methode leiden tot een prestatieverlies.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |
| password | java.lang.String | Het wachtwoord om een document te ontsleutelen. |
| document | [Document\[\]](../../com.aspose.note/document) | Het geladen document. |

**Returns:**
boolean - Retourneert true als het document versleuteld is, anders false.
### print() {#print--}
```
public void print()
```


Print het document met de standaardprinter.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Print het document met de standaardprinter.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Opties die worden gebruikt om een document af te drukken. Kan null zijn. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Print het document met de standaardprinter.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Print het document met de standaardprinter.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Slaat het OneNote-document op naar een stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.OutputStream | De System.iO.stream waar het document wordt opgeslagen. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Slaat het OneNote-document op naar een stream met de opgegeven opslagopties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.OutputStream | De System.iO.stream waar het document wordt opgeslagen. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Specificeert de opties hoe het document wordt opgeslagen in de stream. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Slaat het OneNote-document op naar een stream in het opgegeven formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.OutputStream | De System.iO.stream waar het document wordt opgeslagen. |
| format | int | Het formaat waarin het document moet worden opgeslagen. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Slaat het OneNote-document op naar een bestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | De volledige naam voor het bestand. Als er al een bestand met de opgegeven volledige naam bestaat, wordt het bestaande bestand overschreven. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Slaat het OneNote-document op naar een bestand met de opgegeven opslagopties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | De volledige naam voor het bestand. Als er al een bestand met de opgegeven volledige naam bestaat, wordt het bestaande bestand overschreven. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Specificeert de opties hoe het document in een bestand wordt opgeslagen. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Slaat het OneNote-document op naar een bestand in het opgegeven formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | De volledige naam voor het bestand. Als er al een bestand met de opgegeven volledige naam bestaat, wordt het bestaande bestand overschreven. |
| format | int | Het formaat waarin het document moet worden opgeslagen. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Stelt een waarde in die aangeeft of Aspose.Note automatisch detectie van lay-outwijzigingen uitvoert.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | Nieuwe waarde. Kan null zijn. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Stelt de kleur in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color | Waarde van Color. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Stelt de creatietijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | Waarde van DateTime. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Stelt de weergavenaam in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | Waarde van DateTime. |

