---
title: "LoadOptions"
second_title: "Справочник API Aspose.Note for Java"
description: "Параметры, используемые для загрузки документа."
type: docs
weight: 46
url: /ru/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Параметры, используемые для загрузки документа.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Инициализирует новый экземпляр класса `LoadOptions`. |
## Методы

| Метод | Описание |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Получает или задает пароль для зашифрованного содержимого документа. |
| [getLoadHistory()](#getLoadHistory--) | Получает или задает значение, указывающее, должен ли загрузчик документов игнорировать историю. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Получает или задает пароль для зашифрованного содержимого документа. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Получает или задает значение, указывающее, должен ли загрузчик документов игнорировать историю. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Инициализирует новый экземпляр класса `LoadOptions`.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Получает или задает пароль для зашифрованного содержимого документа. Значение игнорируется, если документ не защищён паролем.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Получает или задает значение, указывающее, должен ли загрузчик документов игнорировать историю. Используйте эту опцию для снижения использования памяти и процессора. Значение по умолчанию — `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Получает или задает пароль для зашифрованного содержимого документа. Значение игнорируется, если документ не защищён паролем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Получает или задает значение, указывающее, должен ли загрузчик документов игнорировать историю. Используйте эту опцию для снижения использования памяти и процессора. Значение по умолчанию — `true`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

