---
title: "PageHistory"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "페이지 기록을 나타냅니다."
type: docs
weight: 70
url: /ko/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

페이지 기록을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | 새 `PageHistory` 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | `PageHistory`의 끝에 페이지 버전을 추가합니다. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | `PageHistory`의 끝에 페이지 버전들을 추가합니다. |
| [clear()](#clear--) | 페이지 기록을 지웁니다. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | 페이지 기록에 페이지 버전이 포함되어 있는지 확인합니다. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | 페이지 버전을 배열에 복사하고, 특정 인덱스에서 시작합니다.. |
| [getCurrent()](#getCurrent--) | 현재 페이지 버전을 가져옵니다. |
| [get_Item(int index)](#get-Item-int-) | 지정된 인덱스의 `PageHistory`에서 페이지 버전을 가져오거나 설정합니다. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | 페이지 기록에서 특정 페이지 버전의 인덱스를 결정합니다. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | 페이지 버전을 페이지 기록에 삽입합니다. |
| [isReadOnly()](#isReadOnly--) | 페이지 기록이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [iterator()](#iterator--) | `PageHistory`의 자식 노드를 순회하는 열거자를 반환합니다. |
| [removeAt(int index)](#removeAt-int-) | `PageHistory`의 지정된 인덱스에 있는 페이지 버전을 제거합니다. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | `PageHistory`에서 페이지 버전을 제거합니다. |
| [removeRange(int index, int count)](#removeRange-int-int-) | `PageHistory`에서 페이지 버전 범위를 제거합니다. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | 지정된 인덱스의 `PageHistory`에서 페이지 버전을 가져오거나 설정합니다. |
| [size()](#size--) | 페이지 기록에 있는 페이지 버전 수를 가져옵니다. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


새 `PageHistory` 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | 현재 페이지 버전. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


`PageHistory`의 끝에 페이지 버전을 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | 페이지 버전. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


`PageHistory`의 끝에 페이지 버전들을 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 항목 | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | 페이지 버전의 `IEnumerable\{Page\}` 컬렉션. |

### clear() {#clear--}
```
public void clear()
```


페이지 기록을 지웁니다.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


페이지 기록에 페이지 버전이 포함되어 있는지 확인합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | 페이지 버전. |

**Returns:**
boolean - `bool`입니다.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


페이지 버전을 배열에 복사하고, 특정 인덱스에서 시작합니다..

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | 대상 배열. |
| arrayIndex | int | 배열 인덱스. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


현재 페이지 버전을 가져옵니다.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


지정된 인덱스의 `PageHistory`에서 페이지 버전을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| index | int | 인덱스. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


페이지 기록에서 특정 페이지 버전의 인덱스를 결정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | 페이지 버전. |

**Returns:**
int - `int`입니다.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


페이지 버전을 페이지 기록에 삽입합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| index | int | 인덱스. |
| item | [Page](../../com.aspose.note/page) | 페이지 버전. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


페이지 기록이 읽기 전용인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


`PageHistory`의 자식 노드를 순회하는 열거자를 반환합니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


`PageHistory`의 지정된 인덱스에 있는 페이지 버전을 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| index | int | 인덱스. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


`PageHistory`에서 페이지 버전을 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | 페이지 버전. |

**Returns:**
boolean - `bool`입니다.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


`PageHistory`에서 페이지 버전 범위를 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| index | int | 인덱스. |
| count | int | 카운트입니다. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


지정된 인덱스의 `PageHistory`에서 페이지 버전을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| index | int | 인덱스. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


페이지 기록에 있는 페이지 버전 수를 가져옵니다.

**Returns:**
int
