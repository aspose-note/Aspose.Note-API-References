---
title: Class License
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.License sınıf. Bileşeni lisanslamak için yöntemler sağlar.
type: docs
weight: 310
url: /tr/net/aspose.note/license/
---
## License class

Bileşeni lisanslamak için yöntemler sağlar.

```csharp
public class License
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [License](license/)() | Default_Constructor |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | Bileşeni lisanslar. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | Bileşeni lisanslar. |

### Örnekler

Aspose.Note için bir lisansın bir dosyadan nasıl yükleneceğini gösterir.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Bir akıştan Aspose.Note için bir lisansın nasıl yükleneceğini gösterir.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

Gömülü dosya kaynağından Aspose.Note için bir lisansın nasıl yükleneceğini gösterir.

```csharp
// Lisans sınıfını başlat
Aspose.Note.License license = new Aspose.Note.License();

// Yalnızca derlemeye katıştırılmış lisans dosyasının adını iletin
license.SetLicense("Aspose.Note.lic");
```

### Ayrıca bakınız

* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


