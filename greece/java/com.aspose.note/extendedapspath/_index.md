---
title: "ExtendedApsPath"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αντιπροσωπεύει ένα wrapper για το τυπικό ApsPath, το οποίο επεκτείνει ορισμένη συμπεριφορά σχεδίασης."
type: docs
weight: 28
url: /el/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Αναπαριστά ένα περιτύλιγμα για το τυπικό ApsPath, το οποίο επεκτείνει κάποια από τη συμπεριφορά σχεδίασης.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedApsPath`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Προσθέτει αυτόν τον κόμβο στο δοσμένο `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Εφαρμόζει μετασχηματισμό επιπέδου, μετακινώντας τον κόμβο στα επίπεδα x και y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Εφαρμόζει κλιμάκωση στον κόμβο. |
| [getBottom()](#getBottom--) | Λαμβάνει το κάτω μέρος. |
| [getCopy()](#getCopy--) | Δημιουργεί ένα πλήρες αντίγραφο αυτού του κόμβου. |
| [getTop()](#getTop--) | Λαμβάνει το επάνω μέρος. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedApsPath`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Η διαδρομή aps. |

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
### getTop() {#getTop--}
```
public float getTop()
```


Λαμβάνει το επάνω μέρος.

**Returns:**
float
