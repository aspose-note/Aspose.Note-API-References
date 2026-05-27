---
title: "Page"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir sayfayı temsil eder."
type: docs
weight: 69
url: /tr/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Bir sayfayı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Page()](#Page--) | `Page` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [deepClone()](#deepClone--) | Sayfayı klonlar. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Sayfayı klonlar. |
| [getAuthor()](#getAuthor--) | Yazarı alır veya ayarlar. |
| [getBackgroundColor()](#getBackgroundColor--) | Sayfanın arka plan rengini alır veya ayarlar. |
| [getCreationTime()](#getCreationTime--) | Oluşturma zamanını alır veya ayarlar. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [getLevel()](#getLevel--) | Seviyeyi alır veya ayarlar. |
| [getMargin()](#getMargin--) | Kenar boşluğunu alır veya ayarlar. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Sayfa ve alt düğümleri için revizyon özetini alır veya ayarlar. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Editörde gösterilen sayfanın düzen boyutunu alır. |
| [getSizeType()](#getSizeType--) | Sayfanın boyut tipini alır veya ayarlar. |
| [getTitle()](#getTitle--) | Başlığı alır veya ayarlar. |
| [isConflictPage()](#isConflictPage--) | Bu sayfanın bir çakışma sayfası olup olmadığını gösteren değeri alır veya ayarlar. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Yazarı alır veya ayarlar. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Sayfanın arka plan rengini alır veya ayarlar. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Bu sayfanın bir çakışma sayfası olup olmadığını gösteren değeri alır veya ayarlar. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Oluşturma zamanını alır veya ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [setLevel(byte value)](#setLevel-byte-) | Seviyeyi alır veya ayarlar. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Kenar boşluğunu alır veya ayarlar. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Sayfa ve alt düğümleri için revizyon özetini alır veya ayarlar. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Editörde gösterilen sayfanın düzen boyutunu ayarlar. |
| [setSizeType(int value)](#setSizeType-int-) | Sayfanın boyut tipini alır veya ayarlar. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Başlığı alır veya ayarlar. |
### Page() {#Page--}
```
public Page()
```


`Page` sınıfının yeni bir örneğini başlatır.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Sayfayı klonlar.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Sayfayı klonlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cloneHistory | boolean | Sayfanın geçmişinin kopyalanıp kopyalanmayacağını belirtir.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Yazarı alır veya ayarlar.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Sayfanın arka plan rengini alır veya ayarlar.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Oluşturma zamanını alır veya ayarlar.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Seviyeyi alır veya ayarlar.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Kenar boşluğunu alır veya ayarlar.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Sayfa ve alt düğümleri için revizyon özetini alır veya ayarlar.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Editörde gösterilen sayfanın düzen boyutunu alır.

--------------------

Bu değer, belge açıldığında Microsoft OneNote uygulaması tarafından alt sayfa düzenini görüntülemek için kullanılır. Belgenin yazdırılmasını ve kaydedilmesini etkilemez. Page.SizeType özelliği PageSizeType.SizeByContent olarak ayarlandığında, bu özellik içeriğin gerçek boyutunu döndürür.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Sayfanın boyut tipini alır veya ayarlar.

--------------------

Varsayılan olarak, bir sayfa otomatik olarak yeniden boyutlandırılır. Varsayılan değer [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Başlığı alır veya ayarlar.

Değer: `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Bu sayfanın bir çakışma sayfası olup olmadığını gösteren değeri alır veya ayarlar.

--------------------

Çakışma sayfası, iki kullanıcının aynı içeriği güncellemeye çalışması durumunda ortaya çıkar. Bu durumda ilk kullanıcının değişiklikleri normal şekilde yazılır. Ancak diğer kullanıcının değişiklikleri birleştirilemez. Bu yüzden sadece bir sayfa kopyası oluşturulur ve çakışma olarak işaretlenir.

Bu sürümde çakışmalar, ilk kullanıcının değişiklikleri lehine çözülür. Bu nedenle belge çakışma sayfalarına sahipse, bu sayfalar geçmişte gösterilir ancak kaydetme sırasında atlanır. Bu bayrağı sıfırlayarak bu sayfaları normal sayfalar gibi geçmişte kaydetmek mümkündür.

Çakışma sayfası ile manipülasyon örneği, çevrimiçi belgelerde bulunabilir.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Yazarı alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Sayfanın arka plan rengini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Bu sayfanın bir çakışma sayfası olup olmadığını gösteren değeri alır veya ayarlar.

--------------------

Çakışma sayfası, iki kullanıcının aynı içeriği güncellemeye çalışması durumunda ortaya çıkar. Bu durumda ilk kullanıcının değişiklikleri normal şekilde yazılır. Ancak diğer kullanıcının değişiklikleri birleştirilemez. Bu yüzden sadece bir sayfa kopyası oluşturulur ve çakışma olarak işaretlenir.

Bu sürümde çakışmalar, ilk kullanıcının değişiklikleri lehine çözülür. Bu nedenle belge çakışma sayfalarına sahipse, bu sayfalar geçmişte gösterilir ancak kaydetme sırasında atlanır. Bu bayrağı sıfırlayarak bu sayfaları normal sayfalar gibi geçmişte kaydetmek mümkündür.

Çakışma sayfası ile manipülasyon örneği, çevrimiçi belgelerde bulunabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Oluşturma zamanını alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Seviyeyi alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Kenar boşluğunu alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Sayfa ve alt düğümleri için revizyon özetini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Editörde gösterilen sayfanın düzen boyutunu ayarlar.

--------------------

Bu değer, belge açıldığında Microsoft OneNote uygulaması tarafından alt sayfa düzenini görüntülemek için kullanılır. Belgenin yazdırılmasını ve kaydedilmesini etkilemez. Page.SizeType özelliği PageSizeType.SizeByContent olarak ayarlandığında, bu özellik içeriğin gerçek boyutunu döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Sayfanın boyut tipini alır veya ayarlar.

--------------------

Varsayılan olarak, bir sayfa otomatik olarak yeniden boyutlandırılır. Varsayılan değer [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Başlığı alır veya ayarlar.

Değer: `Title`.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

