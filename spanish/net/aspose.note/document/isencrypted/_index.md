---
title: Document.IsEncrypted
second_title: Aspose.Note para la referencia de la API de .NET
description: Document método. Comprueba si un documento de un flujo está encriptado. Para verificarlo necesitamos cargar completamente este documento. Por lo tanto este método puede provocar una penalización en el rendimiento.
type: docs
weight: 150
url: /es/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Comprueba si un documento de un flujo está encriptado. Para verificarlo, necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El arroyo. |
| options | LoadOptions | Las opciones de carga. |
| document | Document& | El documento cargado. |

### Valor_devuelto

Devuelve verdadero si el documento está encriptado, de lo contrario falso.

### Ejemplos

Muestra cómo comprobar si un documento está protegido con contraseña.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Muestra cómo verificar si un documento está protegido por contraseña con una contraseña específica.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Comprueba si un documento de un flujo está encriptado. Para verificarlo, necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El arroyo. |
| password | String | La contraseña para descifrar un documento. |
| document | Document& | El documento cargado. |

### Valor_devuelto

Devuelve verdadero si el documento está encriptado, de lo contrario falso.

### Ejemplos

Muestra cómo comprobar si un documento está protegido con contraseña.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Muestra cómo verificar si un documento está protegido por contraseña con una contraseña específica.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Comprueba si un documento de un flujo está encriptado. Para verificarlo, necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El arroyo. |
| document | Document& | El documento cargado. |

### Valor_devuelto

Devuelve verdadero si el documento está encriptado, de lo contrario falso.

### Ejemplos

Muestra cómo comprobar si un documento está protegido con contraseña.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Muestra cómo verificar si un documento está protegido por contraseña con una contraseña específica.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Comprueba si un documento de un archivo está encriptado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |
| options | LoadOptions | Las opciones de carga. |
| document | Document& | El documento cargado. |

### Valor_devuelto

Devuelve verdadero si el documento está encriptado, de lo contrario falso.

### Ejemplos

Muestra cómo comprobar si un documento está protegido con contraseña.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Muestra cómo verificar si un documento está protegido por contraseña con una contraseña específica.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Comprueba si un documento de un archivo está encriptado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |
| document | Document& | El documento cargado. |

### Valor_devuelto

Devuelve verdadero si el documento está encriptado, de lo contrario falso.

### Ejemplos

Muestra cómo comprobar si un documento está protegido con contraseña.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Muestra cómo verificar si un documento está protegido por contraseña con una contraseña específica.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Comprueba si un documento de un archivo está encriptado. Para comprobarlo necesitamos cargar completamente este documento. Por lo tanto, este método puede provocar una penalización en el rendimiento.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |
| password | String | La contraseña para descifrar un documento. |
| document | Document& | El documento cargado. |

### Valor_devuelto

Devuelve verdadero si el documento está encriptado, de lo contrario falso.

### Ejemplos

Muestra cómo comprobar si un documento está protegido con contraseña.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Muestra cómo verificar si un documento está protegido por contraseña con una contraseña específica.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Ver también

* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)


