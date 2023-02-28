---
title: Metered.SetMeteredKey
second_title: Aspose.Note لمرجع NET API
description: Metered طريقة. مجموعات المفاتيح العامة والخاصة التي تم قياسها.
type: docs
weight: 30
url: /ar/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

مجموعات المفاتيح العامة والخاصة التي تم قياسها.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| publicKey | String | المفتاح العمومي. |
| privateKey | String | المفتاح الخاص. |

### ملاحظات

إذا اشتريت ترخيصًا مقننًا ، فيجب استدعاء واجهة برمجة التطبيقات هذه عند بدء تشغيل التطبيق ، عادةً ما يكون هذا كافيًا . ومع ذلك ، إذا فشل في تحميل بيانات الاستهلاك خلال فترة 24 ساعة ، فسيتم تعيين الترخيص على حالة التقييم. لتجنب مثل هذه الحالة ، يجب عليك التحقق بانتظام من حالة الترخيص إذا كانت حالة التقييم ، فاتصل بواجهة برمجة التطبيقات هذه مرة أخرى.

### أمثلة

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

* class [Metered](../)
* مساحة الاسم [Aspose.Note](../../metered/)
* المجسم [Aspose.Note](../../../)


