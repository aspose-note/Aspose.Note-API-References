---
title: "الفئة Metered"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Metered. توفر طرقًا لتعيين المفتاح القابل للقياس"
type: docs
weight: 420
url: /ar/net/aspose.note/metered/
---
## Metered class

يوفر أساليب لتعيين المفتاح المقيس.

```csharp
public class Metered
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [Metered](metered/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | يزيل الترخيص المُعد مسبقًا. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | يضبط المفاتيح العامة والخاصة القابلة للقياس. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | يحصل على رصيد الاستهلاك. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | يحصل على حجم ملف الاستهلاك. |

## أمثلة

في هذا المثال، سيتم محاولة تعيين المفتاح العام والخاص القابل للقياس.

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

يوضح كيفية تعيين الترخيص القابل للقياس.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### انظر أيضًا

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


