---
title: "ExtendedApsNode"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "표준 ApsNode의 래퍼를 나타내며, 일부 그리기 동작을 확장합니다."
type: docs
weight: 26
url: /ko/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

표준 ApsNode에 대한 래퍼를 나타내며, 일부 그리기 동작을 확장합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | 주어진 `compositeNode`에 이 노드를 추가합니다. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 평면 변환을 적용하여 노드를 x 및 y 평면으로 이동시킵니다. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | 노드에 스케일링을 적용합니다. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | 노드 하단의 y 좌표를 가져오거나 설정합니다. |
| [getCopy()](#getCopy--) | 이 노드의 전체 복사본을 생성합니다. |
| [getOrigin()](#getOrigin--) | 노드의 원점을 가져오거나 설정합니다. |
| [getSize()](#getSize--) | 노드의 크기를 가져오거나 설정합니다. |
| [getTop()](#getTop--) | 노드 상단의 y 좌표를 가져오거나 설정합니다. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


주어진 `compositeNode`에 이 노드를 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


평면 변환을 적용하여 노드를 x 및 y 평면으로 이동시킵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


노드에 스케일링을 적용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| scaleTransform | float | 변환에 대한 스케일 계수입니다. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


노드 하단의 y 좌표를 가져오거나 설정합니다.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


이 노드의 전체 복사본을 생성합니다.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


노드의 원점을 가져오거나 설정합니다.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


노드의 크기를 가져오거나 설정합니다.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


노드 상단의 y 좌표를 가져오거나 설정합니다.

**Returns:**
float
