---
title: "License"
second_title: "Справочник API Aspose.Note for Java"
description: "Предоставляет методы лицензирования компонента."
type: docs
weight: 44
url: /ru/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Предоставляет методы лицензирования компонента.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [License()](#License--) | Инициализирует новый экземпляр этого класса. |
## Методы

| Метод | Описание |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Сбрасывает контекст лицензии для текущего потока. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Лицензирует компонент. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Лицензирует компонент. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Лицензирует компонент. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Устанавливает контекст лицензии для текущего потока. |
### License() {#License--}
```
public License()
```


Инициализирует новый экземпляр этого класса.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Сбрасывает контекст лицензии для текущего потока.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Лицензирует компонент.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| licenseFile | java.io.File | Файл лицензии `System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Лицензирует компонент.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | поток | java.io.InputStream | Поток, содержащий лицензию. |

--------------------

`

Используйте этот метод для загрузки лицензии из потока.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Лицензирует компонент.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | licenseName | java.lang.String | Может быть полным или коротким именем файла` или именем встроенного ресурса`. Используйте пустую строку для перехода в режим оценки. |

--------------------

`

Пытается найти лицензию в следующих местах:

` `

1. Явный путь.

` `

2. Папка, содержащая сборку компонента Aspose.

3. Папка, содержащая вызывающую сборку клиента.

4. Папка, содержащая входную (запускную) сборку.

5. Встроенный ресурс в вызывающей сборке клиента.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Явный путь.

2. Встроенный ресурс в вызывающей сборке клиента.

` `

2. Папка, содержащая JAR‑файл компонента Aspose.

3. Папка, содержащая JAR‑файл, вызываемый клиентом.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Устанавливает контекст лицензии для текущего потока.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток, содержащий лицензию. |

