---
title: "IFontsSubsystem"
second_title: "Aspose.Note for Java API-referentie"
description: "Implementeer deze interface als je wilt bepalen hoe Aspose.Note lettertypen ophaalt bij het opslaan van een document."
type: docs
weight: 12
url: /nl/java/com.aspose.note.fonts/ifontssubsystem/
---
```
public interface IFontsSubsystem
```

Implementeer deze interface als je wilt bepalen hoe Aspose.Note lettertypen ophaalt bij het opslaan van een document.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Haalt lettertype op. |
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public abstract Font getFontFamily(String fontName)
```


Haalt lettertype op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fontName | java.lang.String | De lettertype‑naam. |

**Returns:**
java.awt.Font - Het lettertype.
