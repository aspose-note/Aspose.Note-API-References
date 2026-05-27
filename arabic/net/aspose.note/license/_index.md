---
title: "الفئة License"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.License. توفر طرقًا لترخيص المكوّن"
type: docs
weight: 370
url: /ar/net/aspose.note/license/
---
## License class

يوفر أساليب لترخيص المكوّن.

```csharp
public sealed class License
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [License](license/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | يرخص المكوّن. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | يرخص المكوّن. |

## أمثلة

في هذا المثال، سيتم محاولة العثور على ملف ترخيص باسم MyLicense.lic في المجلد الذي يحتوي على المكوّن، في المجلد الذي يحتوي على التجميع المستدعي، في مجلد التجميع الرئيسي ثم في الموارد المدمجة للتجميع المستدعي.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

يوضح كيفية تحميل ترخيص لـ Aspose.Note من ملف.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

يوضح كيفية تحميل ترخيص لـ Aspose.Note من تدفق.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

يوضح كيفية تحميل ترخيص لـ Aspose.Note من مورد ملف مدمج.

```csharp
// إنشاء كائن من الفئة License
Aspose.Note.License license = new Aspose.Note.License();

// مرّر فقط اسم ملف الترخيص المدمج في التجميع
license.SetLicense("Aspose.Note.lic");
```

### انظر أيضًا

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


