---
title: "LoadOptions"
second_title: "Aspose.Note for Java API-referentie"
description: "Opties die worden gebruikt om een document te laden."
type: docs
weight: 46
url: /nl/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Opties die worden gebruikt om een document te laden.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initialiseert een nieuw exemplaar van de `LoadOptions`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Haalt een wachtwoord op of stelt een wachtwoord in voor de versleutelde documentinhoud. |
| [getLoadHistory()](#getLoadHistory--) | Haalt een waarde op of stelt een waarde in die aangeeft of een documentlader de geschiedenis moet negeren. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Haalt een wachtwoord op of stelt een wachtwoord in voor de versleutelde documentinhoud. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Haalt een waarde op of stelt een waarde in die aangeeft of een documentlader de geschiedenis moet negeren. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initialiseert een nieuw exemplaar van de `LoadOptions`-klasse.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Haalt een wachtwoord op of stelt een wachtwoord in voor de versleutelde documentinhoud. De waarde wordt genegeerd als het document niet met een wachtwoord is beveiligd.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Haalt een waarde op of stelt een waarde in die aangeeft of een documentlader de geschiedenis moet negeren. Gebruik deze optie om het geheugen- en CPU-gebruik te verminderen. Standaardwaarde is `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Haalt een wachtwoord op of stelt een wachtwoord in voor de versleutelde documentinhoud. De waarde wordt genegeerd als het document niet met een wachtwoord is beveiligd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Haalt een waarde op of stelt een waarde in die aangeeft of een documentlader de geschiedenis moet negeren. Gebruik deze optie om het geheugen- en CPU-gebruik te verminderen. Standaardwaarde is `true`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

