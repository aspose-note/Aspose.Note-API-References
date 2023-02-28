---
title: Class FontsSubsystem
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Fonts.FontsSubsystem сорт. Базовый класс реализующий интерфейс Aspose.Note.Fonts.IFontsSubsystem. Предоставляет функциональные возможности для шрифта по умолчанию и замены шрифта. Переопределить защищенную функциючлен Aspose.Note.Fonts.FontsSubsystem.FetchFontFamily в производном классе для реализации логики полученияFontFamily объект.
type: docs
weight: 110
url: /ru/net/aspose.note.fonts/fontssubsystem/
---
## FontsSubsystem class

Базовый класс, реализующий интерфейс Aspose.Note.Fonts.IFontsSubsystem. Предоставляет функциональные возможности для шрифта по умолчанию и замены шрифта. Переопределить защищенную функцию-член Aspose.Note.Fonts.FontsSubsystem.FetchFontFamily в производном классе для реализации логики полученияFontFamily объект.

```csharp
public abstract class FontsSubsystem : IFontsSubsystem
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Получает или устанавливает шрифт по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont)(Stream) | Добавьте шрифт. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_2)(string) | Добавьте шрифт. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/#addfont_1)(Stream, string) | Добавьте шрифт. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Добавляет замену шрифта. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Получает семейство шрифтов. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Загружает все шрифты TrueType из указанной папки во внутреннюю коллекцию. |

### Смотрите также

* interface [IFontsSubsystem](../ifontssubsystem/)
* пространство имен [Aspose.Note.Fonts](../../aspose.note.fonts/)
* сборка [Aspose.Note](../../)


