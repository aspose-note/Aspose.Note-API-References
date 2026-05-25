---
title: "License"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Fornisce metodi per licenziare il componente."
type: docs
weight: 44
url: /it/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Fornisce metodi per licenziare il componente.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [License()](#License--) | Inizializza una nuova istanza di questa classe. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Reimposta un contesto di licenza per il thread corrente. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Concede la licenza al componente. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Concede la licenza al componente. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Concede la licenza al componente. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Imposta un contesto di licenza per il thread corrente. |
### License() {#License--}
```
public License()
```


Inizializza una nuova istanza di questa classe.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Reimposta un contesto di licenza per il thread corrente.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Concede la licenza al componente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| licenseFile | java.io.File | File di licenza`System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Concede la licenza al componente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | flusso | java.io.InputStream | Uno stream che contiene la licenza. |

--------------------

`

Utilizza questo metodo per caricare una licenza da uno stream.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Concede la licenza al componente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | licenseName | java.lang.String | Può essere un nome file completo o abbreviato` o nome di una risorsa incorporata`. Usa una stringa vuota per passare alla modalità di valutazione. |

--------------------

`

Cerca di trovare la licenza nei seguenti percorsi:

` `

1. Percorso esplicito.

` `

2. La cartella che contiene l'assembly del componente Aspose.

3. La cartella che contiene l'assembly chiamante del client.

4. La cartella che contiene l'assembly di ingresso (avvio).

5. Una risorsa incorporata nell'assembly chiamante del client.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Percorso esplicito.

2. Una risorsa incorporata nell'assembly chiamante del client.

` `

2. La cartella che contiene il file JAR del componente Aspose.

3. La cartella che contiene il file JAR chiamante del client.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Imposta un contesto di licenza per il thread corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Uno stream che contiene la licenza. |

