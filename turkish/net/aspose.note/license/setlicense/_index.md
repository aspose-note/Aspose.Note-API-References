---
title: License.SetLicense
second_title: Aspose.Note for .NET API Referansı
description: License yöntem. Bileşeni lisanslar.
type: docs
weight: 20
url: /tr/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Bileşeni lisanslar.

```csharp
public void SetLicense(string licenseName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| licenseName | String | Tam veya kısa dosya adı veya katıştırılmış bir kaynağın adı olabilir. Değerlendirme moduna geçmek için boş bir dize kullanın. |

### Notlar

Lisansı aşağıdaki konumlarda bulmaya çalışır:

1. Açık yol.

2. Aspose bileşen montajını içeren klasör.

3. İstemcinin çağrı derlemesini içeren klasör.

4. Giriş (başlangıç) derlemesini içeren klasör.

5. İstemcinin çağrı derlemesinde katıştırılmış bir kaynak.

**Not:**.NET Compact Framework üzerinde, lisansı yalnızca şu konumlarda bulmaya çalışır:

1. Açık yol.

2. İstemcinin çağrı derlemesinde katıştırılmış bir kaynak.

### Örnekler

Aspose.Note için bir lisansın bir dosyadan nasıl yükleneceğini gösterir.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Gömülü dosya kaynağından Aspose.Note için bir lisansın nasıl yükleneceğini gösterir.

```csharp
// Lisans sınıfını başlat
Aspose.Note.License license = new Aspose.Note.License();

// Yalnızca derlemeye katıştırılmış lisans dosyasının adını iletin
license.SetLicense("Aspose.Note.lic");
```

### Ayrıca bakınız

* class [License](../)
* ad alanı [Aspose.Note](../../license/)
* toplantı [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Bileşeni lisanslar.

```csharp
public void SetLicense(Stream stream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Lisansı içeren bir akış. |

### Notlar

Akıştan lisans yüklemek için bu yöntemi kullanın.

### Örnekler

Bir akıştan Aspose.Note için bir lisansın nasıl yükleneceğini gösterir.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### Ayrıca bakınız

* class [License](../)
* ad alanı [Aspose.Note](../../license/)
* toplantı [Aspose.Note](../../../)


