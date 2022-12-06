---
title: License
second_title: Aspose.Note for Java API Reference
description: Provides methods to license the component.
type: docs
weight: 32
url: /java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Provides methods to license the component.
## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | Initializes a new instance of this class. |
## Methods

| Method | Description |
| --- | --- |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Licenses the component. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licenses the component. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Licenses the component. |
| [resetThreadContext()](#resetThreadContext--) | Resets a license context for curent thread. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Sets a license context for current thread. |
### License() {#License--}
```
public License()
```


Initializes a new instance of this class.

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Licenses the component.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | java.lang.String | Can be a full or short file name  or name of an embedded resource . Use an empty string to switch to evaluation mode.

--------------------



Tries to find the license in the following locations:

 

1. Explicit path.

 

2. The folder that contains the Aspose component assembly.

3. The folder that contains the client's calling assembly.

4. The folder that contains the entry (startup) assembly.

5. An embedded resource in the client's calling assembly.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Explicit path.

2. An embedded resource in the client's calling assembly.

 

2. The folder that contains the Aspose component JAR file.

3. The folder that contains the client's calling JAR file.

 |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licenses the component.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A stream that contains the license.

--------------------



Use this method to load a license from a stream.



 void setLicense(java.io.InputStream stream)  |

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Licenses the component.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseFile | java.io.File | File of license System.IO.FileInfo . |

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Resets a license context for curent thread.

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Sets a license context for current thread.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | A stream that contains the license. |

