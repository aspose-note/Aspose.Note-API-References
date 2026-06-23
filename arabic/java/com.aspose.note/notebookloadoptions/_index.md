---
title: "NotebookLoadOptions"
second_title: "مرجع Aspose.Note لـ Java API"
description: "الخيارات المستخدمة لتحميل دفتر ملاحظات."
type: docs
weight: 58
url: /ar/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

الخيارات المستخدمة لتحميل دفتر ملاحظات.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | ينشئ مثيلاً جديداً من الفئة `NotebookLoadOptions`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال صراحةً لاحقاً. |
| [getInstantLoading()](#getInstantLoading--) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال أثناء تحميل المستند الأصلي. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال صراحةً لاحقاً. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال أثناء تحميل المستند الأصلي. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


ينشئ مثيلاً جديداً من الفئة `NotebookLoadOptions`.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال صراحةً لاحقاً.

--------------------

القيمة الافتراضية هي `false`، لذا سيتم تحميل المستندات الفرعية ضمنيًا. القيمة `true` تشير إلى أن المستخدم يجب أن يستدعي `Notebook.loadChildDocument` أو لكل عقدة فرعية للدفتر بعد تحميل الدفتر نفسه. إذا كانت القيمة `true`، سيتم تجاهل خيار `NotebookLoadOptions.instantLoading`. إذا كان الدفتر يُحمَّل من تدفق، تكون القيمة دائمًا `true` رغم أنه تم تعيينها صراحةً من قبل المستخدم إلى `false`.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال أثناء تحميل المستند الأصلي.

--------------------

القيمة الافتراضية هي `false`، لذا سيتم تحميل المستندات الفرعية "بشكل كسول"، أي يجب تأجيل تحميلها حتى الوصول المباشر إلى الطفل المحدد. القيمة `true` تشير إلى أن تحميلها يجب أن يتم فورًا.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال صراحةً لاحقاً.

--------------------

القيمة الافتراضية هي `false`، لذا سيتم تحميل المستندات الفرعية ضمنيًا. القيمة `true` تشير إلى أن المستخدم يجب أن يستدعي `Notebook.loadChildDocument` أو لكل عقدة فرعية للدفتر بعد تحميل الدفتر نفسه. إذا كانت القيمة `true`، سيتم تجاهل خيار `NotebookLoadOptions.instantLoading`. إذا كان الدفتر يُحمَّل من تدفق، تكون القيمة دائمًا `true` رغم أنه تم تعيينها صراحةً من قبل المستخدم إلى `false`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل مستندات الأطفال أثناء تحميل المستند الأصلي.

--------------------

القيمة الافتراضية هي `false`، لذا سيتم تحميل المستندات الفرعية "بشكل كسول"، أي يجب تأجيل تحميلها حتى الوصول المباشر إلى الطفل المحدد. القيمة `true` تشير إلى أن تحميلها يجب أن يتم فورًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

