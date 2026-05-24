---
title: "ExtendedCompositeNode"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Συνδυάζει πολλές περιπτώσεις του IExtendedApsNode."
type: docs
weight: 29
url: /el/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Συνδυάζει αρκετές εμφανίσεις του `IExtendedApsNode`.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedCompositeNode`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Προσθέτει το `extendedApsNode` στην εσωτερική λίστα κόμβων. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Προσθέτει αυτόν τον κόμβο στο δοσμένο `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Εφαρμόζει μετασχηματισμό επιπέδου, μετακινώντας τον κόμβο στα επίπεδα x και y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Εφαρμόζει κλιμάκωση στον κόμβο. |
| [getApsNodes()](#getApsNodes--) | Αποκτά όλες τις περιπτώσεις του `IExtendedApsNode` που συνδυάζονται σε αυτό το `ExtendedCompositeNode`. |
| [getCopy()](#getCopy--) | Δημιουργεί ένα πλήρες αντίγραφο αυτού του κόμβου. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Προσθέτει το `extendedApsNode` στην εσωτερική λίστα κόμβων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Προσθέτει αυτόν τον κόμβο στο δοσμένο `compositeNode`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Εφαρμόζει μετασχηματισμό επιπέδου, μετακινώντας τον κόμβο στα επίπεδα x και y.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Εφαρμόζει κλιμάκωση στον κόμβο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| scaleTransform | float | Ο συντελεστής κλίμακας για τον μετασχηματισμό. |

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Αποκτά όλες τις περιπτώσεις του `IExtendedApsNode` που συνδυάζονται σε αυτό το `ExtendedCompositeNode`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Δημιουργεί ένα πλήρες αντίγραφο αυτού του κόμβου.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
