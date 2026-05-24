---
title: "ExtendedApsImage"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αντιπροσωπεύει ένα wrapper για το τυπικό ApsImage που επεκτείνει κάποια από τη συμπεριφορά σχεδίασης."
type: docs
weight: 25
url: /el/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Αναπαριστά ένα περιτύλιγμα για το τυπικό ApsImage, το οποίο επεκτείνει κάποια από τη συμπεριφορά σχεδίασης.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedApsImage`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Προσθέτει αυτόν τον κόμβο στο δοσμένο `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Εφαρμόζει μετασχηματισμό επιπέδου, μετακινώντας τον κόμβο στα επίπεδα x και y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Εφαρμόζει κλιμάκωση στην εικόνα. |
| [getBottom()](#getBottom--) | Λαμβάνει το κάτω μέρος. |
| [getCopy()](#getCopy--) | Δημιουργεί ένα πλήρες αντίγραφο αυτού του κόμβου. |
| [getOrigin()](#getOrigin--) | Λαμβάνει το αρχικό σημείο. |
| [getSize()](#getSize--) | Λαμβάνει το μέγεθος. |
| [getTop()](#getTop--) | Λαμβάνει το επάνω μέρος. |
| [isBackground()](#isBackground--) | Λαμβάνει εάν η εικόνα είναι εικόνα φόντου. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedApsImage`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | Η εικόνα. |

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


Εφαρμόζει κλιμάκωση στην εικόνα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| scaleTransform | float | Ο συντελεστής κλίμακας για τον μετασχηματισμό. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Λαμβάνει το κάτω μέρος.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Δημιουργεί ένα πλήρες αντίγραφο αυτού του κόμβου.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Λαμβάνει το αρχικό σημείο.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Λαμβάνει το μέγεθος.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Λαμβάνει το επάνω μέρος.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Λαμβάνει εάν η εικόνα είναι εικόνα φόντου.

**Returns:**
boolean
