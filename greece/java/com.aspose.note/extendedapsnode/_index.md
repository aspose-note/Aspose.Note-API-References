---
title: "ExtendedApsNode"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αντιπροσωπεύει το περιτύλιγμα για ένα τυπικό ApsNode που επεκτείνει ορισμένη συμπεριφορά σχεδίασης."
type: docs
weight: 26
url: /el/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Αναπαριστά περιτύλιγμα για ένα τυπικό ApsNode, το οποίο επεκτείνει κάποια από τη συμπεριφορά σχεδίασης.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Προσθέτει αυτόν τον κόμβο στο δοσμένο `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Εφαρμόζει μετασχηματισμό επιπέδου, μετακινώντας τον κόμβο στα επίπεδα x και y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Εφαρμόζει κλιμάκωση στον κόμβο. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Λαμβάνει ή ορίζει τη συντεταγμένη y του κάτω μέρους του κόμβου. |
| [getCopy()](#getCopy--) | Δημιουργεί ένα πλήρες αντίγραφο αυτού του κόμβου. |
| [getOrigin()](#getOrigin--) | Λαμβάνει ή ορίζει την προέλευση του κόμβου. |
| [getSize()](#getSize--) | Λαμβάνει ή ορίζει το μέγεθος του κόμβου. |
| [getTop()](#getTop--) | Λαμβάνει ή ορίζει τη συντεταγμένη y της κορυφής του κόμβου. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Προσθέτει αυτόν τον κόμβο στο δοσμένο `compositeNode`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Εφαρμόζει μετασχηματισμό επιπέδου, μετακινώντας τον κόμβο στα επίπεδα x και y.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Εφαρμόζει κλιμάκωση στον κόμβο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| scaleTransform | float | Ο συντελεστής κλίμακας για τον μετασχηματισμό. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Λαμβάνει ή ορίζει τη συντεταγμένη y του κάτω μέρους του κόμβου.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Δημιουργεί ένα πλήρες αντίγραφο αυτού του κόμβου.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Λαμβάνει ή ορίζει την προέλευση του κόμβου.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Λαμβάνει ή ορίζει το μέγεθος του κόμβου.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Λαμβάνει ή ορίζει τη συντεταγμένη y της κορυφής του κόμβου.

**Returns:**
float
