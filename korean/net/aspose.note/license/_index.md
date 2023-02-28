---
title: Class License
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.License 수업. 구성 요소에 라이선스를 부여하는 방법을 제공합니다.
type: docs
weight: 310
url: /ko/net/aspose.note/license/
---
## License class

구성 요소에 라이선스를 부여하는 방법을 제공합니다.

```csharp
public class License
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [License](license/)() | 기본 생성자입니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | 구성 요소에 라이선스를 부여합니다. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | 구성 요소에 라이선스를 부여합니다. |

### 예

파일에서 Aspose.Note용 라이선스를 로드하는 방법을 보여줍니다.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

스트림에서 Aspose.Note용 라이선스를 로드하는 방법을 보여줍니다.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

포함된 파일 리소스에서 Aspose.Note용 라이선스를 로드하는 방법을 보여줍니다.

```csharp
// 라이선스 클래스 인스턴스화
Aspose.Note.License license = new Aspose.Note.License();

// 어셈블리에 포함된 라이선스 파일의 이름만 전달
license.SetLicense("Aspose.Note.lic");
```

### 또한보십시오

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


