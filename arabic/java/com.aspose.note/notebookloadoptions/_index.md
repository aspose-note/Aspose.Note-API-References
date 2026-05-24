---
title: "NotebookLoadOptions"
second_title: "مرجع Aspose.Note for Java API"
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
| [NotebookLoadOptions()](#NotebookLoadOptions--) | ينشئ مثلاً جديداً من الفئة `NotebookLoadOptions`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية صراحةً لاحقاً. |
| [getInstantLoading()](#getInstantLoading--) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية أثناء تحميل المستند الأصلي. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية صراحةً لاحقاً. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية أثناء تحميل المستند الأصلي. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


ينشئ مثلاً جديداً من الفئة `NotebookLoadOptions`.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية صراحةً لاحقاً.

--------------------

القيمة الافتراضية هي `false`، لذلك سيتم تحميل المستندات الفرعية ضمنيًا. القيمة `true` تشير إلى أنه يجب على المستخدم استدعاء `Notebook.loadChildDocument` أو لكل عقدة فرعية للمفكرة بعد تحميل المفكرة نفسها. إذا كانت القيمة `true`، سيتم تجاهل خيار `NotebookLoadOptions.instantLoading`. إذا كانت المفكرة تُحمَّل من تدفق، تكون القيمة دائمًا `true` رغم أنه تم تعيينها صراحةً من قبل المستخدم إلى `false`.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية أثناء تحميل المستند الأصلي.

--------------------

القيمة الافتراضية هي `false`، لذلك سيتم تحميل المستندات الفرعية "بشكل كسول"، أي يجب تأجيل تحميلها حتى الوصول المباشر إلى الفرع المحدد. القيمة `true` تشير إلى أنه يجب تحميلها فورًا.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية صراحةً لاحقاً.

--------------------

القيمة الافتراضية هي `false`، لذلك سيتم تحميل المستندات الفرعية ضمنيًا. القيمة `true` تشير إلى أنه يجب على المستخدم استدعاء `Notebook.loadChildDocument` أو لكل عقدة فرعية للمفكرة بعد تحميل المفكرة نفسها. إذا كانت القيمة `true`، سيتم تجاهل خيار `NotebookLoadOptions.instantLoading`. إذا كانت المفكرة تُحمَّل من تدفق، تكون القيمة دائمًا `true` رغم أنه تم تعيينها صراحةً من قبل المستخدم إلى `false`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية أثناء تحميل المستند الأصلي.

--------------------

القيمة الافتراضية هي `false`، لذلك سيتم تحميل المستندات الفرعية "بشكل كسول"، أي يجب تأجيل تحميلها حتى الوصول المباشر إلى الفرع المحدد. القيمة `true` تشير إلى أنه يجب تحميلها فورًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

