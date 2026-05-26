---
title: "ExtendedCompositeNode"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "여러 IExtendedApsNode 인스턴스를 결합합니다."
type: docs
weight: 29
url: /ko/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

`IExtendedApsNode` 인스턴스를 여러 개 결합합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | 새 `ExtendedCompositeNode` 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | `extendedApsNode`를 내부 노드 목록에 추가합니다. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | 주어진 `compositeNode`에 이 노드를 추가합니다. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 평면 변환을 적용하여 노드를 x 및 y 평면으로 이동시킵니다. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | 노드에 스케일링을 적용합니다. |
| [getApsNodes()](#getApsNodes--) | 이 `ExtendedCompositeNode`에 결합된 모든 `IExtendedApsNode` 인스턴스를 가져옵니다. |
| [getCopy()](#getCopy--) | 이 노드의 전체 복사본을 생성합니다. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


새 `ExtendedCompositeNode` 클래스 인스턴스를 초기화합니다.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


`extendedApsNode`를 내부 노드 목록에 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

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


노드에 스케일링을 적용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| scaleTransform | float | 변환에 대한 스케일 계수입니다. |

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


이 `ExtendedCompositeNode`에 결합된 모든 `IExtendedApsNode` 인스턴스를 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


이 노드의 전체 복사본을 생성합니다.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
