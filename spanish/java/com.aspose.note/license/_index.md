---
title: "License"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Proporciona métodos para licenciar el componente."
type: docs
weight: 44
url: /es/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Proporciona métodos para licenciar el componente.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [License()](#License--) | Inicializa una nueva instancia de esta clase. |
## Métodos

| Método | Descripción |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Restablece el contexto de licencia para el hilo actual. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Licencia el componente. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licencia el componente. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Licencia el componente. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Establece un contexto de licencia para el hilo actual. |
### License() {#License--}
```
public License()
```


Inicializa una nueva instancia de esta clase.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Restablece el contexto de licencia para el hilo actual.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Licencia el componente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| licenseFile | java.io.File | Archivo de licencia `System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licencia el componente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | flujo | java.io.InputStream | Un flujo que contiene la licencia. |

--------------------

`

Utilice este método para cargar una licencia desde un flujo.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Licencia el componente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | licenseName | java.lang.String | Puede ser un nombre de archivo completo o corto` o el nombre de un recurso incrustado`. Use una cadena vacía para cambiar al modo de evaluación. |

--------------------

`

Intenta encontrar la licencia en las siguientes ubicaciones:

` `

1. Ruta explícita.

` `

2. La carpeta que contiene el ensamblado del componente Aspose.

3. La carpeta que contiene el ensamblado de llamada del cliente.

4. La carpeta que contiene el ensamblado de entrada (inicio).

5. Un recurso incrustado en el ensamblado de llamada del cliente.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Ruta explícita.

2. Un recurso incrustado en el ensamblado de llamada del cliente.

` `

2. La carpeta que contiene el archivo JAR del componente Aspose.

3. La carpeta que contiene el archivo JAR de llamada del cliente.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Establece un contexto de licencia para el hilo actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | Un flujo que contiene la licencia. |

