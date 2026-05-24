---
title: "Notebook"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt ein Aspose.Note-Notizbuch dar."
type: docs
weight: 56
url: /de/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Stellt ein Aspose.Note-Notizbuch dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Notebook()](#Notebook--) | Initialisiert eine neue Instanz der Klasse `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Initialisiert eine neue Instanz der Klasse `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Initialisiert eine neue Instanz der Klasse `Notebook`. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Ruft alle untergeordneten Knoten nach Knotentyp ab. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Fügt den Knoten am Ende der Liste hinzu. |
| [getColor()](#getColor--) | Liest oder setzt die Farbe. |
| [getCount()](#getCount--) | Liefert die Anzahl der im `Notebook` enthaltenen Elemente. |
| [getDisplayName()](#getDisplayName--) | Liest oder setzt den Anzeigenamen. |
| [getFileFormat()](#getFileFormat--) | Liefert das Dateiformat (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Liefert die global eindeutige ID des Objekts. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Liefert das untergeordnete Notizbuch‑Knoten anhand des angegebenen Index. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Liest oder setzt einen Wert, der angibt, ob die Historie aktiviert ist. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der durch die untergeordneten Knoten des `Notebook` iteriert. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Fügt einen untergeordneten Dokumentknoten hinzu. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Fügt einen untergeordneten Dokumentknoten hinzu. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Fügt einen untergeordneten Dokumentknoten hinzu. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Fügt einen untergeordneten Dokumentknoten hinzu. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Fügt einen untergeordneten Notizbuchknoten hinzu. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Fügt einen untergeordneten Notizbuchknoten hinzu. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Entfernt den untergeordneten Knoten. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Speichert das OneNote‑Dokument in einen Stream. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Speichert das OneNote‑Dokument in einen Stream unter Verwendung der angegebenen Speicheroptionen. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Speichert das OneNote‑Dokument in einen Stream im angegebenen Format. |
| [save(String fileName)](#save-java.lang.String-) | Speichert das OneNote‑Dokument in einer Datei. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Speichert das OneNote‑Dokument in einer Datei unter Verwendung der angegebenen Speicheroptionen. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Speichert das OneNote‑Dokument in einer Datei im angegebenen Format. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Liest oder setzt die Farbe. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Liest oder setzt den Anzeigenamen. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Liest oder setzt einen Wert, der angibt, ob die Historie aktiviert ist. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Initialisiert eine neue Instanz der Klasse `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Initialisiert eine neue Instanz der Klasse `Notebook`. Öffnet ein vorhandenes OneNote‑Notizbuch aus einer Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der `Notebook`-Klasse. Öffnet ein vorhandenes OneNote-Notizbuch aus einer Datei. Ermöglicht das Angeben zusätzlicher Optionen wie einer Kind-Lade-Strategie ("lazy"/instant).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Die Ladeoptionen. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Ruft alle untergeordneten Knoten nach Knotentyp ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Eine Liste von Kindknoten.

`T1`: Der Typ der Elemente in der zurückgegebenen Liste.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Fügt den Knoten am Ende der Liste hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Der Knoten zum Hinzufügen. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Liest oder setzt die Farbe.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Liefert die Anzahl der im `Notebook` enthaltenen Elemente.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Liest oder setzt den Anzeigenamen.

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

Wert: Die GUID.

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


Liefert das untergeordnete Notizbuch‑Knoten anhand des angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | Index zum Kindknoten. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Liest oder setzt einen Wert, der angibt, ob die Historie aktiviert ist.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Gibt einen Enumerator zurück, der durch die untergeordneten Knoten des `Notebook` iteriert.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - Ein `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Fügt einen Kind-Dokumentknoten hinzu. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.InputStream | Der Stream. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Fügt einen Kind-Dokumentknoten hinzu. Öffnet ein vorhandenes OneNote-Dokument aus einem Stream. Ermöglicht das Angeben zusätzlicher Ladeoptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.InputStream | Der Stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Die Ladeoptionen. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Fügt einen Kind-Dokumentknoten hinzu. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Fügt einen Kind-Dokumentknoten hinzu. Öffnet ein vorhandenes OneNote-Dokument aus einer Datei. Ermöglicht das Angeben zusätzlicher Ladeoptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Die Ladeoptionen. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Fügt einen Kind-Notizbuchknoten hinzu. Öffnet ein vorhandenes OneNote-Notizbuch aus einer Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Fügt einen Kind-Notizbuchknoten hinzu. Öffnet ein vorhandenes OneNote-Notizbuch aus einer Datei. Ermöglicht das Angeben zusätzlicher Ladeoptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Die Ladeoptionen. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Entfernt den untergeordneten Knoten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Der Knoten zum Entfernen. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Speichert das OneNote‑Dokument in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.OutputStream | Der Stream. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Speichert das OneNote‑Dokument in einen Stream unter Verwendung der angegebenen Speicheroptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.OutputStream | Der Stream. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Gibt die Optionen an, wie das Dokument gespeichert wird. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Speichert das OneNote‑Dokument in einen Stream im angegebenen Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.OutputStream | Der Stream. |
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

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Speichert das OneNote‑Dokument in einer Datei unter Verwendung der angegebenen Speicheroptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der vollständige Name für die Datei. Wenn bereits eine Datei mit dem angegebenen vollständigen Namen existiert, wird die vorhandene Datei überschrieben. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Gibt die Optionen an, wie das Dokument in einer Datei gespeichert wird. |

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

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Liest oder setzt die Farbe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Liest oder setzt den Anzeigenamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Liest oder setzt einen Wert, der angibt, ob die Historie aktiviert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

