---
title: "Document.IsEncrypted"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Document. تتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد تؤدي هذه الطريقة إلى عقوبة في الأداء"
type: docs
weight: 150
url: /ar/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |
| خيارات | LoadOptions | خيارات التحميل. |
| مستند | Document& | المستند المحمَّل. |

### قيمة الإرجاع

يرجع true إذا كان المستند مشفرًا وإلا false.

## أمثلة

يعرض كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

```csharp
// المسار إلى دليل المستندات.
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

يظهر كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور محددة.

```csharp
// المسار إلى دليل المستندات.
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

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |
| كلمة المرور | String | كلمة المرور لفك تشفير مستند. |
| مستند | Document& | المستند المحمَّل. |

### قيمة الإرجاع

يرجع true إذا كان المستند مشفرًا وإلا false.

## أمثلة

يعرض كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

```csharp
// المسار إلى دليل المستندات.
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

يظهر كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور محددة.

```csharp
// المسار إلى دليل المستندات.
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

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |
| مستند | Document& | المستند المحمَّل. |

### قيمة الإرجاع

يرجع true إذا كان المستند مشفرًا وإلا false.

## أمثلة

يعرض كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

```csharp
// المسار إلى دليل المستندات.
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

يظهر كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور محددة.

```csharp
// المسار إلى دليل المستندات.
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

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| خيارات | LoadOptions | خيارات التحميل. |
| مستند | Document& | المستند المحمَّل. |

### قيمة الإرجاع

يرجع true إذا كان المستند مشفرًا وإلا false.

## أمثلة

يعرض كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

```csharp
// المسار إلى دليل المستندات.
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

يظهر كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور محددة.

```csharp
// المسار إلى دليل المستندات.
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

### انظر أيضًا

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| مستند | Document& | المستند المحمَّل. |

### قيمة الإرجاع

يرجع true إذا كان المستند مشفرًا وإلا false.

## أمثلة

يعرض كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

```csharp
// المسار إلى دليل المستندات.
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

يظهر كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور محددة.

```csharp
// المسار إلى دليل المستندات.
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

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| كلمة المرور | String | كلمة المرور لفك تشفير مستند. |
| مستند | Document& | المستند المحمَّل. |

### قيمة الإرجاع

يرجع true إذا كان المستند مشفرًا وإلا false.

## أمثلة

يعرض كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

```csharp
// المسار إلى دليل المستندات.
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

يظهر كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور محددة.

```csharp
// المسار إلى دليل المستندات.
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

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


