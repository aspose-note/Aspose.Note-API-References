---
title: "Metered.SetMeteredKey"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Metered. تعيين المفاتيح العامة والخاصة للعداد"
type: docs
weight: 30
url: /ar/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

يضبط المفاتيح العامة والخاصة القابلة للقياس.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| publicKey | String | المفتاح العام. |
| privateKey | String | المفتاح الخاص. |

## ملاحظات

إذا قمت بشراء ترخيص عددي، يجب استدعاء هذه الواجهة البرمجية عند بدء تشغيل التطبيق، عادةً يكون ذلك كافياً. ومع ذلك، إذا فشل العداد في رفع بيانات الاستهلاك خلال فترة 24 ساعة، سيتم تعيين الترخيص إلى حالة التقييم. لتجنب هذه الحالة، يجب عليك فحص حالة الترخيص بانتظام؛ إذا كانت حالة التقييم، استدعِ هذه الواجهة البرمجية مرة أخرى.

## أمثلة

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

* class [Metered](../)
* namespace [Aspose.Note](../../metered/)
* assembly [Aspose.Note](../../../)


