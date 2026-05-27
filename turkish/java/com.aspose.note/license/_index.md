---
title: "License"
second_title: "Aspose.Note for Java API Referansı"
description: "Bileşeni lisanslamak için yöntemler sağlar."
type: docs
weight: 44
url: /tr/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Bileşeni lisanslamak için yöntemler sağlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [License()](#License--) | Bu sınıfın yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Geçerli iş parçacığı için lisans bağlamını sıfırlar. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Bileşeni lisanslar. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Bileşeni lisanslar. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Bileşeni lisanslar. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Geçerli iş parçacığı için lisans bağlamını ayarlar. |
### License() {#License--}
```
public License()
```


Bu sınıfın yeni bir örneğini başlatır.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Geçerli iş parçacığı için lisans bağlamını sıfırlar.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Bileşeni lisanslar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| licenseFile | java.io.File | Lisans dosyası `System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Bileşeni lisanslar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | akış | java.io.InputStream | Lisansı içeren bir akış. |

--------------------

`

Bu yöntemi bir akıştan lisans yüklemek için kullanın.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Bileşeni lisanslar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | licenseName | java.lang.String | Tam veya kısa bir dosya adı` veya gömülü kaynağın adı` olabilir. Değerlendirme moduna geçmek için boş bir dize kullanın. |

--------------------

`

Lisansı aşağıdaki konumlarda bulmaya çalışır:

` `

1. Açık yol.

` `

2. Aspose bileşen derlemesini içeren klasör.

3. İstemcinin çağıran derlemesini içeren klasör.

4. Giriş (başlangıç) derlemesini içeren klasör.

5. İstemcinin çağıran derlemesindeki gömülü kaynak.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Açık yol.

2. İstemcinin çağıran derlemesindeki gömülü kaynak.

` `

2. Aspose bileşen JAR dosyasını içeren klasör.

3. İstemcinin çağıran JAR dosyasını içeren klasör.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Geçerli iş parçacığı için lisans bağlamını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Lisansı içeren bir akış. |

