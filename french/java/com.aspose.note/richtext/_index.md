---
title: "RichText"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un texte enrichi."
type: docs
weight: 82
url: /fr/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Représente un texte enrichi.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [RichText()](#RichText--) | Initialise une nouvelle instance de la classe [RichText](../../com.aspose.note/richtext). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [append(String value)](#append-java.lang.String-) | Ajoute une chaîne au dernier intervalle de texte. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Ajoute une chaîne à la fin. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Ajoute une chaîne au début de la première plage de texte. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Ajoute une chaîne au début. |
| [clear()](#clear--) | Efface le contenu de cette instance. |
| [getAlignment()](#getAlignment--) | Obtient l'alignement. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient la date de dernière modification. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Obtient l'espacement des lignes. |
| [getParagraphStyle()](#getParagraphStyle--) | Obtient le style du paragraphe. |
| [getSpaceAfter()](#getSpaceAfter--) | Obtient la quantité minimale d'espace après. |
| [getSpaceBefore()](#getSpaceBefore--) | Obtient la quantité minimale d'espace avant. |
| [getStyles()](#getStyles--) | Obtient les styles. |
| [getTags()](#getTags--) | Obtient la liste de toutes les balises d'un paragraphe. |
| [getText()](#getText--) | Obtient le texte. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Renvoie l'index basé sur zéro de la première occurrence du caractère Unicode spécifié dans cette chaîne. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Renvoie l'index basé sur zéro de la première occurrence du caractère Unicode spécifié dans cette chaîne. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Renvoie l'index basé sur zéro de la première occurrence du caractère spécifié dans cette instance. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans cette instance. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans cette instance. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans cette instance. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Insère une chaîne spécifiée à une position d'index spécifiée dans cette instance. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Insère une chaîne spécifiée avec le style spécifié à une position d'index spécifiée dans cette instance. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Supprime tous les caractères de l'instance actuelle, en commençant à une position spécifiée et en continuant jusqu'à la dernière position. |
| [remove(int startIndex, int count)](#remove-int-int-) | Supprime le nombre spécifié de caractères dans l'instance actuelle en commençant à une position spécifiée. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Remplace toutes les occurrences d'un caractère Unicode spécifié dans cette instance par un autre caractère Unicode spécifié. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Remplace toutes les occurrences d'une chaîne spécifiée dans l'instance actuelle par une autre chaîne spécifiée. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Remplace toutes les occurrences d'une chaîne spécifiée dans l'instance actuelle par une autre chaîne spécifiée dans le style spécifié. |
| [setAlignment(int value)](#setAlignment-int-) | Définit l'alignement. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Définit la date de dernière modification. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Définit l'espacement des lignes. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Définit le style du paragraphe. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Définit la quantité minimale d'espace après. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Définit la quantité minimale d'espace avant. |
| [setText(String value)](#setText-java.lang.String-) | Définit le texte. |
| [trim()](#trim--) | Supprime tous les caractères d'espace blanc en début et en fin. |
| [trim(char trimChar)](#trim-char-) | Supprime toutes les occurrences d'un caractère en début et en fin. |
| [trim(char[] trimChars)](#trim-char...-) | Supprime toutes les occurrences en début et en fin d'un ensemble de caractères spécifié dans un tableau. |
| [trimEnd()](#trimEnd--) | Supprime tous les caractères d'espace blanc en fin. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Supprime toutes les occurrences d'un caractère en fin. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Supprime toutes les occurrences en fin d'un ensemble de caractères spécifié dans un tableau. |
| [trimStart()](#trimStart--) | Supprime tous les caractères d'espace blanc en début. |
| [trimStart(char trimChar)](#trimStart-char-) | Supprime toutes les occurrences d'un caractère spécifié en début. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Supprime toutes les occurrences en début d'un ensemble de caractères spécifié dans un tableau. |
### RichText() {#RichText--}
```
public RichText()
```


Initialise une nouvelle instance de la classe [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Ajoute une chaîne au dernier intervalle de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur ajoutée. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Ajoute une chaîne à la fin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur ajoutée. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Le style de la chaîne ajoutée. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Ajoute une chaîne au début de la première plage de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur ajoutée. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Ajoute une chaîne au début.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur ajoutée. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Le style de la chaîne ajoutée. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Efface le contenu de cette instance.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Obtient l'alignement.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient la date de dernière modification.

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


Obtient l'espacement des lignes.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Obtient le style du paragraphe. Ces paramètres sont utilisés s'il n'existe aucun objet TextStyle correspondant dans la collection [getStyles](../../com.aspose.note/richtext\#getStyles) ou si cet objet ne spécifie pas le paramètre requis.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Obtient la quantité minimale d'espace après.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Obtient la quantité minimale d'espace avant.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Obtient les styles.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Obtient la liste de toutes les balises d'un paragraphe.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Obtient le texte. La chaîne NE DOIT PAS contenir de caractères de valeur 10 (saut de ligne).

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


Renvoie l'index basé sur zéro de la première occurrence du caractère Unicode spécifié dans cette chaîne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char | La valeur. |

**Returns:**
int - Le `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Renvoie l'index basé sur zéro de la première occurrence du caractère Unicode spécifié dans cette chaîne. La recherche commence à une position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char | La valeur. |
| startIndex | int | La position de départ de la recherche |

**Returns:**
int - Le `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Renvoie l'index basé sur zéro de la première occurrence du caractère spécifié dans cette instance. La recherche commence à une position de caractère spécifiée et examine un nombre spécifié de positions de caractères.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char | La valeur. |
| startIndex | int | La position de départ de la recherche |
| count | int | Le nombre. |

**Returns:**
int - Le `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur. |

**Returns:**
int - Le `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans cette instance. La recherche commence à une position de caractère spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur. |
| startIndex | int | La position de départ de la recherche |

**Returns:**
int - Le `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans cette instance. La recherche commence à une position de caractère spécifiée et examine un nombre spécifié de positions de caractères.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur. |
| startIndex | int | La position de départ de la recherche |
| count | int | Le nombre. |

**Returns:**
int - Le `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur. |
| startIndex | int | La position de départ de la recherche |
| count | int | Le nombre. |
| comparisonType | short | Le type de recherche à utiliser pour la chaîne spécifiée |

**Returns:**
int - Le `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle. Un paramètre spécifie le type de recherche à utiliser pour la chaîne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur. |
| comparisonType | short | Le type de recherche à utiliser pour la chaîne spécifiée |

**Returns:**
int - Le `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Renvoie l'index basé sur zéro de la première occurrence de la chaîne spécifiée dans l'instance actuelle. Les paramètres spécifient la position de départ de la recherche dans la chaîne actuelle et le type de recherche à utiliser pour la chaîne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | La valeur. |
| startIndex | int | La position de départ de la recherche |
| comparisonType | short | Le type de recherche à utiliser pour la chaîne spécifiée |

**Returns:**
int - Le `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Insère une chaîne spécifiée à une position d'index spécifiée dans cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index de départ. |
| valeur | java.lang.String | La valeur. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Insère une chaîne spécifiée avec le style spécifié à une position d'index spécifiée dans cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index de départ. |
| valeur | java.lang.String | La valeur. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Le style. |

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


Supprime tous les caractères de l'instance actuelle, en commençant à une position spécifiée et en continuant jusqu'à la dernière position.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index de départ. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Supprime le nombre spécifié de caractères dans l'instance actuelle en commençant à une position spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index de départ. |
| count | int | Le nombre. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Remplace toutes les occurrences d'un caractère Unicode spécifié dans cette instance par un autre caractère Unicode spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldChar | char | L'ancien caractère. |
| newChar | char | Le nouveau caractère. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Remplace toutes les occurrences d'une chaîne spécifiée dans l'instance actuelle par une autre chaîne spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | L'ancienne valeur. |
| newValue | java.lang.String | La nouvelle valeur. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Remplace toutes les occurrences d'une chaîne spécifiée dans l'instance actuelle par une autre chaîne spécifiée dans le style spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldValue | java.lang.String | L'ancienne valeur. |
| newValue | java.lang.String | La nouvelle valeur. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Le style de la nouvelle valeur. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Définit l'alignement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Définit la date de dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Définit l'espacement des lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Définit le style du paragraphe. Ces paramètres sont utilisés s'il n'existe aucun objet TextStyle correspondant dans la collection [getStyles](../../com.aspose.note/richtext\#getStyles) ou si cet objet ne spécifie pas le paramètre requis.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Définit la quantité minimale d'espace après.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Définit la quantité minimale d'espace avant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Définit le texte. La chaîne NE DOIT PAS contenir de caractères de valeur 10 (saut de ligne).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Supprime tous les caractères d'espace blanc en début et en fin.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Supprime toutes les occurrences d'un caractère en début et en fin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| trimChar | char | Le caractère de coupe. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Supprime toutes les occurrences en début et en fin d'un ensemble de caractères spécifié dans un tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| trimChars | char[] | Les caractères de coupe. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Supprime tous les caractères d'espace blanc en fin.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Supprime toutes les occurrences d'un caractère en fin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| trimChar | char | Le caractère de coupe. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Supprime toutes les occurrences en fin d'un ensemble de caractères spécifié dans un tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| trimChars | char[] | Les caractères de coupe. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Supprime tous les caractères d'espace blanc en début.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Supprime toutes les occurrences d'un caractère spécifié en début.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| trimChar | char | Le caractère de coupe. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Supprime toutes les occurrences en début d'un ensemble de caractères spécifié dans un tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| trimChars | char[] | Les caractères de coupe. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
