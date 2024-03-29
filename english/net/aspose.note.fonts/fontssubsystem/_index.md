---
title: Class FontsSubsystem
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Fonts.FontsSubsystem class. Base class implementing Aspose.Note.Fonts.IFontsSubsystem interface. Provides functionality for default font and fonts substitutions. Override Aspose.Note.Fonts.FontsSubsystem.FetchFontFamily protected member function in a derived class to implement logic for retrieving of FontFamily object
type: docs
weight: 110
url: /net/aspose.note.fonts/fontssubsystem/
---
## FontsSubsystem class

Base class implementing Aspose.Note.Fonts.IFontsSubsystem interface. Provides functionality for default font and font's substitutions. Override Aspose.Note.Fonts.FontsSubsystem.FetchFontFamily protected member function in a derived class to implement logic for retrieving of FontFamily object.

```csharp
public abstract class FontsSubsystem : IFontsSubsystem
```

## Properties

| Name | Description |
| --- | --- |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Gets or sets default font. |

## Methods

| Name | Description |
| --- | --- |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont)(Stream) | Add the font. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_2)(string) | Add the font. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_1)(Stream, string) | Add the font. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Adds font substitution. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Gets font family. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Loads all TrueType fonts from specified folder to internal collection. |

### See Also

* interface [IFontsSubsystem](../ifontssubsystem/)
* namespace [Aspose.Note.Fonts](../../aspose.note.fonts/)
* assembly [Aspose.Note](../../)


