---
title: "License.SetLicense"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة License. ترخص المكوّن"
type: docs
weight: 20
url: /ar/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

يرخص المكوّن.

```csharp
public void SetLicense(string licenseName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| licenseName | String | يمكن أن يكون اسم ملف كامل أو قصير أو اسم مورد مضمّن. استخدم سلسلة فارغة للتبديل إلى وضع التقييم. |

## ملاحظات

يحاول العثور على الترخيص في المواقع التالية:

1. مسار صريح.

2. المجلد الذي يحتوي على تجميع مكوّن Aspose.

3. المجلد الذي يحتوي على تجميع استدعاء العميل.

4. المجلد الذي يحتوي على تجميع الدخول (بدء التشغيل).

5. مورد مضمّن في تجميع استدعاء العميل.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. مسار صريح.

2. مورد مضمّن في تجميع استدعاء العميل.

## أمثلة

في هذا المثال، سيتم محاولة العثور على ملف ترخيص باسم MyLicense.lic في المجلد الذي يحتوي على المكوّن، في المجلد الذي يحتوي على التجميع المستدعي، في مجلد التجميع الرئيسي ثم في الموارد المدمجة للتجميع المستدعي.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

يوضح كيفية تحميل ترخيص لـ Aspose.Note من ملف.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

يوضح كيفية تحميل ترخيص لـ Aspose.Note من مورد ملف مدمج.

```csharp
// إنشاء كائن من الفئة License
Aspose.Note.License license = new Aspose.Note.License();

// مرّر فقط اسم ملف الترخيص المدمج في التجميع
license.SetLicense("Aspose.Note.lic");
```

### انظر أيضًا

* class [License](../)
* namespace [Aspose.Note](../../license/)
* assembly [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

يرخص المكوّن.

```csharp
public void SetLicense(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | دفق يحتوي على الترخيص. |

## ملاحظات

استخدم هذه الطريقة لتحميل ترخيص من دفق.

## أمثلة

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)
```

يوضح كيفية تحميل ترخيص لـ Aspose.Note من تدفق.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### انظر أيضًا

* class [License](../)
* namespace [Aspose.Note](../../license/)
* assembly [Aspose.Note](../../../)


