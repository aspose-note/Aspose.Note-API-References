---
title: OneSaveOptions.DocumentPassword
second_title: Справочник по API Aspose.Note для .NET
description: OneSaveOptions свойство. Получает или задает пароль для шифрования содержимого документа.
type: docs
weight: 20
url: /ru/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Получает или задает пароль для шифрования содержимого документа.

```csharp
public string DocumentPassword { get; set; }
```

### Примеры

Показывает, как сохранить документ с шифрованием.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Смотрите также

* class [OneSaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../onesaveoptions/)
* сборка [Aspose.Note](../../../)


