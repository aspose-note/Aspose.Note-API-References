---
title: "KeepSolidObjectsAlgorithm"
second_title: "Aspose.Note for Java API Reference"
description: "यदि पूर्ण वस्तु मूल पृष्ठ में फिट नहीं होती है तो उसे अगले पृष्ठ पर शिफ्ट करता है।"
type: docs
weight: 43
url: /hi/java/com.aspose.note/keepsolidobjectsalgorithm/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
```
public class KeepSolidObjectsAlgorithm extends PageSplittingAlgorithm
```

Shifts full object to the next page in case it doesn't fit in original page.
## Constructors

| Constructor | Description |
| --- | --- |
| [KeepSolidObjectsAlgorithm()](#KeepSolidObjectsAlgorithm--) | डिफ़ॉल्ट ऊँचाई सीमा वाले क्लोन किए गए भाग का उपयोग करके `KeepSolidObjectsAlgorithm` क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [KeepSolidObjectsAlgorithm(float heightLimitOfClonedPart)](#KeepSolidObjectsAlgorithm-float-) | विशिष्ट ऊँचाई सीमा वाले क्लोन किए गए भाग का उपयोग करके `KeepSolidObjectsAlgorithm` क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
## Fields

| Field | Description |
| --- | --- |
| [DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART](#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART) | The default max size of cloned part. |
## Methods

| Method | Description |
| --- | --- |
| [getHeightLimitOfClonedPart()](#getHeightLimitOfClonedPart--) | Gets the height limit of cloned part. |
### KeepSolidObjectsAlgorithm() {#KeepSolidObjectsAlgorithm--}
```
public KeepSolidObjectsAlgorithm()
```


डिफ़ॉल्ट ऊँचाई सीमा वाले क्लोन किए गए भाग का उपयोग करके `KeepSolidObjectsAlgorithm` क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है।

### KeepSolidObjectsAlgorithm(float heightLimitOfClonedPart) {#KeepSolidObjectsAlgorithm-float-}
```
public KeepSolidObjectsAlgorithm(float heightLimitOfClonedPart)
```


विशिष्ट ऊँचाई सीमा वाले क्लोन किए गए भाग का उपयोग करके `KeepSolidObjectsAlgorithm` क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| heightLimitOfClonedPart | float | The max height of cloned part. |

### DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART {#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART}
```
public static final float DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART
```


The default max size of cloned part.

### getHeightLimitOfClonedPart() {#getHeightLimitOfClonedPart--}
```
public float getHeightLimitOfClonedPart()
```


Gets the height limit of cloned part.

**Returns:**
float
