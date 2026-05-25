---
title: "NumberList"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta l'elenco numerato o puntato."
type: docs
weight: 64
url: /it/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Rappresenta l'elenco numerato o puntato.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Inizializza una nuova istanza della classe `NumberList`. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Inizializza una nuova istanza della classe `NumberList`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| [getFont()](#getFont--) | Ottiene o imposta il nome del carattere. |
| [getFontColor()](#getFontColor--) | Ottiene o imposta il colore del carattere. |
| [getFontSize()](#getFontSize--) | Ottiene o imposta la dimensione del carattere. |
| [getFormat()](#getFormat--) | Ottiene o imposta il formato dell'intestazione di riga. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene o imposta l'ora dell'ultima modifica. |
| [getNumberFormat()](#getNumberFormat--) | Ottiene o imposta il formato numerico usato per un gruppo di oggetti numerati automaticamente. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Ottiene l'intestazione dell'elenco numerato. |
| [getRestart()](#getRestart--) | Ottiene o imposta il valore numerico che sovrascrive il valore numerico automatico dell'elemento dell'elenco. |
| [hashCode()](#hashCode--) | Funziona come funzione hash per il tipo. |
| [isBold()](#isBold--) | Ottiene o imposta un valore che indica se lo stile del testo è grassetto. |
| [isItalic()](#isItalic--) | Ottiene o imposta un valore che indica se lo stile del testo è corsivo. |
| [setBold(boolean value)](#setBold-boolean-) | Ottiene o imposta un valore che indica se lo stile del testo è grassetto. |
| [setFont(String value)](#setFont-java.lang.String-) | Ottiene o imposta il nome del carattere. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Ottiene o imposta il colore del carattere. |
| [setFontSize(int value)](#setFontSize-int-) | Ottiene o imposta la dimensione del carattere. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Ottiene o imposta il formato dell'intestazione di riga. |
| [setItalic(boolean value)](#setItalic-boolean-) | Ottiene o imposta un valore che indica se lo stile del testo è corsivo. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ottiene o imposta l'ora dell'ultima modifica. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Ottiene o imposta il formato numerico usato per un gruppo di oggetti numerati automaticamente. |
| [setRestart(int value)](#setRestart-int-) | Ottiene o imposta il valore numerico che sovrascrive il valore numerico automatico dell'elemento dell'elenco. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Inizializza una nuova istanza della classe `NumberList`. Questa istanza rappresenta un elenco puntato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Un simbolo che rappresenta un punto elenco. |
| font | java.lang.String | Un font per il punto elenco. |
| fontSize | int | Una dimensione del font per il punto elenco. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Inizializza una nuova istanza della classe `NumberList`. Questa istanza rappresenta un elenco numerato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | java.lang.String | Il formato dell'intestazione numerata. |
| numberFormat | byte | Il formato del numero nell'intestazione. |
| font | java.lang.String | Un carattere per l'intestazione numerata. |
| fontSize | int | Una dimensione del carattere per l'intestazione numerata. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Determina se l'oggetto specificato è uguale all'oggetto corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | L'oggetto. |

**Returns:**
boolean - Il `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina se l'oggetto specificato è uguale all'oggetto corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto. |

**Returns:**
boolean - Il `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Ottiene o imposta il nome del carattere.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Ottiene o imposta il colore del carattere.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Ottiene o imposta la dimensione del carattere.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Ottiene o imposta il formato dell'intestazione di riga. Per gli elenchi puntati rappresenta un simbolo di punto.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Ottiene o imposta l'ora dell'ultima modifica.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Ottiene o imposta il formato numerico usato per un gruppo di oggetti numerati automaticamente. Deve essere null per gli elenchi puntati.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Ottiene l'intestazione dell'elenco numerato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sequenceNumber | int | Il numero di sequenza nell'elenco numerato. |

**Returns:**
java.lang.String - Una rappresentazione stringa del numero di sequenza specificato.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Ottiene o imposta il valore numerico che sovrascrive il valore numerico automatico dell'elemento dell'elenco.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Funziona come funzione hash per il tipo.

**Returns:**
int - Il `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Ottiene o imposta un valore che indica se lo stile del testo è grassetto.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Ottiene o imposta un valore che indica se lo stile del testo è corsivo.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Ottiene o imposta un valore che indica se lo stile del testo è grassetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Ottiene o imposta il nome del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Ottiene o imposta il colore del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Ottiene o imposta la dimensione del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Ottiene o imposta il formato dell'intestazione di riga. Per gli elenchi puntati rappresenta un simbolo di punto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Ottiene o imposta un valore che indica se lo stile del testo è corsivo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ottiene o imposta l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Ottiene o imposta il formato numerico usato per un gruppo di oggetti numerati automaticamente. Deve essere null per gli elenchi puntati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Ottiene o imposta il valore numerico che sovrascrive il valore numerico automatico dell'elemento dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

