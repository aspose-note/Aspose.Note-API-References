---
title: "LoadOptions"
second_title: "Aspose.Note für Java API-Referenz"
description: "Optionen, die zum Laden eines Dokuments verwendet werden."
type: docs
weight: 46
url: /de/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Optionen, die zum Laden eines Dokuments verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initialisiert eine neue Instanz der `LoadOptions`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Liest oder setzt ein Passwort für den verschlüsselten Dokumentinhalt. |
| [getLoadHistory()](#getLoadHistory--) | Liest oder setzt einen Wert, der angibt, ob ein Dokumentenlader die Historie ignorieren soll. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Liest oder setzt ein Passwort für den verschlüsselten Dokumentinhalt. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Liest oder setzt einen Wert, der angibt, ob ein Dokumentenlader die Historie ignorieren soll. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialisiert eine neue Instanz der `LoadOptions`-Klasse.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Liest oder setzt ein Passwort für den verschlüsselten Dokumentinhalt. Der Wert wird ignoriert, falls das Dokument nicht passwortgeschützt ist.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Liest oder setzt einen Wert, der angibt, ob ein Dokumentenlader die Historie ignorieren soll. Verwenden Sie diese Option, um Speicher- und CPU‑Verbrauch zu reduzieren. Der Standardwert ist `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Liest oder setzt ein Passwort für den verschlüsselten Dokumentinhalt. Der Wert wird ignoriert, falls das Dokument nicht passwortgeschützt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Liest oder setzt einen Wert, der angibt, ob ein Dokumentenlader die Historie ignorieren soll. Verwenden Sie diese Option, um Speicher- und CPU‑Verbrauch zu reduzieren. Der Standardwert ist `true`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

