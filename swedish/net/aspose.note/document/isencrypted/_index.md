---
title: IsEncrypted
second_title: Aspose.Note för .NET API-referens
description: Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff.
type: docs
weight: 150
url: /sv/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Strömmen. |
| options | LoadOptions | Inläsningsalternativen. |
| document | Document& | Det laddade dokumentet. |

### Returvärde

Returnerar sant om dokumentet är krypterat annars falskt.

### Exempel

Visar hur man kontrollerar om ett dokument är lösenordsskyddat.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man kontrollerar om ett dokument är lösenordsskyddat med ett specifikt lösenord.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Strömmen. |
| password | String | Lösenordet för att dekryptera ett dokument. |
| document | Document& | Det laddade dokumentet. |

### Returvärde

Returnerar sant om dokumentet är krypterat annars falskt.

### Exempel

Visar hur man kontrollerar om ett dokument är lösenordsskyddat.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man kontrollerar om ett dokument är lösenordsskyddat med ett specifikt lösenord.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Kontrollerar om ett dokument från en ström är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | Strömmen. |
| document | Document& | Det laddade dokumentet. |

### Returvärde

Returnerar sant om dokumentet är krypterat annars falskt.

### Exempel

Visar hur man kontrollerar om ett dokument är lösenordsskyddat.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man kontrollerar om ett dokument är lösenordsskyddat med ett specifikt lösenord.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filsökvägen. |
| options | LoadOptions | Inläsningsalternativen. |
| document | Document& | Det laddade dokumentet. |

### Returvärde

Returnerar sant om dokumentet är krypterat annars falskt.

### Exempel

Visar hur man kontrollerar om ett dokument är lösenordsskyddat.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man kontrollerar om ett dokument är lösenordsskyddat med ett specifikt lösenord.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filsökvägen. |
| document | Document& | Det laddade dokumentet. |

### Returvärde

Returnerar sant om dokumentet är krypterat annars falskt.

### Exempel

Visar hur man kontrollerar om ett dokument är lösenordsskyddat.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man kontrollerar om ett dokument är lösenordsskyddat med ett specifikt lösenord.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Kontrollerar om ett dokument från en fil är krypterat. För att kontrollera det måste vi ladda det här dokumentet helt. Så den här metoden kan leda till prestationsstraff.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filsökvägen. |
| password | String | Lösenordet för att dekryptera ett dokument. |
| document | Document& | Det laddade dokumentet. |

### Returvärde

Returnerar sant om dokumentet är krypterat annars falskt.

### Exempel

Visar hur man kontrollerar om ett dokument är lösenordsskyddat.

```csharp
// Sökvägen till dokumentkatalogen.
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

Visar hur man kontrollerar om ett dokument är lösenordsskyddat med ett specifikt lösenord.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
