---
title: "Title"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un titre."
type: docs
weight: 95
url: /fr/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Représente un titre.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Title()](#Title--) | Initialise une nouvelle instance de la classe `Title`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Obtient tous les nœuds enfants par type de nœud. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | Obtient ou définit le décalage horizontal. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient ou définit l'heure de la dernière modification. |
| [getTitleDate()](#getTitleDate--) | Obtient ou définit une représentation sous forme de chaîne de la date dans le titre. |
| [getTitleText()](#getTitleText--) | Obtient ou définit le texte du titre. |
| [getTitleTime()](#getTitleTime--) | Obtient ou définit une représentation sous forme de chaîne de l'heure dans le titre. |
| [getVerticalOffset()](#getVerticalOffset--) | Obtient ou définit le décalage vertical. |
| [isComposite()](#isComposite--) | Obtient une valeur indiquant si ce nœud est composite. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt les nœuds enfants du [Title](../../com.aspose.note/title). |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Obtient ou définit le décalage horizontal. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtient ou définit l'heure de la dernière modification. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Obtient ou définit une représentation sous forme de chaîne de la date dans le titre. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Obtient ou définit le texte du titre. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Obtient ou définit une représentation sous forme de chaîne de l'heure dans le titre. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Obtient ou définit le décalage vertical. |
### Title() {#Title--}
```
public Title()
```


Initialise une nouvelle instance de la classe `Title`.

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Obtient tous les nœuds enfants par type de nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Une liste de nœuds enfants.

`T1`: Le type des éléments dans la liste retournée.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INNode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Obtient ou définit le décalage horizontal.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient ou définit l'heure de la dernière modification.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Obtient ou définit une représentation sous forme de chaîne de la date dans le titre.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Obtient ou définit le texte du titre.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Obtient ou définit une représentation sous forme de chaîne de l'heure dans le titre.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Obtient ou définit le décalage vertical.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Obtient une valeur indiquant si ce nœud est composite. Si vrai, le nœud peut avoir des nœuds enfants.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Renvoie un énumérateur qui parcourt les nœuds enfants du [Title](../../com.aspose.note/title).

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - L'énumérateur.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


Obtient ou définit le décalage horizontal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtient ou définit l'heure de la dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Obtient ou définit une représentation sous forme de chaîne de la date dans le titre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Obtient ou définit le texte du titre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Obtient ou définit une représentation sous forme de chaîne de l'heure dans le titre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Obtient ou définit le décalage vertical.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

