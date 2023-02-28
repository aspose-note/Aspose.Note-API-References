---
title: Document.IsEncrypted
second_title: Référence de l'API Aspose.Note pour .NET
description: Document méthode. Vérifie si un document dun flux est crypté. Pour le vérifier nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances.
type: docs
weight: 150
url: /fr/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Vérifie si un document d'un flux est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux. |
| options | LoadOptions | Les options de chargement. |
| document | Document& | Le document chargé. |

### Return_Value

Renvoie true si le document est crypté sinon false.

### Exemples

Montre comment vérifier si un document est protégé par un mot de passe.

```csharp
// Le chemin d'accès au répertoire des documents.
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

Montre comment vérifier si un document est protégé par un mot de passe spécifique.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Vérifie si un document d'un flux est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux. |
| password | String | Le mot de passe pour déchiffrer un document. |
| document | Document& | Le document chargé. |

### Return_Value

Renvoie true si le document est crypté sinon false.

### Exemples

Montre comment vérifier si un document est protégé par un mot de passe.

```csharp
// Le chemin d'accès au répertoire des documents.
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

Montre comment vérifier si un document est protégé par un mot de passe spécifique.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Vérifie si un document d'un flux est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux. |
| document | Document& | Le document chargé. |

### Return_Value

Renvoie true si le document est crypté sinon false.

### Exemples

Montre comment vérifier si un document est protégé par un mot de passe.

```csharp
// Le chemin d'accès au répertoire des documents.
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

Montre comment vérifier si un document est protégé par un mot de passe spécifique.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Vérifie si un document d'un fichier est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin du fichier. |
| options | LoadOptions | Les options de chargement. |
| document | Document& | Le document chargé. |

### Return_Value

Renvoie true si le document est crypté sinon false.

### Exemples

Montre comment vérifier si un document est protégé par un mot de passe.

```csharp
// Le chemin d'accès au répertoire des documents.
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

Montre comment vérifier si un document est protégé par un mot de passe spécifique.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Vérifie si un document d'un fichier est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin du fichier. |
| document | Document& | Le document chargé. |

### Return_Value

Renvoie true si le document est crypté sinon false.

### Exemples

Montre comment vérifier si un document est protégé par un mot de passe.

```csharp
// Le chemin d'accès au répertoire des documents.
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

Montre comment vérifier si un document est protégé par un mot de passe spécifique.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Vérifie si un document d'un fichier est crypté. Pour le vérifier, nous devons charger complètement ce document. Cette méthode peut donc entraîner une baisse des performances.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Le chemin du fichier. |
| password | String | Le mot de passe pour déchiffrer un document. |
| document | Document& | Le document chargé. |

### Return_Value

Renvoie true si le document est crypté sinon false.

### Exemples

Montre comment vérifier si un document est protégé par un mot de passe.

```csharp
// Le chemin d'accès au répertoire des documents.
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

Montre comment vérifier si un document est protégé par un mot de passe spécifique.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)


