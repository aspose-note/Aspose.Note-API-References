---
title: "Page"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente une page."
type: docs
weight: 69
url: /fr/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Représente une page.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Page()](#Page--) | Initialise une nouvelle instance de la classe `Page`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [deepClone()](#deepClone--) | Clone la page. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Clone la page. |
| [getAuthor()](#getAuthor--) | Obtient ou définit l'auteur. |
| [getBackgroundColor()](#getBackgroundColor--) | Obtient ou définit la couleur d'arrière-plan de la page. |
| [getCreationTime()](#getCreationTime--) | Obtient ou définit l'heure de création. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient ou définit l'heure de la dernière modification. |
| [getLevel()](#getLevel--) | Obtient ou définit le niveau. |
| [getMargin()](#getMargin--) | Obtient ou définit la marge. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Obtient ou définit le résumé de révision pour la page et ses nœuds enfants. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Obtient la taille de mise en page de la page affichée dans l'éditeur. |
| [getSizeType()](#getSizeType--) | Obtient ou définit le type de taille d'une page. |
| [getTitle()](#getTitle--) | Obtient ou définit le titre. |
| [isConflictPage()](#isConflictPage--) | Obtient ou définit une valeur indiquant si cette page est une page de conflit. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Obtient ou définit l'auteur. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Obtient ou définit la couleur d'arrière-plan de la page. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Obtient ou définit une valeur indiquant si cette page est une page de conflit. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Obtient ou définit l'heure de création. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtient ou définit l'heure de la dernière modification. |
| [setLevel(byte value)](#setLevel-byte-) | Obtient ou définit le niveau. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Obtient ou définit la marge. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Obtient ou définit le résumé de révision pour la page et ses nœuds enfants. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Définit la taille de mise en page de la page affichée dans l'éditeur. |
| [setSizeType(int value)](#setSizeType-int-) | Obtient ou définit le type de taille d'une page. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Obtient ou définit le titre. |
### Page() {#Page--}
```
public Page()
```


Initialise une nouvelle instance de la classe `Page`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Clone la page.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Clone la page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cloneHistory | boolean | Spécifie si l'historique de la page doit être cloné.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtient ou définit l'auteur.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Obtient ou définit la couleur d'arrière-plan de la page.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Obtient ou définit l'heure de création.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient ou définit l'heure de la dernière modification.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Obtient ou définit le niveau.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Obtient ou définit la marge.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Obtient ou définit le résumé de révision pour la page et ses nœuds enfants.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Obtient la taille de mise en page de la page affichée dans l'éditeur.

--------------------

Cette valeur est utilisée par l'application Microsoft OneNote pour afficher la mise en page sous-jacente de la page lorsque le document est ouvert. Elle n'affecte pas l'impression ni l'enregistrement du document de toute façon. Lorsque la propriété Page.SizeType est définie sur PageSizeType.SizeByContent, cette propriété renvoie la taille réelle du contenu.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Obtient ou définit le type de taille d'une page.

--------------------

Par défaut, une page est redimensionnée automatiquement. La valeur par défaut est [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Obtient ou définit le titre.

Valeur : le `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Obtient ou définit une valeur indiquant si cette page est une page de conflit.

--------------------

La page de conflit apparaît lorsque deux utilisateurs tentent de mettre à jour le même contenu. Dans ce cas, les modifications du premier utilisateur sont enregistrées comme d'habitude. Mais les modifications de l'autre utilisateur ne peuvent pas être fusionnées. Ainsi, une simple copie de la page est créée et marquée comme conflit.

Dans cette version, les conflits sont résolus en faveur des modifications du premier utilisateur. Ainsi, si le document comporte des pages de conflit, elles seront affichées dans l'historique mais seront ignorées lors de l'enregistrement. Il est possible de réinitialiser ce drapeau pour enregistrer ces pages dans l'historique comme des pages normales.

Un exemple détaillé de manipulation de page de conflit est disponible dans la documentation en ligne.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Obtient ou définit l'auteur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Obtient ou définit la couleur d'arrière-plan de la page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Obtient ou définit une valeur indiquant si cette page est une page de conflit.

--------------------

La page de conflit apparaît lorsque deux utilisateurs tentent de mettre à jour le même contenu. Dans ce cas, les modifications du premier utilisateur sont enregistrées comme d'habitude. Mais les modifications de l'autre utilisateur ne peuvent pas être fusionnées. Ainsi, une simple copie de la page est créée et marquée comme conflit.

Dans cette version, les conflits sont résolus en faveur des modifications du premier utilisateur. Ainsi, si le document comporte des pages de conflit, elles seront affichées dans l'historique mais seront ignorées lors de l'enregistrement. Il est possible de réinitialiser ce drapeau pour enregistrer ces pages dans l'historique comme des pages normales.

Un exemple détaillé de manipulation de page de conflit est disponible dans la documentation en ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Obtient ou définit l'heure de création.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtient ou définit l'heure de la dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Obtient ou définit le niveau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Obtient ou définit la marge.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Obtient ou définit le résumé de révision pour la page et ses nœuds enfants.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Définit la taille de mise en page de la page affichée dans l'éditeur.

--------------------

Cette valeur est utilisée par l'application Microsoft OneNote pour afficher la mise en page sous-jacente de la page lorsque le document est ouvert. Elle n'affecte pas l'impression ni l'enregistrement du document de toute façon. Lorsque la propriété Page.SizeType est définie sur PageSizeType.SizeByContent, cette propriété renvoie la taille réelle du contenu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Obtient ou définit le type de taille d'une page.

--------------------

Par défaut, une page est redimensionnée automatiquement. La valeur par défaut est [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Obtient ou définit le titre.

Valeur : le `Title`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

