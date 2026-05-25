---
title: "ExtendedApsPage"
second_title: "Aspose.Note for Java API Reference"
description: "मानक ApsGlyphs के लिए एक रैपर का प्रतिनिधित्व करता है जो ड्रॉइंग व्यवहार के कुछ हिस्सों का विस्तार करता है।"
type: docs
weight: 27
url: /hi/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Represents a wrapper for the standard ApsGlyphs, which extends some of the drawing behavior.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | `ExtendedApsPage` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [getContentSize()](#getContentSize--) | मार्जिन को छोड़कर पृष्ठ का आकार प्राप्त करता है। |
| [getMargin()](#getMargin--) | इस पृष्ठ का मार्जिन प्राप्त करता है। |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | जब एक MS OneNote पृष्ठ को कई aps पृष्ठों में विभाजित किया जाता है, तब MS OneNote पृष्ठ में पृष्ठ के अंत की स्थिति प्राप्त करता है। |
| [getPageSize()](#getPageSize--) | अंतिम पृष्ठ का आकार प्राप्त करता है। |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | जब एक MS OneNote पृष्ठ को कई aps पृष्ठों में विभाजित किया जाता है, तब MS OneNote पृष्ठ में पृष्ठ की शुरुआत की स्थिति प्राप्त करता है। |
| [iterator()](#iterator--) | इस पृष्ठ के सभी नोड्स के माध्यम से इटररेट करने वाले एनेमरेटर को लौटाता है। |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | एनेमरेटर प्राप्त करें। |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


`ExtendedApsPage` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | पृष्ठ का आकार। |
| pageStartInNotePage | float | मूल MS OneNote पृष्ठ में पृष्ठ की शुरुआत। |
| margin | com.aspose.foundation.layout.Margin | The extended page margin. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


मार्जिन को छोड़कर पृष्ठ का आकार प्राप्त करता है।

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


इस पृष्ठ का मार्जिन प्राप्त करता है।

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


जब एक MS OneNote पृष्ठ को कई aps पृष्ठों में विभाजित किया जाता है, तब MS OneNote पृष्ठ में पृष्ठ के अंत की स्थिति प्राप्त करता है।

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


अंतिम पृष्ठ का आकार प्राप्त करता है।

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


जब एक MS OneNote पृष्ठ को कई aps पृष्ठों में विभाजित किया जाता है, तब MS OneNote पृष्ठ में पृष्ठ की शुरुआत की स्थिति प्राप्त करता है।

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


इस पृष्ठ के सभी नोड्स के माध्यम से इटररेट करने वाले एनेमरेटर को लौटाता है।

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - The `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


एनेमरेटर प्राप्त करें।

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - The `IEnumerator`.
