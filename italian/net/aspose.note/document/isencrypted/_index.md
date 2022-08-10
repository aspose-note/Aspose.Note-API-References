---
title: IsEncrypted
second_title: Aspose.Note per .NET API Reference
description: Verifica se un documento da un flusso è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni.
type: docs
weight: 150
url: /it/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Verifica se un documento da un flusso è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso. |
| options | LoadOptions | Le opzioni di caricamento. |
| document | Document& | Il documento caricato. |

### Valore di ritorno

Restituisce vero se il documento è crittografato altrimenti falso.

### Esempi

Mostra come verificare se un documento è protetto da password.

```csharp
// Il percorso della directory dei documenti.
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

Mostra come verificare se un documento è protetto da una password specifica.

```csharp
// Il percorso della directory dei documenti.
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

### Guarda anche

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Verifica se un documento da un flusso è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso. |
| password | String | La password per decrittografare un documento. |
| document | Document& | Il documento caricato. |

### Valore di ritorno

Restituisce vero se il documento è crittografato altrimenti falso.

### Esempi

Mostra come verificare se un documento è protetto da password.

```csharp
// Il percorso della directory dei documenti.
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

Mostra come verificare se un documento è protetto da una password specifica.

```csharp
// Il percorso della directory dei documenti.
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

### Guarda anche

* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Verifica se un documento da un flusso è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso. |
| document | Document& | Il documento caricato. |

### Valore di ritorno

Restituisce vero se il documento è crittografato altrimenti falso.

### Esempi

Mostra come verificare se un documento è protetto da password.

```csharp
// Il percorso della directory dei documenti.
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

Mostra come verificare se un documento è protetto da una password specifica.

```csharp
// Il percorso della directory dei documenti.
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

### Guarda anche

* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Verifica se un documento da un file è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |
| options | LoadOptions | Le opzioni di caricamento. |
| document | Document& | Il documento caricato. |

### Valore di ritorno

Restituisce vero se il documento è crittografato altrimenti falso.

### Esempi

Mostra come verificare se un documento è protetto da password.

```csharp
// Il percorso della directory dei documenti.
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

Mostra come verificare se un documento è protetto da una password specifica.

```csharp
// Il percorso della directory dei documenti.
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

### Guarda anche

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Verifica se un documento da un file è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |
| document | Document& | Il documento caricato. |

### Valore di ritorno

Restituisce vero se il documento è crittografato altrimenti falso.

### Esempi

Mostra come verificare se un documento è protetto da password.

```csharp
// Il percorso della directory dei documenti.
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

Mostra come verificare se un documento è protetto da una password specifica.

```csharp
// Il percorso della directory dei documenti.
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

### Guarda anche

* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Verifica se un documento da un file è crittografato. Per verificarlo dobbiamo caricare completamente questo documento. Quindi questo metodo può comportare una riduzione delle prestazioni.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |
| password | String | La password per decrittografare un documento. |
| document | Document& | Il documento caricato. |

### Valore di ritorno

Restituisce vero se il documento è crittografato altrimenti falso.

### Esempi

Mostra come verificare se un documento è protetto da password.

```csharp
// Il percorso della directory dei documenti.
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

Mostra come verificare se un documento è protetto da una password specifica.

```csharp
// Il percorso della directory dei documenti.
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

### Guarda anche

* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
