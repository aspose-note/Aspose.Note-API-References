---
title: Document.Document
second_title: .NET API 참조용 Aspose.Note
description: Document 건설자. 의 새 인스턴스를 초기화합니다.Document class. 빈 OneNote 문서를 만듭니다.
type: docs
weight: 10
url: /ko/net/aspose.note/document/document/
---
## Document() {#constructor}

의 새 인스턴스를 초기화합니다.[`Document`](../) class. 빈 OneNote 문서를 만듭니다.

```csharp
public Document()
```

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

의 새 인스턴스를 초기화합니다.[`Document`](../) class. 파일에서 기존 OneNote 문서를 엽니다.

```csharp
public Document(string filePath)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일 경로. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 문서 형식이 인식되지 않거나 지원되지 않습니다. |
| [FileCorruptedException](../../filecorruptedexception/) | 문서가 손상된 것 같으며 로드할 수 없습니다. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 문서가 암호화되어 있고 열려면 암호가 필요하지만 잘못된 암호를 제공했습니다. |
| InvalidOperationException | 문서에 문제가 있어 Aspose.Note 개발자에게 보고해야 합니다. |
| IOException | 입/출력 예외가 있습니다. |

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

의 새 인스턴스를 초기화합니다.[`Document`](../)class. 파일에서 기존 OneNote 문서를 엽니다. 암호화 암호와 같은 추가 옵션을 지정할 수 있습니다.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일 경로. |
| loadOptions | LoadOptions | 문서를 로드하는 데 사용되는 옵션입니다. null일 수 있습니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 문서 형식이 인식되지 않거나 지원되지 않습니다. |
| [FileCorruptedException](../../filecorruptedexception/) | 문서가 손상된 것 같으며 로드할 수 없습니다. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 문서가 암호화되어 있고 열려면 암호가 필요하지만 잘못된 암호를 제공했습니다. |
| InvalidOperationException | 문서에 문제가 있어 Aspose.Note 개발자에게 보고해야 합니다. |
| IOException | 입/출력 예외가 있습니다. |

### 또한보십시오

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`Document`](../) class. 스트림에서 기존 OneNote 문서를 엽니다.

```csharp
public Document(Stream inStream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| inStream | Stream | 스트림. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 문서 형식이 인식되지 않거나 지원되지 않습니다. |
| [FileCorruptedException](../../filecorruptedexception/) | 문서가 손상된 것 같으며 로드할 수 없습니다. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 문서가 암호화되어 있고 열려면 암호가 필요하지만 잘못된 암호를 제공했습니다. |
| InvalidOperationException | 문서에 문제가 있어 Aspose.Note 개발자에게 보고해야 합니다. |
| IOException | 입/출력 예외가 있습니다. |
| ArgumentException | 스트림이 읽기를 지원하지 않거나 null이거나 이미 닫혀 있습니다. |

### 또한보십시오

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

의 새 인스턴스를 초기화합니다.[`Document`](../) class. 스트림에서 기존 OneNote 문서를 엽니다. 암호화 암호와 같은 추가 옵션을 지정할 수 있습니다.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| inStream | Stream | 스트림. |
| loadOptions | LoadOptions | 문서를 로드하는 데 사용되는 옵션입니다. null일 수 있습니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 문서 형식이 인식되지 않거나 지원되지 않습니다. |
| [FileCorruptedException](../../filecorruptedexception/) | 문서가 손상된 것 같으며 로드할 수 없습니다. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 문서가 암호화되어 있고 열려면 암호가 필요하지만 잘못된 암호를 제공했습니다. |
| InvalidOperationException | 문서에 문제가 있어 Aspose.Note 개발자에게 보고해야 합니다. |
| IOException | 입/출력 예외가 있습니다. |
| ArgumentException | 스트림이 읽기를 지원하지 않거나 null이거나 이미 닫혀 있습니다. |

### 또한보십시오

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


