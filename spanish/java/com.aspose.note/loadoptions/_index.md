---
title: "LoadOptions"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Opciones usadas para cargar un documento."
type: docs
weight: 46
url: /es/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Opciones usadas para cargar un documento.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Inicializa una nueva instancia de la clase `LoadOptions`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Obtiene o establece una contraseña para el contenido del documento cifrado. |
| [getLoadHistory()](#getLoadHistory--) | Obtiene o establece un valor que indica si el cargador de documentos debe ignorar el historial. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Obtiene o establece una contraseña para el contenido del documento cifrado. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Obtiene o establece un valor que indica si el cargador de documentos debe ignorar el historial. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Inicializa una nueva instancia de la clase `LoadOptions`.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Obtiene o establece una contraseña para el contenido del documento cifrado. El valor se ignora en caso de que el documento no esté protegido con contraseña.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Obtiene o establece un valor que indica si el cargador de documentos debe ignorar el historial. Utilice esta opción para reducir el uso de memoria y CPU. El valor predeterminado es `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Obtiene o establece una contraseña para el contenido del documento cifrado. El valor se ignora en caso de que el documento no esté protegido con contraseña.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Obtiene o establece un valor que indica si el cargador de documentos debe ignorar el historial. Utilice esta opción para reducir el uso de memoria y CPU. El valor predeterminado es `true`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

