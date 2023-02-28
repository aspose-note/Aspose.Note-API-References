---
title: Document.IsEncrypted
second_title: Aspose.Note voor .NET API-referentie
description: Document methode. Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf.
type: docs
weight: 150
url: /nl/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stroom. |
| options | LoadOptions | De laadopties. |
| document | Document& | Het geladen document. |

### Winstwaarde

Retourneert waar als het document is gecodeerd, anders onwaar.

### Voorbeelden

Laat zien hoe u kunt controleren of een document met een wachtwoord is beveiligd.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u kunt controleren of een document met een specifiek wachtwoord is beveiligd met een wachtwoord.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stroom. |
| password | String | Het wachtwoord om een document te decoderen. |
| document | Document& | Het geladen document. |

### Winstwaarde

Retourneert waar als het document is gecodeerd, anders onwaar.

### Voorbeelden

Laat zien hoe u kunt controleren of een document met een wachtwoord is beveiligd.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u kunt controleren of een document met een specifiek wachtwoord is beveiligd met een wachtwoord.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Controleert of een document uit een stream versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stroom. |
| document | Document& | Het geladen document. |

### Winstwaarde

Retourneert waar als het document is gecodeerd, anders onwaar.

### Voorbeelden

Laat zien hoe u kunt controleren of een document met een wachtwoord is beveiligd.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u kunt controleren of een document met een specifiek wachtwoord is beveiligd met een wachtwoord.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het bestandspad. |
| options | LoadOptions | De laadopties. |
| document | Document& | Het geladen document. |

### Winstwaarde

Retourneert waar als het document is gecodeerd, anders onwaar.

### Voorbeelden

Laat zien hoe u kunt controleren of een document met een wachtwoord is beveiligd.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u kunt controleren of een document met een specifiek wachtwoord is beveiligd met een wachtwoord.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het bestandspad. |
| document | Document& | Het geladen document. |

### Winstwaarde

Retourneert waar als het document is gecodeerd, anders onwaar.

### Voorbeelden

Laat zien hoe u kunt controleren of een document met een wachtwoord is beveiligd.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u kunt controleren of een document met een specifiek wachtwoord is beveiligd met een wachtwoord.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Controleert of een document uit een bestand versleuteld is. Om dit te controleren moeten we dit document volledig laden. Dus deze methode kan leiden tot een prestatiestraf.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Het bestandspad. |
| password | String | Het wachtwoord om een document te decoderen. |
| document | Document& | Het geladen document. |

### Winstwaarde

Retourneert waar als het document is gecodeerd, anders onwaar.

### Voorbeelden

Laat zien hoe u kunt controleren of een document met een wachtwoord is beveiligd.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u kunt controleren of een document met een specifiek wachtwoord is beveiligd met een wachtwoord.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


