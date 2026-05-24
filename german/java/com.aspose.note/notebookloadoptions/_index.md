---
title: "NotebookLoadOptions"
second_title: "Aspose.Note für Java API-Referenz"
description: "Optionen, die zum Laden eines Notizbuchs verwendet werden."
type: docs
weight: 58
url: /de/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Optionen, die zum Laden eines Notizbuchs verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Initialisiert eine neue Instanz der `NotebookLoadOptions`‑Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob Kinddokumente später explizit geladen werden sollen. |
| [getInstantLoading()](#getInstantLoading--) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob Kinddokumente geladen werden sollen, während das übergeordnete Dokument geladen wird. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob Kinddokumente später explizit geladen werden sollen. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Ruft einen Wert ab oder legt ihn fest, der angibt, ob Kinddokumente geladen werden sollen, während das übergeordnete Dokument geladen wird. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Initialisiert eine neue Instanz der `NotebookLoadOptions`‑Klasse.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Ruft einen Wert ab oder legt ihn fest, der angibt, ob Kinddokumente später explizit geladen werden sollen.

--------------------

Standardwert ist `false`, sodass untergeordnete Dokumente implizit geladen werden. Der Wert `true` bedeutet, dass der Benutzer `Notebook.loadChildDocument` aufrufen sollte oder für jeden Kindknoten des Notizbuchs, nachdem das Notizbuch selbst geladen wurde. Wenn der Wert `true` ist, wird die Option `NotebookLoadOptions.instantLoading` ignoriert. Wird das Notizbuch aus einem Stream geladen, ist der Wert immer `true`, obwohl er vom Benutzer explizit auf `false` gesetzt wurde.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Ruft einen Wert ab oder legt ihn fest, der angibt, ob Kinddokumente geladen werden sollen, während das übergeordnete Dokument geladen wird.

--------------------

Standardwert ist `false`, sodass untergeordnete Dokumente "lazy" geladen werden, d. h. ihr Laden sollte bis zu einem direkten Zugriff auf das jeweilige Kind verschoben werden. Der Wert `true` bedeutet, dass ihr Laden sofort erfolgen soll.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Ruft einen Wert ab oder legt ihn fest, der angibt, ob Kinddokumente später explizit geladen werden sollen.

--------------------

Standardwert ist `false`, sodass untergeordnete Dokumente implizit geladen werden. Der Wert `true` bedeutet, dass der Benutzer `Notebook.loadChildDocument` aufrufen sollte oder für jeden Kindknoten des Notizbuchs, nachdem das Notizbuch selbst geladen wurde. Wenn der Wert `true` ist, wird die Option `NotebookLoadOptions.instantLoading` ignoriert. Wird das Notizbuch aus einem Stream geladen, ist der Wert immer `true`, obwohl er vom Benutzer explizit auf `false` gesetzt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Ruft einen Wert ab oder legt ihn fest, der angibt, ob Kinddokumente geladen werden sollen, während das übergeordnete Dokument geladen wird.

--------------------

Standardwert ist `false`, sodass untergeordnete Dokumente "lazy" geladen werden, d. h. ihr Laden sollte bis zu einem direkten Zugriff auf das jeweilige Kind verschoben werden. Der Wert `true` bedeutet, dass ihr Laden sofort erfolgen soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

