---
title: Class DocumentFontsSubsystem
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Fonts.DocumentFontsSubsystem 수업. Aspose.Note.Fonts.FontsSubsystem의 간단한 구현. 검색FontFamily OS. 의 객체
type: docs
weight: 100
url: /ko/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Aspose.Note.Fonts.FontsSubsystem의 간단한 구현. 검색FontFamily OS. 의 객체

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | 의 새 인스턴스를 초기화합니다.`DocumentFontsSubsystem` 클래스. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | 의 새 인스턴스를 초기화합니다.`DocumentFontsSubsystem` 클래스. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | 의 새 인스턴스를 초기화합니다.`DocumentFontsSubsystem` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | 정적 기본 인스턴스를 가져오거나 설정합니다. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | 기본 글꼴을 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | 지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 만듭니다. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | 지정된 파일의 글꼴을 기본값으로 사용하여 새 DocumentFontsSubsystem 인스턴스를 만듭니다. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | 지정된 스트림의 글꼴을 기본값으로 사용하여 새 DocumentFontsSubsystem 인스턴스를 만듭니다. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | 글꼴을 추가합니다. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | 글꼴을 추가합니다. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | 글꼴을 추가합니다. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | 글꼴 대체를 추가합니다. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | 글꼴 패밀리를 가져옵니다. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | 지정된 폴더에서 내부 컬렉션으로 모든 트루타입 글꼴을 로드합니다. |

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

파일의 기본 글꼴을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 문서를 PDF로 저장
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

스트림의 기본 글꼴을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 문서를 PDF로 저장
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### 또한보십시오

* class [FontsSubsystem](../fontssubsystem/)
* 네임스페이스 [Aspose.Note.Fonts](../../aspose.note.fonts/)
* 집회 [Aspose.Note](../../)


