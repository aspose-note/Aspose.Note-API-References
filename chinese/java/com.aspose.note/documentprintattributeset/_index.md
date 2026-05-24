---
title: "DocumentPrintAttributeSet"
second_title: "Aspose.Note for Java API 参考"
description: "表示具有用户友好界面的 AttributeSet 辅助类。"
type: docs
weight: 21
url: /zh/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

表示具有用户友好界面的 AttributeSet 辅助类。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | 初始化 `DocumentPrintAttributeSet` 的新实例。 |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | 初始化 `DocumentPrintAttributeSet` 的新实例。 |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | 初始化 `DocumentPrintAttributeSet` 的新实例。 |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | 初始化 `DocumentPrintAttributeSet` 的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | 设置一个值，指示文档是否已装订。 |
| [setCopies(int value)](#setCopies-int-) | 设置要打印的副本数量。 |
| [setDuplex(boolean value)](#setDuplex-boolean-) | 设置双面打印的打印机设置。 |
| [setLandscape(boolean value)](#setLandscape-boolean-) | 设置页面的方向。 |
| [setPrintRange(int page)](#setPrintRange-int-) | 设置要打印的单页。 |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | 设置要打印的页面范围。 |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | 要使用的打印机名称。 |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | 要使用的打印机名称。 |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


初始化 `DocumentPrintAttributeSet` 的新实例。默认情况下会打印文档的所有页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 副本 | int | 要打印的文档副本数量。 |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


初始化 `DocumentPrintAttributeSet` 的新实例。默认情况下会打印文档的所有页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称。 |
| 副本 | int | 要打印的文档副本数量。 |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


初始化 `DocumentPrintAttributeSet` 的新实例。默认情况下每页仅打印一份。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称。 |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


初始化 `DocumentPrintAttributeSet` 的新实例。默认情况下每页仅打印一份。

### getCopies() {#getCopies--}
```
public int getCopies()
```




**Returns:**
int
### getLandscape() {#getLandscape--}
```
public boolean getLandscape()
```




**Returns:**
boolean
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```




**Returns:**
java.lang.String
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


设置一个值，指示文档是否已装订。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | true 等价于 SheetCollate.COLLATED 的设置，false 等价于 SheetCollate.UNCOLLATED 的设置 |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


设置要打印的副本数量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要打印的副本数量。 |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


设置双面打印的打印机设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | true 等价于 Sides.DUPLEX 的设置，false 等价于 Sides.ONE\_SIDED 的设置 |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


设置页面的方向。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | true 等价于 OrientationRequested.LANDSCAPE 的设置，false 等价于 OrientationRequested.PORTRAIT 的设置 |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


设置要打印的单页。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 页面 | int | 要打印的页面。 |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


设置要打印的页面范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 从 | int | 第第一页。 |
| 至 | int | 最后一页。 |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


要使用的打印机名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称。 |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


要使用的打印机名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| printerName | java.lang.String | 打印机的名称。 |
| 区域设置 | java.util.Locale | printerName 的区域设置。 |

