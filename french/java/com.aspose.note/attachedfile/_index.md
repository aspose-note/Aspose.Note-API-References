---
title: "AttachedFile"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un fichier joint."
type: docs
weight: 11
url: /fr/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Représente un fichier joint.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Initialise une nouvelle instance de la classe `AttachedFile`. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initialise une nouvelle instance de la classe `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Initialise une nouvelle instance de la classe `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initialise une nouvelle instance de la classe `AttachedFile`. |
| [AttachedFile()](#AttachedFile--) | Initialise une nouvelle instance de la classe `AttachedFile`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getAlignment()](#getAlignment--) | Obtient l'alignement. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Obtient ou définit le corps d'un texte alternatif pour l'icône du fichier joint. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Obtient ou définit le titre du texte alternatif pour l'icône du fichier joint. |
| [getBytes()](#getBytes--) | Obtient les données binaires d'un fichier intégré. |
| [getExtension()](#getExtension--) | Obtient l'extension d'un fichier intégré. |
| [getFileName()](#getFileName--) | Obtient le nom du fichier intégré. |
| [getFilePath()](#getFilePath--) | Obtient le chemin du fichier original. |
| [getHeight()](#getHeight--) | Obtient la hauteur originale de l'icône du fichier intégré. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Obtient le décalage horizontal. |
| [getIcon()](#getIcon--) | Obtient les données binaires de l'icône associée au fichier intégré. |
| [getIconExtension()](#getIconExtension--) | Obtient l'extension de l'icône. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient la date de dernière modification. |
| [getMaxHeight()](#getMaxHeight--) | Obtient la hauteur maximale pour afficher l'icône du fichier intégré. |
| [getMaxWidth()](#getMaxWidth--) | Obtient la largeur maximale pour afficher l'icône du fichier intégré. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Obtient les données concernant l'erreur survenue lors de l'accès au fichier. |
| [getTags()](#getTags--) | Obtient la liste des balises d'un fichier joint. |
| [getText()](#getText--) | Obtient la représentation textuelle du fichier intégré. |
| [getVerticalOffset()](#getVerticalOffset--) | Obtient le décalage vertical. |
| [getWidth()](#getWidth--) | Obtient la largeur originale de l'icône du fichier intégré. |
| [isPrintout()](#isPrintout--) | Obtient une valeur indiquant si la vue du fichier est une impression. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Obtient une valeur indiquant si la taille de l'icône a été explicitement mise à jour par l'utilisateur. |
| [setAlignment(int value)](#setAlignment-int-) | Définit l'alignement. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Obtient ou définit le corps d'un texte alternatif pour l'icône du fichier joint. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Obtient ou définit le titre du texte alternatif pour l'icône du fichier joint. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Définit le décalage horizontal. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Définit la date de dernière modification. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Définit la hauteur maximale pour afficher l'icône du fichier intégré. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Définit la largeur maximale pour afficher l'icône du fichier intégré. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Définit une valeur indiquant si la vue du fichier est une impression. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Définit une valeur indiquant si la taille de l'icône a été explicitement mise à jour par l'utilisateur. |
| [setText(String value)](#setText-java.lang.String-) | Définit la représentation textuelle du fichier intégré. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Définit le décalage vertical. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Initialise une nouvelle instance de la classe `AttachedFile`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | Une chaîne qui contient le chemin vers le fichier à partir duquel créer le `AttachedFile`. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initialise une nouvelle instance de la classe `AttachedFile`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | Une chaîne qui contient le chemin vers le fichier à partir duquel créer le `AttachedFile`. |
| icône | java.io.InputStream | Une icône pour le fichier joint. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Initialise une nouvelle instance de la classe `AttachedFile`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Un nom du fichier joint. |
| attachedFileStream | java.io.InputStream | Un flux qui contient les octets du fichier joint. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initialise une nouvelle instance de la classe `AttachedFile`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Un nom du fichier joint. |
| attachedFileStream | java.io.InputStream | Un flux qui contient les octets du fichier joint. |
| icône | java.io.InputStream | Une icône pour le fichier joint. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Un format de l'icône du fichier joint. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Initialise une nouvelle instance de la classe `AttachedFile`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Obtient l'alignement.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Obtient ou définit le corps d'un texte alternatif pour l'icône du fichier joint.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Obtient ou définit le titre du texte alternatif pour l'icône du fichier joint.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Obtient les données binaires d'un fichier intégré.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Obtient l'extension d'un fichier intégré.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Obtient le nom du fichier intégré.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Obtient le chemin du fichier original.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Obtient la hauteur originale de l'icône du fichier intégré.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Obtient le décalage horizontal.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Obtient les données binaires de l'icône associée au fichier intégré.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Obtient l'extension de l'icône.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient la date de dernière modification.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Obtient la hauteur maximale pour afficher l'icône du fichier intégré.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Obtient la largeur maximale pour afficher l'icône du fichier intégré.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Obtient les données concernant l'erreur survenue lors de l'accès au fichier.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Obtient la liste des balises d'un fichier joint.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Obtient la représentation textuelle du fichier incorporé. La chaîne NE DOIT PAS contenir de caractères de valeur 10 (saut de ligne) ou 13 (retour chariot).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Obtient le décalage vertical.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Obtient la largeur originale de l'icône du fichier intégré.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Obtient une valeur indiquant si la vue du fichier est une impression.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Obtient une valeur indiquant si la taille de l'icône a été explicitement mise à jour par l'utilisateur.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Définit l'alignement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | Valeur de l'alignement. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Obtient ou définit le corps d'un texte alternatif pour l'icône du fichier joint.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Obtient ou définit le titre du texte alternatif pour l'icône du fichier joint.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Définit le décalage horizontal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float | Valeur des décalages. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Définit la date de dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | Valeur de la date. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Définit la hauteur maximale pour afficher l'icône du fichier intégré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float | Valeur de la hauteur maximale. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Définit la largeur maximale pour afficher l'icône du fichier intégré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float | Valeur de la largeur maximale. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Définit une valeur indiquant si la vue du fichier est une impression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean | Nouvelle valeur. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Définit une valeur indiquant si la taille de l'icône a été explicitement mise à jour par l'utilisateur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean | Nouvelle valeur. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Définit la représentation textuelle du fichier incorporé. La chaîne NE DOIT PAS contenir de caractères de valeur 10 (saut de ligne) ou 13 (retour chariot).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | Valeur du texte. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Définit le décalage vertical.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float | Valeur du décalage. |

