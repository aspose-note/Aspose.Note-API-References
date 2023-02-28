---
title: Document.Document
second_title: Aspose.Note for .NET API Referansı
description: Document inşaatçı. Yeni bir örneğini başlatır.Document class. Boş bir OneNote belgesi oluşturur.
type: docs
weight: 10
url: /tr/net/aspose.note/document/document/
---
## Document() {#constructor}

Yeni bir örneğini başlatır.[`Document`](../) class. Boş bir OneNote belgesi oluşturur.

```csharp
public Document()
```

### Ayrıca bakınız

* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Yeni bir örneğini başlatır.[`Document`](../) class. Bir dosyadan mevcut bir OneNote belgesini açar.

```csharp
public Document(string filePath)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |

### istisnalar

| istisna | şart |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Belge biçimi tanınmıyor veya desteklenmiyor. |
| [FileCorruptedException](../../filecorruptedexception/) | Belge bozuk görünüyor ve yüklenemiyor. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Belge şifreli ve açılması için parola gerekiyor, ancak parolayı yanlış girdiniz. |
| InvalidOperationException | Belgede bir sorun var ve Aspose.Note geliştiricilerine bildirilmesi gerekiyor. |
| IOException | Bir giriş/çıkış istisnası var. |

### Ayrıca bakınız

* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Yeni bir örneğini başlatır.[`Document`](../)class. Bir dosyadan mevcut bir OneNote belgesini açar. Şifreleme parolası gibi ek seçeneklerin belirtilmesine izin verir.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |
| loadOptions | LoadOptions | Belge yüklemek için kullanılan seçenekler. Boş olabilir. |

### istisnalar

| istisna | şart |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Belge biçimi tanınmıyor veya desteklenmiyor. |
| [FileCorruptedException](../../filecorruptedexception/) | Belge bozuk görünüyor ve yüklenemiyor. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Belge şifreli ve açılması için parola gerekiyor, ancak parolayı yanlış girdiniz. |
| InvalidOperationException | Belgede bir sorun var ve Aspose.Note geliştiricilerine bildirilmesi gerekiyor. |
| IOException | Bir giriş/çıkış istisnası var. |

### Ayrıca bakınız

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Yeni bir örneğini başlatır.[`Document`](../) class. Akıştan mevcut bir OneNote belgesini açar.

```csharp
public Document(Stream inStream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| inStream | Stream | Akış. |

### istisnalar

| istisna | şart |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Belge biçimi tanınmıyor veya desteklenmiyor. |
| [FileCorruptedException](../../filecorruptedexception/) | Belge bozuk görünüyor ve yüklenemiyor. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Belge şifreli ve açılması için parola gerekiyor, ancak parolayı yanlış girdiniz. |
| InvalidOperationException | Belgede bir sorun var ve Aspose.Note geliştiricilerine bildirilmesi gerekiyor. |
| IOException | Bir giriş/çıkış istisnası var. |
| ArgumentException | Akış okumayı desteklemiyor, boş veya zaten kapalı. |

### Ayrıca bakınız

* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Yeni bir örneğini başlatır.[`Document`](../) class. Akıştan mevcut bir OneNote belgesini açar. Şifreleme parolası gibi ek seçeneklerin belirtilmesine izin verir.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| inStream | Stream | Akış. |
| loadOptions | LoadOptions | Belge yüklemek için kullanılan seçenekler. Boş olabilir. |

### istisnalar

| istisna | şart |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Belge biçimi tanınmıyor veya desteklenmiyor. |
| [FileCorruptedException](../../filecorruptedexception/) | Belge bozuk görünüyor ve yüklenemiyor. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Belge şifreli ve açılması için parola gerekiyor, ancak parolayı yanlış girdiniz. |
| InvalidOperationException | Belgede bir sorun var ve Aspose.Note geliştiricilerine bildirilmesi gerekiyor. |
| IOException | Bir giriş/çıkış istisnası var. |
| ArgumentException | Akış okumayı desteklemiyor, boş veya zaten kapalı. |

### Ayrıca bakınız

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)


