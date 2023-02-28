---
title: Document.Document
second_title: Aspose.Note para la referencia de la API de .NET
description: Document constructor. Inicializa una nueva instancia delDocument class. Crea un documento de OneNote en blanco.
type: docs
weight: 10
url: /es/net/aspose.note/document/document/
---
## Document() {#constructor}

Inicializa una nueva instancia del[`Document`](../) class. Crea un documento de OneNote en blanco.

```csharp
public Document()
```

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Inicializa una nueva instancia del[`Document`](../) class. Abre un documento de OneNote existente desde un archivo.

```csharp
public Document(string filePath)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | El formato del documento no se reconoce o no es compatible. |
| [FileCorruptedException](../../filecorruptedexception/) | El documento parece estar dañado y no se puede cargar. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | El documento está encriptado y requiere una contraseña para abrirlo, pero proporcionó una contraseña incorrecta. |
| InvalidOperationException | Hay un problema con el documento y debe informarse a los desarrolladores de Aspose.Note. |
| IOException | Hay una excepción de entrada/salida. |

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Inicializa una nueva instancia del[`Document`](../)class. Abre un documento de OneNote existente desde un archivo. Permite especificar opciones adicionales como una contraseña de cifrado.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |
| loadOptions | LoadOptions | Opciones utilizadas para cargar un documento. Puede ser nulo. |

### Excepciones

| excepción | condición |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | El formato del documento no se reconoce o no es compatible. |
| [FileCorruptedException](../../filecorruptedexception/) | El documento parece estar dañado y no se puede cargar. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | El documento está encriptado y requiere una contraseña para abrirlo, pero proporcionó una contraseña incorrecta. |
| InvalidOperationException | Hay un problema con el documento y debe informarse a los desarrolladores de Aspose.Note. |
| IOException | Hay una excepción de entrada/salida. |

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Inicializa una nueva instancia del[`Document`](../) class. Abre un documento de OneNote existente desde una secuencia.

```csharp
public Document(Stream inStream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| inStream | Stream | El arroyo. |

### Excepciones

| excepción | condición |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | El formato del documento no se reconoce o no es compatible. |
| [FileCorruptedException](../../filecorruptedexception/) | El documento parece estar dañado y no se puede cargar. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | El documento está encriptado y requiere una contraseña para abrirlo, pero proporcionó una contraseña incorrecta. |
| InvalidOperationException | Hay un problema con el documento y debe informarse a los desarrolladores de Aspose.Note. |
| IOException | Hay una excepción de entrada/salida. |
| ArgumentException | La secuencia no admite la lectura, es nula o ya está cerrada. |

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Inicializa una nueva instancia del[`Document`](../) class. Abre un documento de OneNote existente desde una secuencia. Permite especificar opciones adicionales como una contraseña de cifrado.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| inStream | Stream | El arroyo. |
| loadOptions | LoadOptions | Opciones utilizadas para cargar un documento. Puede ser nulo. |

### Excepciones

| excepción | condición |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | El formato del documento no se reconoce o no es compatible. |
| [FileCorruptedException](../../filecorruptedexception/) | El documento parece estar dañado y no se puede cargar. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | El documento está encriptado y requiere una contraseña para abrirlo, pero proporcionó una contraseña incorrecta. |
| InvalidOperationException | Hay un problema con el documento y debe informarse a los desarrolladores de Aspose.Note. |
| IOException | Hay una excepción de entrada/salida. |
| ArgumentException | La secuencia no admite la lectura, es nula o ya está cerrada. |

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)


