---
title: Document.IsEncrypted
second_title: Aspose.Note لمرجع NET API
description: Document طريقة. للتحقق مما إذا كان مستند من دفق مشفر . للتحقق من ذلك  نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء.
type: docs
weight: 150
url: /ar/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

للتحقق مما إذا كان مستند من دفق مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | الدفق . |
| options | LoadOptions | خيارات التحميل . |
| document | Document& | المستند الذي تم تحميله. |

### قيمة الإرجاع

يتم إرجاع صحيح إذا تم تشفير المستند أو خطأ.

### أمثلة

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

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

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور معينة.

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

### أنظر أيضا

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

للتحقق مما إذا كان مستند من دفق مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | الدفق . |
| password | String | كلمة المرور لفك تشفير مستند. |
| document | Document& | المستند الذي تم تحميله. |

### قيمة الإرجاع

يتم إرجاع صحيح إذا تم تشفير المستند أو خطأ.

### أمثلة

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

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

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور معينة.

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

### أنظر أيضا

* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

للتحقق مما إذا كان مستند من دفق مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | الدفق . |
| document | Document& | المستند الذي تم تحميله. |

### قيمة الإرجاع

يتم إرجاع صحيح إذا تم تشفير المستند أو خطأ.

### أمثلة

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

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

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور معينة.

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

### أنظر أيضا

* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

للتحقق مما إذا كان مستند من ملف مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| options | LoadOptions | خيارات التحميل . |
| document | Document& | المستند الذي تم تحميله. |

### قيمة الإرجاع

يتم إرجاع صحيح إذا تم تشفير المستند أو خطأ.

### أمثلة

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

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

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور معينة.

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

### أنظر أيضا

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

للتحقق مما إذا كان مستند من ملف مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| document | Document& | المستند الذي تم تحميله. |

### قيمة الإرجاع

يتم إرجاع صحيح إذا تم تشفير المستند أو خطأ.

### أمثلة

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

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

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور معينة.

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

### أنظر أيضا

* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

للتحقق مما إذا كان مستند من ملف مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| password | String | كلمة المرور لفك تشفير مستند. |
| document | Document& | المستند الذي تم تحميله. |

### قيمة الإرجاع

يتم إرجاع صحيح إذا تم تشفير المستند أو خطأ.

### أمثلة

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

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

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور معينة.

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

### أنظر أيضا

* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)


