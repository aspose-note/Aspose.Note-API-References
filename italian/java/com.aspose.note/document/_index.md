---
title: "Document"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un documento **Aspose.Note**."
type: docs
weight: 20
url: /it/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Rappresenta un documento **Aspose.Note**.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Document()](#Document--) | Inizializza una nuova istanza della classe `Document`. |
| [Document(String filePath)](#Document-java.lang.String-) | Inizializza una nuova istanza della classe `Document`. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Inizializza una nuova istanza della classe `Document`. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Inizializza una nuova istanza della classe `Document`. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Inizializza una nuova istanza della classe `Document`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Rileva tutte le modifiche apportate al layout del documento dalla precedente chiamata a `DetectLayoutChanges`. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Ottiene un valore che indica se Aspose.Note esegue automaticamente il rilevamento delle modifiche al layout. |
| [getColor()](#getColor--) | Ottiene il colore. |
| [getCreationTime()](#getCreationTime--) | Ottiene l'ora di creazione. |
| [getDisplayName()](#getDisplayName--) | Ottiene il nome visualizzato. |
| [getFileFormat()](#getFileFormat--) | Restituisce il formato file (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Restituisce l'ID univoco globale dell'oggetto. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Ottiene il `PageHistory` che contiene la cronologia completa per ogni pagina presente in un documento (la più antica all'indice 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Verifica se un documento proveniente da uno stream è crittografato. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Verifica se un documento proveniente da uno stream è crittografato. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Verifica se un documento proveniente da uno stream è crittografato. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Verifica se un documento proveniente da un file è crittografato. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Verifica se un documento proveniente da un file è crittografato. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Verifica se un documento proveniente da un file è crittografato. |
| [print()](#print--) | Stampa il documento utilizzando la stampante predefinita. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Stampa il documento utilizzando la stampante predefinita. |
| [print(String printerName)](#print-java.lang.String-) | Stampa il documento utilizzando la stampante predefinita. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Stampa il documento utilizzando la stampante predefinita. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Salva il documento OneNote su uno stream. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Salva il documento OneNote su uno stream utilizzando le opzioni di salvataggio specificate. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Salva il documento OneNote su uno stream nel formato specificato. |
| [save(String fileName)](#save-java.lang.String-) | Salva il documento OneNote su un file. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Salva il documento OneNote su un file utilizzando le opzioni di salvataggio specificate. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Salva il documento OneNote su un file nel formato specificato. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Imposta un valore che indica se Aspose.Note esegue automaticamente il rilevamento delle modifiche al layout. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Imposta il colore. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Imposta l'ora di creazione. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Imposta il nome visualizzato. |
### Document() {#Document--}
```
public Document()
```


Inizializza una nuova istanza della classe `Document`. Crea un documento OneNote vuoto.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Inizializza una nuova istanza della classe `Document`. Apre un documento OneNote esistente da un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Inizializza una nuova istanza della classe `Document`. Apre un documento OneNote esistente da un file. Consente di specificare opzioni aggiuntive come una password di crittografia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opzioni utilizzate per caricare un documento. Può essere null. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Inizializza una nuova istanza della classe `Document`. Apre un documento OneNote esistente da uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inStream | java.io.InputStream | Lo stream. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Inizializza una nuova istanza della classe `Document`. Apre un documento OneNote esistente da uno stream. Consente di specificare opzioni aggiuntive come una password di crittografia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inStream | java.io.InputStream | Lo stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opzioni utilizzate per caricare un documento. Può essere null. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Rileva tutte le modifiche apportate al layout del documento dalla precedente chiamata `DetectLayoutChanges`. Nel caso in cui `AutomaticLayoutChangesDetectionEnabled` sia impostato su true, viene utilizzato automaticamente all'inizio dell'esportazione del documento.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Ottiene un valore che indica se Aspose.Note esegue automaticamente il rilevamento delle modifiche al layout. Il valore predefinito è `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Ottiene il colore.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Ottiene l'ora di creazione.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Ottiene il nome visualizzato.

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


Ottiene il `PageHistory` che contiene la cronologia completa per ogni pagina presente in un documento (la più antica all'indice 0). La revisione corrente della pagina è accessibile come `PageHistory.current` ed è contenuta separatamente dalla collezione delle versioni storiche.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | La revisione corrente di una pagina. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Verifica se un documento proveniente da uno stream è crittografato. Per verificarlo è necessario caricare completamente questo documento. Pertanto questo metodo può comportare un penalizzo sulle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Lo stream. |
| document | [Document\[\]](../../com.aspose.note/document) | Il documento caricato. |

**Returns:**
boolean - Restituisce true se il documento è crittografato, altrimenti false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Verifica se un documento proveniente da uno stream è crittografato. Per verificarlo è necessario caricare completamente questo documento. Pertanto questo metodo può comportare un penalizzo sulle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Lo stream. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Le opzioni di caricamento. |
| document | [Document\[\]](../../com.aspose.note/document) | Il documento caricato. |

**Returns:**
boolean - Restituisce true se il documento è crittografato, altrimenti false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Verifica se un documento proveniente da uno stream è crittografato. Per verificarlo è necessario caricare completamente questo documento. Pertanto questo metodo può comportare un penalizzo sulle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Lo stream. |
| password | java.lang.String | La password per decrittare un documento. |
| document | [Document\[\]](../../com.aspose.note/document) | Il documento caricato. |

**Returns:**
boolean - Restituisce true se il documento è crittografato, altrimenti false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Verifica se un documento proveniente da un file è crittografato. Per verificarlo è necessario caricare completamente questo documento. Pertanto questo metodo può comportare un penalizzo sulle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |
| document | [Document\[\]](../../com.aspose.note/document) | Il documento caricato. |

**Returns:**
boolean - Restituisce true se il documento è crittografato, altrimenti false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Verifica se un documento proveniente da un file è crittografato. Per verificarlo è necessario caricare completamente questo documento. Pertanto questo metodo può comportare un penalizzo sulle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Le opzioni di caricamento. |
| document | [Document\[\]](../../com.aspose.note/document) | Il documento caricato. |

**Returns:**
boolean - Restituisce true se il documento è crittografato, altrimenti false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Verifica se un documento proveniente da un file è crittografato. Per verificarlo è necessario caricare completamente questo documento. Pertanto questo metodo può comportare un penalizzo sulle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file. |
| password | java.lang.String | La password per decrittare un documento. |
| document | [Document\[\]](../../com.aspose.note/document) | Il documento caricato. |

**Returns:**
boolean - Restituisce true se il documento è crittografato, altrimenti false.
### print() {#print--}
```
public void print()
```


Stampa il documento utilizzando la stampante predefinita.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Stampa il documento utilizzando la stampante predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Opzioni utilizzate per stampare un documento. Può essere null. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Stampa il documento utilizzando la stampante predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Stampa il documento utilizzando la stampante predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Salva il documento OneNote su uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.OutputStream | Il System.iO.stream dove verrà salvato il documento. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Salva il documento OneNote su uno stream utilizzando le opzioni di salvataggio specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.OutputStream | Il System.iO.stream dove verrà salvato il documento. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Specifica le opzioni su come il documento viene salvato nello stream. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Salva il documento OneNote su uno stream nel formato specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.OutputStream | Il System.iO.stream dove verrà salvato il documento. |
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

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Salva il documento OneNote su un file utilizzando le opzioni di salvataggio specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome completo del file. Se un file con lo stesso nome completo esiste già, il file esistente viene sovrascritto. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Specifica le opzioni su come il documento viene salvato nel file. |

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

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Imposta un valore che indica se Aspose.Note esegue automaticamente il rilevamento delle modifiche al layout.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | Nuovo valore. Può essere null. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Imposta il colore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color | Valore del colore. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Imposta l'ora di creazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | Valore di DateTime. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Imposta il nome visualizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Valore di DateTime. |

