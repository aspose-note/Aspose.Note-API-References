---
title: "ExtendedApsDocument"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "전체 one-note 문서를 나타내며, 페이지를 페이지 세트로 변환한 것입니다."
type: docs
weight: 23
url: /ko/java/com.aspose.note/extendedapsdocument/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsDocument extends ApsNode implements System.Collections.Generic.IGenericEnumerable<ApsPage>
```

전체 OneNote 문서를 나타내며, 페이지를 페이지 세트로 변환하여 구성됩니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ExtendedApsDocument()](#ExtendedApsDocument--) | 새로운 `ExtendedApsDocument` 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(ApsDocumentVisitor visitor)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) | 이 요소에 ApsDocumentVisitor를 수락합니다. |
| [addPage(ApsPage page)](#addPage-com.aspose.foundation.rendering.ApsPage-) | 문서에 페이지 세트를 추가합니다. |
| [getPageList()](#getPageList--) | 페이지 세트 목록을 가져옵니다. |
| [iterator()](#iterator--) | 열거자를 반환합니다. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) |  |
### ExtendedApsDocument() {#ExtendedApsDocument--}
```
public ExtendedApsDocument()
```


새로운 `ExtendedApsDocument` 클래스 인스턴스를 초기화합니다.

### accept(ApsDocumentVisitor visitor) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor visitor)
```


이 요소에 ApsDocumentVisitor를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 방문자 | com.aspose.foundation.rendering.ApsDocumentVisitor | 방문자. |

### addPage(ApsPage page) {#addPage-com.aspose.foundation.rendering.ApsPage-}
```
public void addPage(ApsPage page)
```


문서에 페이지 세트를 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 페이지 | com.aspose.foundation.rendering.ApsPage | 페이지 세트. |

### getPageList() {#getPageList--}
```
public System.Collections.Generic.List<ApsPage> getPageList()
```


페이지 세트 목록을 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsPage> iterator()
```


열거자를 반환합니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```




**Returns:**
com.aspose.ms.System.Collections.IEnumerator
