---
title: "ExtendedApsGlyphs"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά έναν περιτύλιγμα για τα τυπικά ApsGlyphs που επεκτείνει ορισμένη συμπεριφορά σχεδίασης."
type: docs
weight: 24
url: /el/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Αναπαριστά περιτύλιγμα για το τυπικό ApsGlyphs, το οποίο επεκτείνει κάποια από τη συμπεριφορά σχεδίασης.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedApsGlyphs`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Προσθέτει αυτόν τον κόμβο στο δοσμένο `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Εφαρμόζει μετασχηματισμό επιπέδου, μετακινώντας τον κόμβο στα επίπεδα x και y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Εφαρμόζει κλιμάκωση στα glyphs. |
| [getBottom()](#getBottom--) | Λαμβάνει το κάτω μέρος των glyphs. |
| [getCopy()](#getCopy--) | Λαμβάνει το αντίγραφο των glyphs. |
| [getOrigin()](#getOrigin--) | Λαμβάνει το αρχικό σημείο. |
| [getSize()](#getSize--) | Λαμβάνει το μέγεθος. |
| [getTop()](#getTop--) | Λαμβάνει το επάνω μέρος. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedApsGlyphs`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Ένα αρχικό σύμβολο aps. |

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


Εφαρμόζει κλιμάκωση στα glyphs.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| scaleTransform | float | Ο συντελεστής κλίμακας για τον μετασχηματισμό. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Λαμβάνει το κάτω μέρος των glyphs.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Λαμβάνει το αντίγραφο των glyphs.

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
