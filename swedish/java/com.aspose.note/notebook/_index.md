---
title: "Anteckningsbok"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en **Aspose.Note**-anteckningsbok."
type: docs
weight: 56
url: /sv/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Representerar en **Aspose.Note**-anteckningsbok.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Notebook()](#Notebook--) | Initierar en ny instans av klassen `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Initierar en ny instans av klassen `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Initierar en ny instans av klassen `Notebook`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Hämta alla underordnade noder efter nodtypen. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Lägger till noden i slutet av listan. |
| [getColor()](#getColor--) | Hämtar eller anger färgen. |
| [getCount()](#getCount--) | Hämtar antalet element som finns i `Notebook`. |
| [getDisplayName()](#getDisplayName--) | Hämtar eller anger visningsnamnet. |
| [getFileFormat()](#getFileFormat--) | Hämtar filformat (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Hämtar objektets globalt unika ID. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Hämtar en underordnad nod i anteckningsboken med det angivna indexet. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Hämtar eller anger ett värde som indikerar om historiken är aktiverad. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom underordnade noder i `Notebook`. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Lägger till en underordnad dokumentnod. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Lägger till en underordnad dokumentnod. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Lägger till en underordnad dokumentnod. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Lägger till en underordnad dokumentnod. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Lägger till en underordnad anteckningsboksnod. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Lägger till en underordnad anteckningsboksnod. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Tar bort den underordnade noden. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Sparar OneNote-dokumentet till en ström. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Sparar OneNote-dokumentet till en ström med de angivna sparalternativen. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Sparar OneNote-dokumentet till en ström i det angivna formatet. |
| [save(String fileName)](#save-java.lang.String-) | Sparar OneNote-dokumentet till en fil. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Sparar OneNote-dokumentet till en fil med de angivna sparalternativen. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Sparar OneNote-dokumentet till en fil i det angivna formatet. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Hämtar eller anger färgen. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Hämtar eller anger visningsnamnet. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Hämtar eller anger ett värde som indikerar om historiken är aktiverad. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Initierar en ny instans av klassen `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Initierar en ny instans av klassen `Notebook`. Öppnar en befintlig OneNote-anteckningsbok från en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Initierar en ny instans av klassen `Notebook`. Öppnar en befintlig OneNote-anteckningsbok från en fil. Tillåter att ange ytterligare alternativ såsom en laddningsstrategi för barn ("lazy"/instant).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Laddningsalternativen. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Hämta alla underordnade noder efter nodtypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - En lista med barnnoder.

`T1`: Typen av element i den returnerade listan.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Lägger till noden i slutet av listan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Noden att lägga till. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Hämtar eller anger färgen.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar antalet element som finns i `Notebook`.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Hämtar eller anger visningsnamnet.

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

Värde: GUID:en.

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


Hämtar en underordnad nod i anteckningsboken med det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Index till barnnod. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Hämtar eller anger ett värde som indikerar om historiken är aktiverad.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Returnerar en enumerator som itererar genom underordnade noder i `Notebook`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - En `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Lägger till en barn-dokumentnod. Öppnar ett befintligt OneNote-dokument från en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Lägger till en barn-dokumentnod. Öppnar ett befintligt OneNote-dokument från en ström. Tillåter att ange ytterligare laddningsalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Laddningsalternativen. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Lägger till en barn-dokumentnod. Öppnar ett befintligt OneNote-dokument från en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Lägger till en barn-dokumentnod. Öppnar ett befintligt OneNote-dokument från en fil. Tillåter att ange ytterligare laddningsalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Laddningsalternativen. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Lägger till en barn-anteckningsboksnod. Öppnar en befintlig OneNote-anteckningsbok från en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Lägger till en barn-anteckningsboksnod. Öppnar en befintlig OneNote-anteckningsbok från en fil. Tillåter att ange ytterligare laddningsalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Laddningsalternativen. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Tar bort den underordnade noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Noden att ta bort. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Sparar OneNote-dokumentet till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.OutputStream | Strömmen. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Sparar OneNote-dokumentet till en ström med de angivna sparalternativen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.OutputStream | Strömmen. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Anger alternativen för hur dokumentet sparas. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Sparar OneNote-dokumentet till en ström i det angivna formatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.OutputStream | Strömmen. |
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

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Sparar OneNote-dokumentet till en fil med de angivna sparalternativen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Det fullständiga namnet för filen. Om en fil med det angivna fullständiga namnet redan finns, skrivs den befintliga filen över. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Anger alternativen för hur dokumentet sparas i filen. |

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

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Hämtar eller anger färgen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Hämtar eller anger visningsnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Hämtar eller anger ett värde som indikerar om historiken är aktiverad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

