---
title: License.SetLicense
second_title: .NET API 참조용 Aspose.Note
description: License 방법. 구성 요소에 라이선스를 부여합니다.
type: docs
weight: 20
url: /ko/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

구성 요소에 라이선스를 부여합니다.

```csharp
public void SetLicense(string licenseName)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| licenseName | String | 포함된 리소스의 전체 또는 짧은 파일 이름 또는 이름일 수 있습니다. 평가 모드로 전환하려면 빈 문자열을 사용하십시오. |

### 비고

다음 위치에서 라이센스를 찾으려고 시도합니다.

1. 명시적 경로.

2. Aspose 컴포넌트 어셈블리가 포함된 폴더.

3. 클라이언트의 호출 어셈블리가 포함된 폴더.

4. 항목(시작) 어셈블리가 포함된 폴더.

5. 클라이언트의 호출 어셈블리에 포함된 리소스.

**메모:**.NET Compact Framework에서는 다음 위치에서만 라이선스를 찾으려고 시도합니다.

1. 명시적 경로.

2. 클라이언트의 호출 어셈블리에 포함된 리소스.

### 예

파일에서 Aspose.Note용 라이선스를 로드하는 방법을 보여줍니다.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

포함된 파일 리소스에서 Aspose.Note용 라이선스를 로드하는 방법을 보여줍니다.

```csharp
// 라이선스 클래스 인스턴스화
Aspose.Note.License license = new Aspose.Note.License();

// 어셈블리에 포함된 라이선스 파일의 이름만 전달
license.SetLicense("Aspose.Note.lic");
```

### 또한보십시오

* class [License](../)
* 네임스페이스 [Aspose.Note](../../license/)
* 집회 [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

구성 요소에 라이선스를 부여합니다.

```csharp
public void SetLicense(Stream stream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 라이선스가 포함된 스트림입니다. |

### 비고

스트림에서 라이센스를 로드하려면 이 방법을 사용하십시오.

### 예

스트림에서 Aspose.Note용 라이선스를 로드하는 방법을 보여줍니다.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### 또한보십시오

* class [License](../)
* 네임스페이스 [Aspose.Note](../../license/)
* 집회 [Aspose.Note](../../../)


