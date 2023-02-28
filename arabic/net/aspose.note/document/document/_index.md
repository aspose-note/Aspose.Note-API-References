---
title: Document.Document
second_title: Aspose.Note لمرجع NET API
description: Document البناء. يقوم بتهيئة مثيل جديد لملفDocument class. ينشئ مستند OneNote فارغًا.
type: docs
weight: 10
url: /ar/net/aspose.note/document/document/
---
## Document() {#constructor}

يقوم بتهيئة مثيل جديد لملف[`Document`](../) class. ينشئ مستند OneNote فارغًا.

```csharp
public Document()
```

### أنظر أيضا

* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

يقوم بتهيئة مثيل جديد لملف[`Document`](../) class. يفتح مستند OneNote موجود من ملف.

```csharp
public Document(string filePath)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | تنسيق المستند غير معروف أو غير مدعوم. |
| [FileCorruptedException](../../filecorruptedexception/) | يبدو أن المستند تالف ولا يمكن تحميله. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | المستند مشفر ويتطلب كلمة مرور لفتحه ، لكنك أدخلت كلمة مرور غير صحيحة. |
| InvalidOperationException | توجد مشكلة في المستند ويجب إبلاغ مطوري Aspose.Note بها. |
| IOException | هناك استثناء الإدخال / الإخراج. |

### أنظر أيضا

* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

يقوم بتهيئة مثيل جديد لملف[`Document`](../)class. يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| loadOptions | LoadOptions | الخيارات المستخدمة لتحميل مستند. يمكن أن يكون فارغًا. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | تنسيق المستند غير معروف أو غير مدعوم. |
| [FileCorruptedException](../../filecorruptedexception/) | يبدو أن المستند تالف ولا يمكن تحميله. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | المستند مشفر ويتطلب كلمة مرور لفتحه ، لكنك أدخلت كلمة مرور غير صحيحة. |
| InvalidOperationException | توجد مشكلة في المستند ويجب إبلاغ مطوري Aspose.Note بها. |
| IOException | هناك استثناء الإدخال / الإخراج. |

### أنظر أيضا

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`Document`](../) class. يفتح مستند OneNote موجود من دفق.

```csharp
public Document(Stream inStream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| inStream | Stream | الدفق . |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | تنسيق المستند غير معروف أو غير مدعوم. |
| [FileCorruptedException](../../filecorruptedexception/) | يبدو أن المستند تالف ولا يمكن تحميله. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | المستند مشفر ويتطلب كلمة مرور لفتحه ، لكنك أدخلت كلمة مرور غير صحيحة. |
| InvalidOperationException | توجد مشكلة في المستند ويجب إبلاغ مطوري Aspose.Note بها. |
| IOException | هناك استثناء الإدخال / الإخراج. |
| ArgumentException | الدفق لا يدعم القراءة أو أنه فارغ أو مغلق بالفعل. |

### أنظر أيضا

* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`Document`](../) class. يفتح مستند OneNote موجود من دفق. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| inStream | Stream | الدفق . |
| loadOptions | LoadOptions | الخيارات المستخدمة لتحميل مستند. يمكن أن يكون فارغًا. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | تنسيق المستند غير معروف أو غير مدعوم. |
| [FileCorruptedException](../../filecorruptedexception/) | يبدو أن المستند تالف ولا يمكن تحميله. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | المستند مشفر ويتطلب كلمة مرور لفتحه ، لكنك أدخلت كلمة مرور غير صحيحة. |
| InvalidOperationException | توجد مشكلة في المستند ويجب إبلاغ مطوري Aspose.Note بها. |
| IOException | هناك استثناء الإدخال / الإخراج. |
| ArgumentException | الدفق لا يدعم القراءة أو أنه فارغ أو مغلق بالفعل. |

### أنظر أيضا

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)


