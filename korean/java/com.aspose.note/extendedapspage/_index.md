---
title: "ExtendedApsPage"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "표준 ApsGlyphs에 대한 래퍼를 나타내며, 일부 그리기 동작을 확장합니다."
type: docs
weight: 27
url: /ko/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

표준 ApsGlyphs에 대한 래퍼를 나타내며, 일부 그리기 동작을 확장합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | 새 `ExtendedApsPage` 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getContentSize()](#getContentSize--) | 여백을 제외한 페이지 크기를 가져옵니다. |
| [getMargin()](#getMargin--) | 이 페이지의 여백을 가져옵니다. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | MS OneNote 페이지가 여러 aps 페이지로 분할될 때, MS OneNote 페이지에서 페이지 끝 위치를 가져옵니다. |
| [getPageSize()](#getPageSize--) | 최종 페이지 크기를 가져옵니다. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | MS OneNote 페이지가 여러 aps 페이지로 분할될 때, MS OneNote 페이지에서 페이지 시작 위치를 가져옵니다. |
| [iterator()](#iterator--) | 이 페이지의 모든 노드를 순회하는 열거자를 반환합니다. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | 열거자를 가져옵니다. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


새 `ExtendedApsPage` 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | 페이지 크기입니다. |
| pageStartInNotePage | float | 원본 MS OneNote 페이지에서 페이지 시작 위치입니다. |
| margin | com.aspose.foundation.layout.Margin | 확장된 페이지 여백. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


여백을 제외한 페이지 크기를 가져옵니다.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


이 페이지의 여백을 가져옵니다.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


MS OneNote 페이지가 여러 aps 페이지로 분할될 때, MS OneNote 페이지에서 페이지 끝 위치를 가져옵니다.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


최종 페이지 크기를 가져옵니다.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


MS OneNote 페이지가 여러 aps 페이지로 분할될 때, MS OneNote 페이지에서 페이지 시작 위치를 가져옵니다.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


이 페이지의 모든 노드를 순회하는 열거자를 반환합니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - 해당 `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


열거자를 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - 해당 `IEnumerator`.
