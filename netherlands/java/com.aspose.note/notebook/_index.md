---
title: "Notitieboek"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een Aspose.Note-notitieblok voor."
type: docs
weight: 56
url: /nl/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Stelt een Aspose.Note-notitieblok voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Notebook()](#Notebook--) | Initialiseert een nieuw exemplaar van de `Notebook`-klasse. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Initialiseert een nieuw exemplaar van de `Notebook`-klasse. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Initialiseert een nieuw exemplaar van de `Notebook`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Haalt alle kindknopen op op basis van het knooptype. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Voegt de knoop toe aan het einde van de lijst. |
| [getColor()](#getColor--) | Haalt de kleur op of stelt deze in. |
| [getCount()](#getCount--) | Haalt het aantal elementen op dat in de `Notebook` zit. |
| [getDisplayName()](#getDisplayName--) | Haalt de weergavenaam op of stelt deze in. |
| [getFileFormat()](#getFileFormat--) | Haalt het bestandsformaat op (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Haalt de wereldwijd unieke id van het object op. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Haalt een kindknoop van het notitieboek op op basis van de opgegeven index. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Haalt een waarde op of stelt deze in die aangeeft of de geschiedenis is ingeschakeld. |
| [iterator()](#iterator--) | Retourneert een enumerator die door de kindknopen van de `Notebook` iterereert. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Voegt een kinddocumentknoop toe. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Voegt een kinddocumentknoop toe. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Voegt een kinddocumentknoop toe. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Voegt een kinddocumentknoop toe. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Voegt een kindnotitieboekknoop toe. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Voegt een kindnotitieboekknoop toe. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Verwijdert de kindknoop. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Slaat het OneNote-document op naar een stream. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Slaat het OneNote-document op naar een stream met de opgegeven opslagopties. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Slaat het OneNote-document op naar een stream in het opgegeven formaat. |
| [save(String fileName)](#save-java.lang.String-) | Slaat het OneNote-document op naar een bestand. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Slaat het OneNote-document op naar een bestand met de opgegeven opslagopties. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Slaat het OneNote-document op naar een bestand in het opgegeven formaat. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Haalt de kleur op of stelt deze in. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Haalt de weergavenaam op of stelt deze in. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Haalt een waarde op of stelt deze in die aangeeft of de geschiedenis is ingeschakeld. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Initialiseert een nieuw exemplaar van de `Notebook`-klasse.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Initialiseert een nieuw exemplaar van de `Notebook`-klasse. Opent een bestaand OneNote-notitieboek vanuit een bestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de `Notebook`-klasse. Opent een bestaande OneNote-notebook vanuit een bestand. Staat toe extra opties op te geven, zoals een laadsstrategie voor kinderen (\"lazy\"/instant).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | De laadopties. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Haalt alle kindknopen op op basis van het knooptype.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Een lijst van kindknooppunten.

`T1`: Het type van elementen in de geretourneerde lijst.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Voegt de knoop toe aan het einde van de lijst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Het toe te voegen knooppunt. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Haalt de kleur op of stelt deze in.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Haalt het aantal elementen op dat in de `Notebook` zit.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Haalt de weergavenaam op of stelt deze in.

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

Waarde: De GUID.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


Haalt een kindknoop van het notitieboek op op basis van de opgegeven index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | Index naar kindknooppunt. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Haalt een waarde op of stelt deze in die aangeeft of de geschiedenis is ingeschakeld.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Retourneert een enumerator die door de kindknopen van de `Notebook` iterereert.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - Een `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Voegt een kinddocumentknooppunt toe. Opent een bestaand OneNote-document vanuit een stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.InputStream | De stream. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Voegt een kinddocumentknooppunt toe. Opent een bestaand OneNote-document vanuit een stream. Staat toe extra laadopties op te geven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.InputStream | De stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | De laadopties. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Voegt een kinddocumentknooppunt toe. Opent een bestaand OneNote-document vanuit een bestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Voegt een kinddocumentknooppunt toe. Opent een bestaand OneNote-document vanuit een bestand. Staat toe extra laadopties op te geven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | De laadopties. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Voegt een kindnotebookknooppunt toe. Opent een bestaande OneNote-notebook vanuit een bestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Voegt een kindnotebookknooppunt toe. Opent een bestaande OneNote-notebook vanuit een bestand. Staat toe extra laadopties op te geven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String | Het bestandspad. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | De laadopties. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Verwijdert de kindknoop.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Het te verwijderen knooppunt. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Slaat het OneNote-document op naar een stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.OutputStream | De stream. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Slaat het OneNote-document op naar een stream met de opgegeven opslagopties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.OutputStream | De stream. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Specificeert de opties hoe het document wordt opgeslagen. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Slaat het OneNote-document op naar een stream in het opgegeven formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.OutputStream | De stream. |
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

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Slaat het OneNote-document op naar een bestand met de opgegeven opslagopties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | De volledige naam voor het bestand. Als er al een bestand met de opgegeven volledige naam bestaat, wordt het bestaande bestand overschreven. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Specificeert de opties hoe het document in een bestand wordt opgeslagen. |

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

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Haalt de kleur op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Haalt de weergavenaam op of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Haalt een waarde op of stelt deze in die aangeeft of de geschiedenis is ingeschakeld.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

