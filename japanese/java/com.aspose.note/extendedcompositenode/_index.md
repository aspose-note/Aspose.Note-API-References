---
title: "ExtendedCompositeNode"
second_title: "Aspose.Note for Java API リファレンス"
description: "複数の IExtendedApsNode インスタンスを結合します。"
type: docs
weight: 29
url: /ja/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

`IExtendedApsNode` インスタンスをいくつか組み合わせます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | `ExtendedCompositeNode` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | `extendedApsNode` をノードの内部リストに追加します。 |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | このノードを指定された `compositeNode` に追加します。 |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 平面変換を適用し、ノードを x および y 平面で移動させます。 |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | ノードにスケーリングを適用します。 |
| [getApsNodes()](#getApsNodes--) | この `ExtendedCompositeNode` に結合されたすべての `IExtendedApsNode` インスタンスを取得します。 |
| [getCopy()](#getCopy--) | このノードの完全なコピーを作成します。 |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


`ExtendedCompositeNode` クラスの新しいインスタンスを初期化します。

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


`extendedApsNode` をノードの内部リストに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


このノードを指定された `compositeNode` に追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


平面変換を適用し、ノードを x および y 平面で移動させます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


ノードにスケーリングを適用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| scaleTransform | float | 変換のスケール係数です。 |

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


この `ExtendedCompositeNode` に結合されたすべての `IExtendedApsNode` インスタンスを取得します。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


このノードの完全なコピーを作成します。

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
