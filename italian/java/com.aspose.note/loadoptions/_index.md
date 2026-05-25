---
title: "LoadOptions"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Opzioni utilizzate per caricare un documento."
type: docs
weight: 46
url: /it/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Opzioni utilizzate per caricare un documento.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Inizializza una nuova istanza della classe `LoadOptions`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Ottiene o imposta una password per il contenuto del documento crittografato. |
| [getLoadHistory()](#getLoadHistory--) | Ottiene o imposta un valore che indica se il caricatore di documenti deve ignorare la cronologia. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Ottiene o imposta una password per il contenuto del documento crittografato. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Ottiene o imposta un valore che indica se il caricatore di documenti deve ignorare la cronologia. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Inizializza una nuova istanza della classe `LoadOptions`.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Ottiene o imposta una password per il contenuto del documento crittografato. Il valore è ignorato nel caso in cui il documento non sia protetto da password.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Ottiene o imposta un valore che indica se il caricatore di documenti deve ignorare la cronologia. Usa questa opzione per ridurre l'utilizzo di memoria e CPU. Il valore predefinito è `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Ottiene o imposta una password per il contenuto del documento crittografato. Il valore è ignorato nel caso in cui il documento non sia protetto da password.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Ottiene o imposta un valore che indica se il caricatore di documenti deve ignorare la cronologia. Usa questa opzione per ridurre l'utilizzo di memoria e CPU. Il valore predefinito è `true`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

