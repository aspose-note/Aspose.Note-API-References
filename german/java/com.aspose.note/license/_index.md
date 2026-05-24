---
title: "License"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt Methoden zur Lizenzierung der Komponente bereit."
type: docs
weight: 44
url: /de/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Stellt Methoden zur Lizenzierung der Komponente bereit.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [License()](#License--) | Initialisiert eine neue Instanz dieser Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Setzt den Lizenzkontext für den aktuellen Thread zurück. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Lizenziert die Komponente. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Lizenziert die Komponente. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Lizenziert die Komponente. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Setzt einen Lizenzkontext für den aktuellen Thread. |
### License() {#License--}
```
public License()
```


Initialisiert eine neue Instanz dieser Klasse.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Setzt den Lizenzkontext für den aktuellen Thread zurück.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Lizenziert die Komponente.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| licenseFile | java.io.File | Datei der Lizenz`System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Lizenziert die Komponente.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Datenstrom | java.io.InputStream | Ein Stream, der die Lizenz enthält. |

--------------------

`

Verwenden Sie diese Methode, um eine Lizenz aus einem Stream zu laden.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Lizenziert die Komponente.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | licenseName | java.lang.String | Kann ein voller oder kurzer Dateiname` oder Name einer eingebetteten Ressource` sein. Verwenden Sie eine leere Zeichenkette, um in den Evaluierungsmodus zu wechseln. |

--------------------

`

Versucht, die Lizenz an den folgenden Orten zu finden:

` `

1. Expliziter Pfad.

` `

2. Der Ordner, der die Aspose component assembly enthält.

3. Der Ordner, der die Aufruf‑Assembly des Clients enthält.

4. Der Ordner, der die Entry‑(Startup‑)Assembly enthält.

5. Eine eingebettete Ressource in der Aufruf‑Assembly des Clients.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Expliziter Pfad.

2. Eine eingebettete Ressource in der Aufruf‑Assembly des Clients.

` `

2. Der Ordner, der die Aspose component JAR‑Datei enthält.

3. Der Ordner, der die Aufruf‑JAR‑Datei des Clients enthält.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Setzt einen Lizenzkontext für den aktuellen Thread.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datenstrom | java.io.InputStream | Ein Stream, der die Lizenz enthält. |

