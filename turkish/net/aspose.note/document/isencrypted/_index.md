---
title: IsEncrypted
second_title: Aspose.Note for .NET API Referansı
description: Bir akıştaki belgenin şifrelenip şifrelenmediğini kontrol eder. Bunu kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir.
type: docs
weight: 150
url: /tr/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Bir akıştaki belgenin şifrelenip şifrelenmediğini kontrol eder. Bunu kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Akış. |
| options | LoadOptions | Yükleme seçenekleri. |
| document | Document& | Yüklenen belge. |

### Geri dönüş değeri

Belge şifrelenmişse true döndürür, aksi takdirde false.

### Örnekler

Bir belgenin parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

Bir belgenin belirli bir parolayla parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

### Ayrıca bakınız

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Bir akıştaki belgenin şifrelenip şifrelenmediğini kontrol eder. Bunu kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Akış. |
| password | String | Bir belgenin şifresini çözmek için kullanılan parola. |
| document | Document& | Yüklenen belge. |

### Geri dönüş değeri

Belge şifrelenmişse true döndürür, aksi takdirde false.

### Örnekler

Bir belgenin parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

Bir belgenin belirli bir parolayla parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

### Ayrıca bakınız

* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Bir akıştaki belgenin şifrelenip şifrelenmediğini kontrol eder. Bunu kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Akış. |
| document | Document& | Yüklenen belge. |

### Geri dönüş değeri

Belge şifrelenmişse true döndürür, aksi takdirde false.

### Örnekler

Bir belgenin parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

Bir belgenin belirli bir parolayla parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

### Ayrıca bakınız

* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Bir dosyadaki belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |
| options | LoadOptions | Yükleme seçenekleri. |
| document | Document& | Yüklenen belge. |

### Geri dönüş değeri

Belge şifrelenmişse true döndürür, aksi takdirde false.

### Örnekler

Bir belgenin parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

Bir belgenin belirli bir parolayla parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

### Ayrıca bakınız

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Bir dosyadaki belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |
| document | Document& | Yüklenen belge. |

### Geri dönüş değeri

Belge şifrelenmişse true döndürür, aksi takdirde false.

### Örnekler

Bir belgenin parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

Bir belgenin belirli bir parolayla parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

### Ayrıca bakınız

* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Bir dosyadaki belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için bu belgeyi tamamen yüklememiz gerekir. Dolayısıyla bu yöntem performans cezasına neden olabilir.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |
| password | String | Bir belgenin şifresini çözmek için kullanılan parola. |
| document | Document& | Yüklenen belge. |

### Geri dönüş değeri

Belge şifrelenmişse true döndürür, aksi takdirde false.

### Örnekler

Bir belgenin parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

Bir belgenin belirli bir parolayla parola korumalı olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
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

### Ayrıca bakınız

* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
