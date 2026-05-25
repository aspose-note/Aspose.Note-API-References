---
title: "NotebookLoadOptions"
second_title: "Aspose.Note for Java API Reference"
description: "Options used to load a notebook."
type: docs
weight: 58
url: /hi/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Options used to load a notebook.
## Constructors

| Constructor | Description |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | `NotebookLoadOptions` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | बाद में स्पष्ट रूप से लोड किए जाने वाले चाइल्ड डॉक्यूमेंट्स को दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [getInstantLoading()](#getInstantLoading--) | पैरेंट डॉक्यूमेंट लोड होते समय चाइल्ड डॉक्यूमेंट्स को लोड किया जाना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | बाद में स्पष्ट रूप से लोड किए जाने वाले चाइल्ड डॉक्यूमेंट्स को दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | पैरेंट डॉक्यूमेंट लोड होते समय चाइल्ड डॉक्यूमेंट्स को लोड किया जाना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


`NotebookLoadOptions` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


बाद में स्पष्ट रूप से लोड किए जाने वाले चाइल्ड डॉक्यूमेंट्स को दर्शाने वाला मान प्राप्त करता है या सेट करता है।

--------------------

डिफ़ॉल्ट मान `false` है, इसलिए चाइल्ड दस्तावेज़ों को स्वचालित रूप से लोड किया जाएगा। मान `true` यह दर्शाता है कि उपयोगकर्ता को `Notebook.loadChildDocument` को कॉल करना चाहिए या नोटबुक स्वयं लोड होने के बाद प्रत्येक नोटबुक के चाइल्ड नोड के लिए। यदि मान `true` है, तो `NotebookLoadOptions.instantLoading` विकल्प को अनदेखा किया जाएगा। यदि नोटबुक स्ट्रीम से लोड हो रहा है, तो मान हमेशा `true` रहेगा, भले ही उपयोगकर्ता ने इसे स्पष्ट रूप से `false` सेट किया हो।

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


पैरेंट डॉक्यूमेंट लोड होते समय चाइल्ड डॉक्यूमेंट्स को लोड किया जाना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

--------------------

डिफ़ॉल्ट मान `false` है, इसलिए चाइल्ड दस्तावेज़ \"धीरज से\" लोड किए जाएंगे, अर्थात् उनका लोडिंग तब तक स्थगित रहना चाहिए जब तक किसी विशिष्ट चाइल्ड तक प्रत्यक्ष पहुँच न हो। मान `true` यह दर्शाता है कि उनका लोडिंग तुरंत किया जाना चाहिए।

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


बाद में स्पष्ट रूप से लोड किए जाने वाले चाइल्ड डॉक्यूमेंट्स को दर्शाने वाला मान प्राप्त करता है या सेट करता है।

--------------------

डिफ़ॉल्ट मान `false` है, इसलिए चाइल्ड दस्तावेज़ों को स्वचालित रूप से लोड किया जाएगा। मान `true` यह दर्शाता है कि उपयोगकर्ता को `Notebook.loadChildDocument` को कॉल करना चाहिए या नोटबुक स्वयं लोड होने के बाद प्रत्येक नोटबुक के चाइल्ड नोड के लिए। यदि मान `true` है, तो `NotebookLoadOptions.instantLoading` विकल्प को अनदेखा किया जाएगा। यदि नोटबुक स्ट्रीम से लोड हो रहा है, तो मान हमेशा `true` रहेगा, भले ही उपयोगकर्ता ने इसे स्पष्ट रूप से `false` सेट किया हो।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


पैरेंट डॉक्यूमेंट लोड होते समय चाइल्ड डॉक्यूमेंट्स को लोड किया जाना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

--------------------

डिफ़ॉल्ट मान `false` है, इसलिए चाइल्ड दस्तावेज़ \"धीरज से\" लोड किए जाएंगे, अर्थात् उनका लोडिंग तब तक स्थगित रहना चाहिए जब तक किसी विशिष्ट चाइल्ड तक प्रत्यक्ष पहुँच न हो। मान `true` यह दर्शाता है कि उनका लोडिंग तुरंत किया जाना चाहिए।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

