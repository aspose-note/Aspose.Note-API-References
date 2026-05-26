---
title: "LoadOptions"
second_title: "Aspose.Note for Java API-referens"
description: "Alternativ som används för att läsa in ett dokument."
type: docs
weight: 46
url: /sv/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Alternativ som används för att läsa in ett dokument.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initierar en ny instans av klassen `LoadOptions`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Hämtar eller anger ett lösenord för det krypterade dokumentinnehållet. |
| [getLoadHistory()](#getLoadHistory--) | Hämtar eller anger ett värde som indikerar om en dokumentläsare ska ignorera historiken. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Hämtar eller anger ett lösenord för det krypterade dokumentinnehållet. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Hämtar eller anger ett värde som indikerar om en dokumentläsare ska ignorera historiken. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initierar en ny instans av klassen `LoadOptions`.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Hämtar eller anger ett lösenord för det krypterade dokumentinnehållet. Värdet ignoreras om dokumentet inte är lösenordsskyddat.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Hämtar eller anger ett värde som indikerar om en dokumentläsare ska ignorera historiken. Använd detta alternativ för att minska minne- och CPU-användning. Standardvärdet är `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Hämtar eller anger ett lösenord för det krypterade dokumentinnehållet. Värdet ignoreras om dokumentet inte är lösenordsskyddat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Hämtar eller anger ett värde som indikerar om en dokumentläsare ska ignorera historiken. Använd detta alternativ för att minska minne- och CPU-användning. Standardvärdet är `true`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

