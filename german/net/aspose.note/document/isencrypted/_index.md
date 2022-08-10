---
title: IsEncrypted
second_title: Aspose.Note für .NET-API-Referenz
description: Überprüft ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu überprüfen müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen.
type: docs
weight: 150
url: /de/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Strom. |
| options | LoadOptions | Die Ladeoptionen. |
| document | Document& | Das geladene Dokument. |

### Rückgabewert

Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.

### Beispiele

Zeigt, wie überprüft wird, ob ein Dokument passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie überprüft werden kann, ob ein Dokument durch ein bestimmtes Passwort passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Strom. |
| password | String | Das Passwort zum Entschlüsseln eines Dokuments. |
| document | Document& | Das geladene Dokument. |

### Rückgabewert

Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.

### Beispiele

Zeigt, wie überprüft wird, ob ein Dokument passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie überprüft werden kann, ob ein Dokument durch ein bestimmtes Passwort passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Überprüft, ob ein Dokument aus einem Stream verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Strom. |
| document | Document& | Das geladene Dokument. |

### Rückgabewert

Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.

### Beispiele

Zeigt, wie überprüft wird, ob ein Dokument passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie überprüft werden kann, ob ein Dokument durch ein bestimmtes Passwort passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Dateipfad. |
| options | LoadOptions | Die Ladeoptionen. |
| document | Document& | Das geladene Dokument. |

### Rückgabewert

Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.

### Beispiele

Zeigt, wie überprüft wird, ob ein Dokument passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie überprüft werden kann, ob ein Dokument durch ein bestimmtes Passwort passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Dateipfad. |
| document | Document& | Das geladene Dokument. |

### Rückgabewert

Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.

### Beispiele

Zeigt, wie überprüft wird, ob ein Dokument passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie überprüft werden kann, ob ein Dokument durch ein bestimmtes Passwort passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Überprüft, ob ein Dokument aus einer Datei verschlüsselt ist. Um dies zu überprüfen, müssen wir dieses Dokument vollständig laden. Diese Methode kann also zu Leistungseinbußen führen.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Dateipfad. |
| password | String | Das Passwort zum Entschlüsseln eines Dokuments. |
| document | Document& | Das geladene Dokument. |

### Rückgabewert

Gibt true zurück, wenn das Dokument verschlüsselt ist, andernfalls false.

### Beispiele

Zeigt, wie überprüft wird, ob ein Dokument passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie überprüft werden kann, ob ein Dokument durch ein bestimmtes Passwort passwortgeschützt ist.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
