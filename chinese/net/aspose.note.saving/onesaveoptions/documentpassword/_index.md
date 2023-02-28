---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note for .NET API 参考
description: OneSaveOptions 财产. 获取或设置用于加密文档内容的密码
type: docs
weight: 20
url: /zh/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

获取或设置用于加密文档内容的密码。

```csharp
public string DocumentPassword { get; set; }
```

### 例子

显示如何使用加密保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### 也可以看看

* class [OneSaveOptions](../)
* 命名空间 [Aspose.Note.Saving](../../onesaveoptions/)
* 部件 [Aspose.Note](../../../)


