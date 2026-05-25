---
title: "RichText"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un testo ricco."
type: docs
weight: 82
url: /it/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Rappresenta un testo ricco.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [RichText()](#RichText--) | Inizializza una nuova istanza della classe [RichText](../../com.aspose.note/richtext). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [append(String value)](#append-java.lang.String-) | Aggiunge una stringa all'ultimo intervallo di testo. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Aggiunge una stringa alla fine. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Aggiunge una stringa all'inizio del primo intervallo di testo. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Aggiunge una stringa all'inizio. |
| [clear()](#clear--) | Cancella il contenuto di questa istanza. |
| [getAlignment()](#getAlignment--) | Ottiene l'allineamento. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene l'ora dell'ultima modifica. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Ottiene l'interlinea. |
| [getParagraphStyle()](#getParagraphStyle--) | Ottiene lo stile del paragrafo. |
| [getSpaceAfter()](#getSpaceAfter--) | Ottiene la quantità minima di spazio dopo. |
| [getSpaceBefore()](#getSpaceBefore--) | Ottiene la quantità minima di spazio prima. |
| [getStyles()](#getStyles--) | Ottiene gli stili. |
| [getTags()](#getTags--) | Ottiene l'elenco di tutti i tag di un paragrafo. |
| [getText()](#getText--) | Ottiene il testo. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Restituisce l'indice basato su zero della prima occorrenza del carattere Unicode specificato in questa stringa. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Restituisce l'indice basato su zero della prima occorrenza del carattere Unicode specificato in questa stringa. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Restituisce l'indice basato su zero della prima occorrenza del carattere specificato in questa istanza. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Restituisce l'indice basato su zero della prima occorrenza della stringa specificata in questa istanza. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Restituisce l'indice basato su zero della prima occorrenza della stringa specificata in questa istanza. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Restituisce l'indice basato su zero della prima occorrenza della stringa specificata in questa istanza. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Restituisce l'indice basato su zero della prima occorrenza della stringa specificata nell'istanza corrente. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Restituisce l'indice basato su zero della prima occorrenza della stringa specificata nell'istanza corrente. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Restituisce l'indice basato su zero della prima occorrenza della stringa specificata nell'istanza corrente. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Inserisce una stringa specificata in una posizione di indice specificata in questa istanza. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Inserisce una stringa specificata con lo stile specificato in una posizione di indice specificata in questa istanza. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Rimuove tutti i caratteri nell'istanza corrente, a partire da una posizione specificata e continuando fino all'ultima posizione. |
| [remove(int startIndex, int count)](#remove-int-int-) | Rimuove un numero specificato di caratteri nell'istanza corrente a partire da una posizione specificata. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Sostituisce tutte le occorrenze di un carattere Unicode specificato in questa istanza con un altro carattere Unicode specificato. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Sostituisce tutte le occorrenze di una stringa specificata nell'istanza corrente con un'altra stringa specificata. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Sostituisce tutte le occorrenze di una stringa specificata nell'istanza corrente con un'altra stringa specificata nello stile specificato. |
| [setAlignment(int value)](#setAlignment-int-) | Imposta l'allineamento. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Imposta l'ora dell'ultima modifica. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Imposta l'interlinea. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Imposta lo stile del paragrafo. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Imposta la quantità minima di spazio dopo. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Imposta la quantità minima di spazio prima. |
| [setText(String value)](#setText-java.lang.String-) | Imposta il testo. |
| [trim()](#trim--) | Rimuove tutti i caratteri di spazio bianco iniziali e finali. |
| [trim(char trimChar)](#trim-char-) | Rimuove tutte le occorrenze iniziali e finali di un carattere. |
| [trim(char[] trimChars)](#trim-char...-) | Rimuove tutte le occorrenze iniziali e finali di un insieme di caratteri specificato in un array. |
| [trimEnd()](#trimEnd--) | Rimuove tutti i caratteri di spazio bianco finali. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Rimuove tutte le occorrenze finali di un carattere. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Rimuove tutte le occorrenze finali di un insieme di caratteri specificato in un array. |
| [trimStart()](#trimStart--) | Rimuove tutti i caratteri di spazio bianco iniziali. |
| [trimStart(char trimChar)](#trimStart-char-) | Rimuove tutte le occorrenze iniziali di un carattere specificato. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Rimuove tutte le occorrenze iniziali di un insieme di caratteri specificato in un array. |
### RichText() {#RichText--}
```
public RichText()
```


Inizializza una nuova istanza della classe [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Aggiunge una stringa all'ultimo intervallo di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore aggiunto. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Aggiunge una stringa alla fine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore aggiunto. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Lo stile della stringa aggiunta. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Aggiunge una stringa all'inizio del primo intervallo di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore aggiunto. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Aggiunge una stringa all'inizio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore aggiunto. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Lo stile della stringa aggiunta. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Cancella il contenuto di questa istanza.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Ottiene l'allineamento.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Ottiene l'ora dell'ultima modifica.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


Ottiene l'interlinea.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Ottiene lo stile del paragrafo. Queste impostazioni sono utilizzate se non esiste un oggetto TextStyle corrispondente nella collezione [getStyles](../../com.aspose.note/richtext\#getStyles) oppure questo oggetto non specifica l'impostazione necessaria.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Ottiene la quantità minima di spazio dopo.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Ottiene la quantità minima di spazio prima.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Ottiene gli stili.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Ottiene l'elenco di tutti i tag di un paragrafo.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Ottiene il testo. La stringa NON DEVE contenere alcun carattere con valore 10 (line feed).

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


Restituisce l'indice basato su zero della prima occorrenza del carattere Unicode specificato in questa stringa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char | Il valore. |

**Returns:**
int - Il `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Restituisce l'indice basato su zero della prima occorrenza del carattere Unicode specificato in questa stringa. La ricerca inizia da una posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char | Il valore. |
| startIndex | int | La posizione di ricerca iniziale |

**Returns:**
int - Il `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Restituisce l'indice basato su zero della prima occorrenza del carattere specificato in questa istanza. La ricerca inizia da una posizione di carattere specificata ed esamina un numero specificato di posizioni di carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char | Il valore. |
| startIndex | int | La posizione di ricerca iniziale |
| count | int | Il conteggio. |

**Returns:**
int - Il `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Restituisce l'indice basato su zero della prima occorrenza della stringa specificata in questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore. |

**Returns:**
int - Il `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Restituisce l'indice basato su zero della prima occorrenza della stringa specificata in questa istanza. La ricerca inizia a una posizione di carattere specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore. |
| startIndex | int | La posizione di ricerca iniziale |

**Returns:**
int - Il `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Restituisce l'indice basato su zero della prima occorrenza della stringa specificata in questa istanza. La ricerca inizia a una posizione di carattere specificata ed esamina un numero specificato di posizioni di carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore. |
| startIndex | int | La posizione di ricerca iniziale |
| count | int | Il conteggio. |

**Returns:**
int - Il `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Restituisce l'indice basato su zero della prima occorrenza della stringa specificata nell'istanza corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore. |
| startIndex | int | La posizione di ricerca iniziale |
| count | int | Il conteggio. |
| comparisonType | short | Il tipo di ricerca da utilizzare per la stringa specificata |

**Returns:**
int - Il `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Restituisce l'indice basato su zero della prima occorrenza della stringa specificata nell'istanza corrente. Un parametro specifica il tipo di ricerca da utilizzare per la stringa specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore. |
| comparisonType | short | Il tipo di ricerca da utilizzare per la stringa specificata |

**Returns:**
int - Il `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Restituisce l'indice basato su zero della prima occorrenza della stringa specificata nell'istanza corrente. I parametri specificano la posizione di avvio della ricerca nella stringa corrente e il tipo di ricerca da utilizzare per la stringa specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore. |
| startIndex | int | La posizione di ricerca iniziale |
| comparisonType | short | Il tipo di ricerca da utilizzare per la stringa specificata |

**Returns:**
int - Il `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Inserisce una stringa specificata in una posizione di indice specificata in questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice di inizio. |
| valore | java.lang.String | Il valore. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Inserisce una stringa specificata con lo stile specificato in una posizione di indice specificata in questa istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice di inizio. |
| valore | java.lang.String | Il valore. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Lo stile. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


Rimuove tutti i caratteri nell'istanza corrente, a partire da una posizione specificata e continuando fino all'ultima posizione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice di inizio. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Rimuove un numero specificato di caratteri nell'istanza corrente a partire da una posizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice di inizio. |
| count | int | Il conteggio. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Sostituisce tutte le occorrenze di un carattere Unicode specificato in questa istanza con un altro carattere Unicode specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldChar | char | Il vecchio carattere. |
| newChar | char | Il nuovo carattere. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Sostituisce tutte le occorrenze di una stringa specificata nell'istanza corrente con un'altra stringa specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldValue | java.lang.String | Il valore vecchio. |
| newValue | java.lang.String | Il nuovo valore. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Sostituisce tutte le occorrenze di una stringa specificata nell'istanza corrente con un'altra stringa specificata nello stile specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldValue | java.lang.String | Il valore vecchio. |
| newValue | java.lang.String | Il nuovo valore. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Lo stile del nuovo valore. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Imposta l'allineamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Imposta l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Imposta l'interlinea.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Imposta lo stile del paragrafo. Queste impostazioni vengono utilizzate se non esiste un oggetto TextStyle corrispondente nella collezione [getStyles](../../com.aspose.note/richtext\#getStyles) oppure se questo oggetto non specifica un'impostazione necessaria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Imposta la quantità minima di spazio dopo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Imposta la quantità minima di spazio prima.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Imposta il testo. La stringa NON DEVE contenere alcun carattere con valore 10 (a capo).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Rimuove tutti i caratteri di spazio bianco iniziali e finali.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Rimuove tutte le occorrenze iniziali e finali di un carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| trimChar | char | Il carattere di trim. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Rimuove tutte le occorrenze iniziali e finali di un insieme di caratteri specificato in un array.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| trimChars | char[] | I caratteri di ritaglio. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Rimuove tutti i caratteri di spazio bianco finali.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Rimuove tutte le occorrenze finali di un carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| trimChar | char | Il carattere di trim. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Rimuove tutte le occorrenze finali di un insieme di caratteri specificato in un array.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| trimChars | char[] | I caratteri di ritaglio. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Rimuove tutti i caratteri di spazio bianco iniziali.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Rimuove tutte le occorrenze iniziali di un carattere specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| trimChar | char | Il carattere di trim. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Rimuove tutte le occorrenze iniziali di un insieme di caratteri specificato in un array.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| trimChars | char[] | I caratteri di ritaglio. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
