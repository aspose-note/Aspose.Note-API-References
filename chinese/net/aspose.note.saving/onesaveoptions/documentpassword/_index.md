---
title: "OneSaveOptions.DocumentPassword"
second_title: "Aspose.Note for .NET API 参考"
description: "OneSaveOptions 属性。获取或设置用于加密文档内容的密码"
type: docs
weight: 20
url: /zh/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

获取或设置用于加密文档内容的密码。

```csharp
public string DocumentPassword { get; set; }
```

## 示例

展示如何使用加密保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### 另请参阅

* class [OneSaveOptions](../)
* namespace [Aspose.Note.Saving](../../onesaveoptions/)
* assembly [Aspose.Note](../../../)


