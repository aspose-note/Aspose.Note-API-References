---
title: "ExtendedApsPage"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αντιπροσωπεύει ένα wrapper για τα τυπικά ApsGlyphs που επεκτείνει ορισμένη συμπεριφορά σχεδίασης."
type: docs
weight: 27
url: /el/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Αναπαριστά ένα περιτύλιγμα για το τυπικό ApsGlyphs, το οποίο επεκτείνει κάποια από τη συμπεριφορά σχεδίασης.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedApsPage`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getContentSize()](#getContentSize--) | Λαμβάνει το μέγεθος της σελίδας χωρίς τα περιθώρια. |
| [getMargin()](#getMargin--) | Λαμβάνει το περιθώριο αυτής της σελίδας. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Λαμβάνει τη θέση του τέλους της σελίδας, στη σελίδα MS OneNote, όταν μια σελίδα MS OneNote διαιρείται σε πολλές σελίδες aps. |
| [getPageSize()](#getPageSize--) | Λαμβάνει το τελικό μέγεθος της σελίδας. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Λαμβάνει τη θέση της αρχής της σελίδας στη σελίδα MS OneNote, όταν μια σελίδα MS OneNote διαιρείται σε πολλές σελίδες aps. |
| [iterator()](#iterator--) | Επιστρέφει τον enumerator που διατρέχει όλους τους κόμβους από αυτή τη σελίδα. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | Ο enumerator λήψης. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `ExtendedApsPage`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | Το μέγεθος της σελίδας. |
| pageStartInNotePage | float | Η αρχή της σελίδας στην αρχική σελίδα MS OneNote. |
| margin | com.aspose.foundation.layout.Margin | Το εκτεταμένο περιθώριο σελίδας. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Λαμβάνει το μέγεθος της σελίδας χωρίς τα περιθώρια.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Λαμβάνει το περιθώριο αυτής της σελίδας.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Λαμβάνει τη θέση του τέλους της σελίδας, στη σελίδα MS OneNote, όταν μια σελίδα MS OneNote διαιρείται σε πολλές σελίδες aps.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Λαμβάνει το τελικό μέγεθος της σελίδας.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Λαμβάνει τη θέση της αρχής της σελίδας στη σελίδα MS OneNote, όταν μια σελίδα MS OneNote διαιρείται σε πολλές σελίδες aps.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Επιστρέφει τον enumerator που διατρέχει όλους τους κόμβους από αυτή τη σελίδα.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - Το `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


Ο enumerator λήψης.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - Το `IEnumerator`.
