---
title: "License"
second_title: "Aspose.Note for Java API-referentie"
description: "Biedt methoden om de component te licentiëren."
type: docs
weight: 44
url: /nl/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Biedt methoden om de component te licentiëren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [License()](#License--) | Initialiseert een nieuw exemplaar van deze klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Reset een licentiecontext voor de huidige thread. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Licentieert het component. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licentieert het component. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Licentieert het component. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Stelt een licentiecontext in voor de huidige thread. |
### License() {#License--}
```
public License()
```


Initialiseert een nieuw exemplaar van deze klasse.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Reset een licentiecontext voor de huidige thread.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Licentieert het component.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| licenseFile | java.io.File | Bestand van licentie`System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licentieert het component.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stroom | java.io.InputStream | Een stroom die de licentie bevat. |

--------------------

`

Gebruik deze methode om een licentie te laden vanaf een stream.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Licentieert het component.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | licenseName | java.lang.String | Kan een volledige of korte bestandsnaam` of de naam van een ingebedde resource` zijn. Gebruik een lege tekenreeks om over te schakelen naar evaluatiemodus. |

--------------------

`

Probeert de licentie te vinden op de volgende locaties:

` `

1. Expliciet pad.

` `

2. De map die de Aspose componentassembly bevat.

3. De map die de aanroepende assembly van de client bevat.

4. De map die de entry (startup) assembly bevat.

5. Een ingebedde resource in de aanroepende assembly van de client.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Expliciet pad.

2. Een ingebedde resource in de aanroepende assembly van de client.

` `

2. De map die het Aspose component JAR‑bestand bevat.

3. De map die het JAR‑bestand van de client bevat.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Stelt een licentiecontext in voor de huidige thread.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | java.io.InputStream | Een stroom die de licentie bevat. |

