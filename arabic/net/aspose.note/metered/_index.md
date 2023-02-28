---
title: Class Metered
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Metered فصل. يوفر طرقًا لتعيين المفتاح المقنن .
type: docs
weight: 350
url: /ar/net/aspose.note/metered/
---
## Metered class

يوفر طرقًا لتعيين المفتاح المقنن .

```csharp
public class Metered
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Metered](metered/)() | Default_Constructor |

## طُرق

| اسم | وصف |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | يزيل ترخيص الإعداد السابق . |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | مجموعات المفاتيح العامة والخاصة التي تم قياسها. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | يحصل على ائتمان الاستهلاك. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | الحصول على حجم ملف الاستهلاك. |

### أمثلة

في هذا المثال ، ستُبذل محاولة لتعيين المفتاح العام والخاص المحسوب

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

يوضح كيفية تعيين الترخيص المقنن.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل مستند OneNote واحصل على الطفل الأول           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### أنظر أيضا

* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


