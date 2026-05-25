---
title: "Notebook"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un taccuino Aspose.Note."
type: docs
weight: 56
url: /it/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Rappresenta un taccuino Aspose.Note.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Notebook()](#Notebook--) | Inizializza una nuova istanza della classe `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Inizializza una nuova istanza della classe `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Inizializza una nuova istanza della classe `Notebook`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Ottieni tutti i nodi figli per tipo di nodo. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Aggiunge il nodo alla fine dell'elenco. |
| [getColor()](#getColor--) | Ottiene o imposta il colore. |
| [getCount()](#getCount--) | Restituisce il numero di elementi contenuti nel `Notebook`. |
| [getDisplayName()](#getDisplayName--) | Ottiene o imposta il nome visualizzato. |
| [getFileFormat()](#getFileFormat--) | Restituisce il formato file (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Restituisce l'ID univoco globale dell'oggetto. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Restituisce il nodo figlio del notebook all'indice specificato. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Ottiene o imposta un valore che indica se la cronologia è abilitata. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso i nodi figli del `Notebook`. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Aggiunge un nodo documento figlio. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Aggiunge un nodo documento figlio. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Aggiunge un nodo documento figlio. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Aggiunge un nodo documento figlio. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Aggiunge un nodo notebook figlio. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Aggiunge un nodo notebook figlio. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Rimuove il nodo figlio. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Salva il documento OneNote su uno stream. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Salva il documento OneNote su uno stream utilizzando le opzioni di salvataggio specificate. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Salva il documento OneNote su uno stream nel formato specificato. |
| [save(String fileName)](#save-java.lang.String-) | Salva il documento OneNote su un file. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Salva il documento OneNote su un file utilizzando le opzioni di salvataggio specificate. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Salva il documento OneNote su un file nel formato specificato. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Ottiene o imposta il colore. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Ottiene o imposta il nome visualizzato. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Ottiene o imposta un valore che indica se la cronologia è abilitata. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Inizializza una nuova istanza della classe `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Inizializza una nuova istanza della classe `Notebook`. Apre un notebook OneNote esistente da un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe `Notebook`. Apre un blocco note OneNote esistente da un file. Consente di specificare opzioni aggiuntive come una strategia di caricamento dei figli ("lazy"/instant).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Le opzioni di caricamento. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Ottieni tutti i nodi figli per tipo di nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Un elenco di nodi figli.

`T1`: Il tipo di elementi nella lista restituita.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Aggiunge il nodo alla fine dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Il nodo da aggiungere. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Ottiene o imposta il colore.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Restituisce il numero di elementi contenuti nel `Notebook`.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Ottiene o imposta il nome visualizzato.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Restituisce il formato file (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Restituisce l'ID univoco globale dell'oggetto.

Valore: Il GUID.

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


Restituisce il nodo figlio del notebook all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | Indice al nodo figlio. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Ottiene o imposta un valore che indica se la cronologia è abilitata.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Restituisce un enumeratore che itera attraverso i nodi figli del `Notebook`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - Un `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Aggiunge un nodo documento figlio. Apre un documento OneNote esistente da uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Lo stream. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Aggiunge un nodo documento figlio. Apre un documento OneNote esistente da uno stream. Consente di specificare opzioni di caricamento aggiuntive.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Lo stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Le opzioni di caricamento. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Aggiunge un nodo documento figlio. Apre un documento OneNote esistente da un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Aggiunge un nodo documento figlio. Apre un documento OneNote esistente da un file. Consente di specificare opzioni di caricamento aggiuntive.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Le opzioni di caricamento. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Aggiunge un nodo blocco note figlio. Apre un blocco note OneNote esistente da un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Aggiunge un nodo blocco note figlio. Apre un blocco note OneNote esistente da un file. Consente di specificare opzioni di caricamento aggiuntive.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Le opzioni di caricamento. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Rimuove il nodo figlio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Il nodo da rimuovere. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Salva il documento OneNote su uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.OutputStream | Lo stream. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Salva il documento OneNote su uno stream utilizzando le opzioni di salvataggio specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.OutputStream | Lo stream. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Specifica le opzioni su come il documento viene salvato. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Salva il documento OneNote su uno stream nel formato specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.OutputStream | Lo stream. |
| format | int | Il formato in cui salvare il documento. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Salva il documento OneNote su un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome completo del file. Se un file con lo stesso nome completo esiste già, il file esistente viene sovrascritto. |

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Salva il documento OneNote su un file utilizzando le opzioni di salvataggio specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome completo del file. Se un file con lo stesso nome completo esiste già, il file esistente viene sovrascritto. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Specifica le opzioni su come il documento viene salvato nel file. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Salva il documento OneNote su un file nel formato specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome completo del file. Se un file con lo stesso nome completo esiste già, il file esistente viene sovrascritto. |
| format | int | Il formato in cui salvare il documento. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Ottiene o imposta il colore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Ottiene o imposta il nome visualizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Ottiene o imposta un valore che indica se la cronologia è abilitata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

