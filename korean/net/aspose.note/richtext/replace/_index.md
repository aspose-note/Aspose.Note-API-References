---
title: RichText.Replace
second_title: .NET API 참조용 Aspose.Note
description: RichText 방법. 이 인스턴스에서 지정된 유니코드 문자의 모든 항목을 지정된 다른 유니코드 문자로 바꿉니다.
type: docs
weight: 200
url: /ko/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

이 인스턴스에서 지정된 유니코드 문자의 모든 항목을 지정된 다른 유니코드 문자로 바꿉니다.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| oldChar | Char | 이전 char. |
| newChar | Char | 새 문자입니다. |

### 반환 값

[`RichText`](../) .

### 또한보십시오

* class [RichText](../)
* 네임스페이스 [Aspose.Note](../../richtext/)
* 집회 [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

현재 인스턴스에서 지정된 문자열의 모든 발생을 다른 지정된 문자열로 바꿉니다.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| oldValue | String | 이전 값입니다. |
| newValue | String | 새 값입니다. |

### 반환 값

[`RichText`](../) .

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### 예

페이지의 텍스트를 통과하고 교체하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// 모든 RichText 노드 가져오기
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 도형의 텍스트 바꾸기
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// 지원되는 파일 형식으로 저장
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

템플릿에서 특수 텍스트 부분을 교체하여 새 문서를 생성하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// 템플릿 문서를 Aspose.Note에 로드합니다.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// 모든 템플릿 단어를 바꾸자
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### 또한보십시오

* class [RichText](../)
* 네임스페이스 [Aspose.Note](../../richtext/)
* 집회 [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

현재 인스턴스에서 지정된 문자열의 모든 항목을 지정된 스타일의 다른 지정된 문자열로 바꿉니다.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| oldValue | String | 이전 값입니다. |
| newValue | String | 새 값입니다. |
| style | TextStyle | 새 값의 스타일입니다. |

### 반환 값

[`RichText`](../) .

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### 또한보십시오

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* 네임스페이스 [Aspose.Note](../../richtext/)
* 집회 [Aspose.Note](../../../)


