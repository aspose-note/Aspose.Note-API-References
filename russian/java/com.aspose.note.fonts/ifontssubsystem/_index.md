---
title: "IFontsSubsystem"
second_title: "Справочник API Aspose.Note for Java"
description: "Реализуйте этот интерфейс, если хотите контролировать, как Aspose.Note получает шрифты при сохранении документа."
type: docs
weight: 12
url: /ru/java/com.aspose.note.fonts/ifontssubsystem/
---
```
public interface IFontsSubsystem
```

Реализуйте этот интерфейс, если хотите контролировать, как Aspose.Note получает шрифты при сохранении документа.
## Методы

| Метод | Описание |
| --- | --- |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Получает шрифт. |
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public abstract Font getFontFamily(String fontName)
```


Получает шрифт.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontName | java.lang.String | Имя шрифта. |

**Returns:**
java.awt.Font - Шрифт.
