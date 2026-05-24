---
title: "PdfSaveOptions"
second_title: "Aspose.Note for Java API 参考"
description: "允许在将文档页面渲染为 PDF 时指定其他选项。"
type: docs
weight: 77
url: /zh/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

允许在将文档页面渲染为 PDF 时指定其他选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | 初始化 `PdfSaveOptions` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | 获取应用于 PDF 文件中图像的压缩类型。 |
| [getJpegQuality()](#getJpegQuality--) | 获取决定 PDF 文档中 JPEG 图像质量的值。 |
| [getPageSettings()](#getPageSettings--) | 获取或设置文档中每页的页面设置。 |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | 获取或设置用于页面拆分的算法。 |
| [setImageCompression(int value)](#setImageCompression-int-) | 设置应用于 PDF 文件中图像的压缩类型。 |
| [setJpegQuality(int value)](#setJpegQuality-int-) | 设置决定 PDF 文档中 JPEG 图像质量的值。 |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | 获取或设置文档中每页的页面设置。 |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | 获取或设置用于页面拆分的算法。 |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


初始化 `PdfSaveOptions` 类的新实例。

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


获取应用于 PDF 文件中图像的压缩类型。

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


获取决定 PDF 文档中 JPEG 图像质量的值。该值范围为 0 到 100，其中 0 表示质量最差但压缩最大，100 表示质量最佳但压缩最小。

--------------------

默认值为 90。

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


获取或设置文档中每页的页面设置。默认情况下取决于 CurrentUICulture，\*US 文化使用信纸设置，其他使用 A4 设置。

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


获取或设置用于页面拆分的算法。

值：`PageSplittingAlgorithm`。

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


设置应用于 PDF 文件中图像的压缩类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


设置决定 PDF 文档中 JPEG 图像质量的值。该值范围为 0 到 100，其中 0 表示质量最差但压缩最大，100 表示质量最佳但压缩最小。

--------------------

默认值为 90。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


获取或设置文档中每页的页面设置。默认情况下取决于 CurrentUICulture，\*US 文化使用信纸设置，其他使用 A4 设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


获取或设置用于页面拆分的算法。

值：`PageSplittingAlgorithm`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

