---
title: "License"
second_title: "Aspose.Note for Java API-referens"
description: "Tillhandahåller metoder för att licensiera komponenten."
type: docs
weight: 44
url: /sv/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Tillhandahåller metoder för att licensiera komponenten.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [License()](#License--) | Initierar en ny instans av denna klass. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Återställer en licenskontext för aktuell tråd. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Licensierar komponenten. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licensierar komponenten. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Licensierar komponenten. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Anger en licenskontext för aktuell tråd. |
### License() {#License--}
```
public License()
```


Initierar en ny instans av denna klass.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Återställer en licenskontext för aktuell tråd.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Licensierar komponenten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| licenseFile | java.io.File | Fil för licens`System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licensierar komponenten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ström | java.io.InputStream | En ström som innehåller licensen. |

--------------------

`

Använd den här metoden för att läsa in en licens från en ström.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Licensierar komponenten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | licenseName | java.lang.String | Kan vara ett fullständigt eller kort filnamn` eller namnet på en inbäddad resurs`. Använd en tom sträng för att växla till evalueringsläge. |

--------------------

`

Försöker hitta licensen på följande platser:

` `

1. Explicit sökväg.

` `

2. Mappen som innehåller Aspose-komponentens assembly.

3. Mappen som innehåller klientens anropande assembly.

4. Mappen som innehåller entry (startup) assemblyn.

5. En inbäddad resurs i klientens anropande assembly.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Explicit sökväg.

2. En inbäddad resurs i klientens anropande assembly.

` `

2. Mappen som innehåller Aspose-komponentens JAR‑fil.

3. Mappen som innehåller klientens anropande JAR‑fil.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Anger en licenskontext för aktuell tråd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | En ström som innehåller licensen. |

