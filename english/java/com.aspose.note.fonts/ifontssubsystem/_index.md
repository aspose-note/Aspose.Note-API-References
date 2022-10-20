---
title: IFontsSubsystem
second_title: Aspose.Note for Java API Reference
description: Implement this interface if you want to control how Aspose.Note retrieves fonts when saving a document.
type: docs
weight: 12
url: /java/com.aspose.note.fonts/ifontssubsystem/
---
```
public interface IFontsSubsystem
```

Implement this interface if you want to control how Aspose.Note retrieves fonts when saving a document.
## Methods

| Method | Description |
| --- | --- |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Gets font. |
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public abstract Font getFontFamily(String fontName)
```


Gets font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | java.lang.String | The font name. |

**Returns:**
java.awt.Font - The Font.
