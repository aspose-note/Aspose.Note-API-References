---
title: "Margins"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "노드 여백의 크기를 지정합니다."
type: docs
weight: 49
url: /ko/java/com.aspose.note/margins/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Margins extends Struct<Margins> implements System.IEquatable<Margins>
```

노드 여백의 크기를 지정합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Margins()](#Margins--) |  |
| [Margins(float left, float right, float top, float bottom)](#Margins-float-float-float-float-) | 지정된 왼쪽, 오른쪽, 위, 아래 여백을 사용하여 `Margins` 구조체의 새 인스턴스를 초기화합니다. |
## 필드

| 필드 | 설명 |
| --- | --- |
| [Empty](#Empty) | 빈 여백입니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [Clone()](#Clone--) |  |
| [CloneTo(Margins that)](#CloneTo-com.aspose.note.Margins-) |  |
| [clone()](#clone--) |  |
| [equals(Margins other)](#equals-com.aspose.note.Margins-) |  |
| [equals(Margins obj1, Margins obj2)](#equals-com.aspose.note.Margins-com.aspose.note.Margins-) |  |
| [equals(Object obj)](#equals-java.lang.Object-) | 두 `T:Margins` 구조가 같은지 테스트합니다. |
| [getBottom()](#getBottom--) | 아래쪽 여백 너비를 가져오거나 설정합니다. |
| [getLeft()](#getLeft--) | 왼쪽 여백 너비를 가져오거나 설정합니다. |
| [getRight()](#getRight--) | 오른쪽 여백 너비를 가져오거나 설정합니다. |
| [getTop()](#getTop--) | 위쪽 여백 너비를 가져오거나 설정합니다. |
| [op_Equality(Margins lhs, Margins rhs)](#op-Equality-com.aspose.note.Margins-com.aspose.note.Margins-) | 두 `T:Margins` 구조가 같은지 테스트합니다. |
| [op_Inequality(Margins lhs, Margins rhs)](#op-Inequality-com.aspose.note.Margins-com.aspose.note.Margins-) | 두 `T:Margins` 구조가 같지 않은지 테스트합니다. |
| [setBottom(float value)](#setBottom-float-) | 아래쪽 여백 너비를 가져오거나 설정합니다. |
| [setLeft(float value)](#setLeft-float-) | 왼쪽 여백 너비를 가져오거나 설정합니다. |
| [setRight(float value)](#setRight-float-) | 오른쪽 여백 너비를 가져오거나 설정합니다. |
| [setTop(float value)](#setTop-float-) | 위쪽 여백 너비를 가져오거나 설정합니다. |
### Margins() {#Margins--}
```
public Margins()
```


### Margins(float left, float right, float top, float bottom) {#Margins-float-float-float-float-}
```
public Margins(float left, float right, float top, float bottom)
```


지정된 왼쪽, 오른쪽, 위, 아래 여백을 사용하여 `Margins` 구조체의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 왼쪽 | float | 왼쪽 여백 너비입니다. |
| 오른쪽 | float | 오른쪽 여백 너비입니다. |
| 위쪽 | float | 위쪽 여백 너비입니다. |
| 아래쪽 | float | 하단 여백 너비입니다. |

### Empty {#Empty}
```
public static final Margins Empty
```


빈 여백입니다.

### Clone() {#Clone--}
```
public Margins Clone()
```




**Returns:**
[Margins](../../com.aspose.note/margins)
### CloneTo(Margins that) {#CloneTo-com.aspose.note.Margins-}
```
public void CloneTo(Margins that)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| that | [Margins](../../com.aspose.note/margins) |  |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object
### equals(Margins other) {#equals-com.aspose.note.Margins-}
```
public boolean equals(Margins other)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| other | [Margins](../../com.aspose.note/margins) |  |

**Returns:**
boolean
### equals(Margins obj1, Margins obj2) {#equals-com.aspose.note.Margins-com.aspose.note.Margins-}
```
public static boolean equals(Margins obj1, Margins obj2)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| obj1 | [Margins](../../com.aspose.note/margins) |  |
| obj2 | [Margins](../../com.aspose.note/margins) |  |

**Returns:**
boolean
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


두 `T:Margins` 구조가 같은지 테스트합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 임의 객체. |

**Returns:**
boolean - `bool`입니다.
### getBottom() {#getBottom--}
```
public float getBottom()
```


아래쪽 여백 너비를 가져오거나 설정합니다.

**Returns:**
float
### getLeft() {#getLeft--}
```
public float getLeft()
```


왼쪽 여백 너비를 가져오거나 설정합니다.

**Returns:**
float
### getRight() {#getRight--}
```
public float getRight()
```


오른쪽 여백 너비를 가져오거나 설정합니다.

**Returns:**
float
### getTop() {#getTop--}
```
public float getTop()
```


위쪽 여백 너비를 가져오거나 설정합니다.

**Returns:**
float
### op_Equality(Margins lhs, Margins rhs) {#op-Equality-com.aspose.note.Margins-com.aspose.note.Margins-}
```
public static boolean op_Equality(Margins lhs, Margins rhs)
```


두 `T:Margins` 구조가 같은지 테스트합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| lhs | [Margins](../../com.aspose.note/margins) | `T:Margins` 구조체. |
| rhs | [Margins](../../com.aspose.note/margins) | 비교 대상인 `T:Margins` 구조체. |

**Returns:**
boolean - `bool`입니다.
### op_Inequality(Margins lhs, Margins rhs) {#op-Inequality-com.aspose.note.Margins-com.aspose.note.Margins-}
```
public static boolean op_Inequality(Margins lhs, Margins rhs)
```


두 `T:Margins` 구조가 같지 않은지 테스트합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| lhs | [Margins](../../com.aspose.note/margins) | `T:Margins` 구조체. |
| rhs | [Margins](../../com.aspose.note/margins) | 비교 대상인 `T:Margins` 구조체. |

**Returns:**
boolean - `bool`입니다.
### setBottom(float value) {#setBottom-float-}
```
public void setBottom(float value)
```


아래쪽 여백 너비를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setLeft(float value) {#setLeft-float-}
```
public void setLeft(float value)
```


왼쪽 여백 너비를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setRight(float value) {#setRight-float-}
```
public void setRight(float value)
```


오른쪽 여백 너비를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setTop(float value) {#setTop-float-}
```
public void setTop(float value)
```


위쪽 여백 너비를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

