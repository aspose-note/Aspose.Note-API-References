---
title: "ExtendedApsGlyphs"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "표준 ApsGlyphs에 대한 래퍼를 나타내며, 일부 그리기 동작을 확장합니다."
type: docs
weight: 24
url: /ko/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

표준 ApsGlyphs에 대한 래퍼를 나타내며, 일부 그리기 동작을 확장합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | 새 `ExtendedApsGlyphs` 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | 주어진 `compositeNode`에 이 노드를 추가합니다. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 평면 변환을 적용하여 노드를 x 및 y 평면으로 이동시킵니다. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | 글리프에 스케일링을 적용합니다. |
| [getBottom()](#getBottom--) | 글리프의 하단을 가져옵니다. |
| [getCopy()](#getCopy--) | 글리프의 복사본을 가져옵니다. |
| [getOrigin()](#getOrigin--) | 원점을 가져옵니다. |
| [getSize()](#getSize--) | 크기를 가져옵니다. |
| [getTop()](#getTop--) | 상단을 가져옵니다. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


새 `ExtendedApsGlyphs` 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | 원본 aps 글리프입니다. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


주어진 `compositeNode`에 이 노드를 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


평면 변환을 적용하여 노드를 x 및 y 평면으로 이동시킵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


글리프에 스케일링을 적용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| scaleTransform | float | 변환에 대한 스케일 계수입니다. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


글리프의 하단을 가져옵니다.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


글리프의 복사본을 가져옵니다.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


원점을 가져옵니다.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


크기를 가져옵니다.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


상단을 가져옵니다.

**Returns:**
float
