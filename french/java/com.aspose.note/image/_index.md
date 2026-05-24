---
title: "Image"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente une Image."
type: docs
weight: 33
url: /fr/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Représente une Image.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Initialise une nouvelle instance de la classe `Image`. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Initialise une nouvelle instance de la classe `Image`. |
| [Image()](#Image--) | Initialise une nouvelle instance de la classe `Image`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getAlignment()](#getAlignment--) | Obtient l'alignement. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Obtient le texte alternatif du corps pour l'image. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Obtient le titre du texte alternatif pour l'image. |
| [getBytes()](#getBytes--) | Obtient le magasin de données de l'image. |
| [getFileName()](#getFileName--) | Obtient le nom du fichier. |
| [getFilePath()](#getFilePath--) | Obtient le chemin du fichier image. |
| [getFormat()](#getFormat--) | Obtient le format de l'image. |
| [getHeight()](#getHeight--) | Obtient la hauteur. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Obtient le décalage horizontal. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Obtient le lien hypertexte associé à l'image. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient la date de dernière modification. |
| [getOriginalHeight()](#getOriginalHeight--) | Obtient la hauteur originale. |
| [getOriginalWidth()](#getOriginalWidth--) | Obtient la largeur originale. |
| [getTags()](#getTags--) | Obtient la liste de toutes les balises d'une image. |
| [getVerticalOffset()](#getVerticalOffset--) | Obtient le décalage vertical. |
| [getWidth()](#getWidth--) | Obtient la largeur. |
| [isBackground()](#isBackground--) | Obtient si l'image est une image d'arrière-plan. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Remplace les données d'image actuelles par les données de l'objet Image fourni. |
| [setAlignment(int value)](#setAlignment-int-) | Définit l'alignement. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Définit le texte alternatif du corps pour l'image. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Définit le titre du texte alternatif pour l'image. |
| [setBackground(boolean value)](#setBackground-boolean-) | Obtient si l'image est une image d'arrière-plan. |
| [setHeight(float value)](#setHeight-float-) | Définit la hauteur. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Définit le décalage horizontal. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Définit le lien hypertexte associé à l'image. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Définit la date de dernière modification. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Définit le décalage vertical. |
| [setWidth(float value)](#setWidth-float-) | Définit la largeur. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Initialise une nouvelle instance de la classe `Image`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | Une chaîne qui contient le chemin du fichier à partir duquel créer l'`Image`. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Initialise une nouvelle instance de la classe `Image`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Un nom de l'image. |
| imageStream | java.io.InputStream | Un flux qui contient l'image. |

### Image() {#Image--}
```
public Image()
```


Initialise une nouvelle instance de la classe `Image`.

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


Obtient le texte alternatif du corps pour l'image.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Obtient le titre du texte alternatif pour l'image.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Obtient le magasin de données de l'image.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Obtient le nom du fichier.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Obtient le chemin du fichier image.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Obtient le format de l'image.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Obtient la hauteur. C'est la vraie hauteur de l'image dans le document MS OneNote.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Obtient le décalage horizontal.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Obtient le lien hypertexte associé à l'image.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient la date de dernière modification.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Obtient la hauteur originale. C'est la largeur originale de l'image, avant le redimensionnement.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Obtient la largeur originale. C'est la largeur originale de l'image, avant le redimensionnement.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Obtient la liste de toutes les balises d'une image.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Obtient le décalage vertical.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Obtient la largeur. C'est la vraie largeur de l'image dans le document MS OneNote.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Obtient si l'image est une image d'arrière-plan.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Remplace les données d'image actuelles par les données de l'objet Image fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Définit l'alignement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Définit le texte alternatif du corps pour l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Définit le titre du texte alternatif pour l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Obtient si l'image est une image d'arrière-plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Définit la hauteur. C'est la vraie hauteur de l'image dans le document MS OneNote.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Définit le décalage horizontal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Définit le lien hypertexte associé à l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Définit la date de dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Définit le décalage vertical.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Définit la largeur. C'est la vraie largeur de l'image dans le document MS OneNote.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

