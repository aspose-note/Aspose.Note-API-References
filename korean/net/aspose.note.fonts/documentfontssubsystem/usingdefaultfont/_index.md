---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: .NET API 참조용 Aspose.Note
description: DocumentFontsSubsystem 방법. 지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 만듭니다.
type: docs
weight: 30
url: /ko/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 만듭니다.

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontName | String | 기본 글꼴 이름입니다. |
| fontsSubstitutions | Dictionary`2 | 글꼴 대체. |

### 반환 값

[`DocumentFontsSubsystem`](../) .

### 예

지정된 기본 글꼴을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 문서를 PDF로 저장
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

### 또한보십시오

* class [DocumentFontsSubsystem](../)
* 네임스페이스 [Aspose.Note.Fonts](../../documentfontssubsystem/)
* 집회 [Aspose.Note](../../../)


