---
title: "NotebookLoadOptions"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός σημειωματάριου."
type: docs
weight: 58
url: /el/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός σημειωματάριου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης `NotebookLoadOptions`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα-παιδιά πρέπει να φορτωθούν ρητά αργότερα. |
| [getInstantLoading()](#getInstantLoading--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα-παιδιά πρέπει να φορτωθούν ενώ το γονικό έγγραφο φορτώνεται. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα-παιδιά πρέπει να φορτωθούν ρητά αργότερα. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα-παιδιά πρέπει να φορτωθούν ενώ το γονικό έγγραφο φορτώνεται. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `NotebookLoadOptions`.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα-παιδιά πρέπει να φορτωθούν ρητά αργότερα.

--------------------

Η προεπιλεγμένη τιμή είναι `false`, έτσι τα παιδικά έγγραφα θα φορτωθούν έμμεσα. Η τιμή `true` υποδεικνύει ότι ο χρήστης πρέπει να καλέσει `Notebook.loadChildDocument` ή για κάθε παιδικό κόμβο του σημειωματάριου μετά τη φόρτωση του ίδιου του σημειωματάριου. Εάν η τιμή είναι `true`, η επιλογή `NotebookLoadOptions.instantLoading` θα αγνοηθεί. Εάν το σημειωματάριο φορτώνεται από ροή, η τιμή είναι πάντα `true` παρόλο που ορίστηκε ρητά από τον χρήστη σε `false`.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα-παιδιά πρέπει να φορτωθούν ενώ το γονικό έγγραφο φορτώνεται.

--------------------

Η προεπιλεγμένη τιμή είναι `false`, έτσι τα παιδικά έγγραφα θα φορτωθούν «αργά», δηλαδή η φόρτωσή τους θα πρέπει να αναβληθεί μέχρι να γίνει άμεση πρόσβαση σε συγκεκριμένο παιδί. Η τιμή `true` υποδεικνύει ότι η φόρτωσή τους πρέπει να γίνει αμέσως.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα-παιδιά πρέπει να φορτωθούν ρητά αργότερα.

--------------------

Η προεπιλεγμένη τιμή είναι `false`, έτσι τα παιδικά έγγραφα θα φορτωθούν έμμεσα. Η τιμή `true` υποδεικνύει ότι ο χρήστης πρέπει να καλέσει `Notebook.loadChildDocument` ή για κάθε παιδικό κόμβο του σημειωματάριου μετά τη φόρτωση του ίδιου του σημειωματάριου. Εάν η τιμή είναι `true`, η επιλογή `NotebookLoadOptions.instantLoading` θα αγνοηθεί. Εάν το σημειωματάριο φορτώνεται από ροή, η τιμή είναι πάντα `true` παρόλο που ορίστηκε ρητά από τον χρήστη σε `false`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα-παιδιά πρέπει να φορτωθούν ενώ το γονικό έγγραφο φορτώνεται.

--------------------

Η προεπιλεγμένη τιμή είναι `false`, έτσι τα παιδικά έγγραφα θα φορτωθούν «αργά», δηλαδή η φόρτωσή τους θα πρέπει να αναβληθεί μέχρι να γίνει άμεση πρόσβαση σε συγκεκριμένο παιδί. Η τιμή `true` υποδεικνύει ότι η φόρτωσή τους πρέπει να γίνει αμέσως.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

