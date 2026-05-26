---
title: "License"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "구성 요소를 라이선스하는 메서드를 제공합니다."
type: docs
weight: 44
url: /ko/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

구성 요소를 라이선스하는 메서드를 제공합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [License()](#License--) | 이 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | 현재 스레드에 대한 라이선스 컨텍스트를 재설정합니다. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | 구성 요소에 라이선스를 적용합니다. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | 구성 요소에 라이선스를 적용합니다. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | 구성 요소에 라이선스를 적용합니다. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | 현재 스레드에 대한 라이선스 컨텍스트를 설정합니다. |
### License() {#License--}
```
public License()
```


이 클래스의 새 인스턴스를 초기화합니다.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


현재 스레드에 대한 라이선스 컨텍스트를 재설정합니다.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


구성 요소에 라이선스를 적용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| licenseFile | java.io.File | 라이선스 파일`System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


구성 요소에 라이선스를 적용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 스트림 | java.io.InputStream | 라이선스를 포함하는 스트림입니다. |

--------------------

`

이 메서드를 사용하여 스트림에서 라이선스를 로드합니다.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


구성 요소에 라이선스를 적용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | licenseName | java.lang.String | 전체 또는 짧은 파일 이름` 또는 포함된 리소스의 이름`이 될 수 있습니다. 평가 모드로 전환하려면 빈 문자열을 사용하십시오. |

--------------------

`

다음 위치에서 라이선스를 찾으려고 시도합니다:

` `

1. 명시적 경로.

` `

2. Aspose 구성 요소 어셈블리를 포함하는 폴더.

3. 클라이언트의 호출 어셈블리를 포함하는 폴더.

4. 엔트리(시작) 어셈블리를 포함하는 폴더.

5. 클라이언트의 호출 어셈블리 내에 포함된 리소스.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. 명시적 경로.

2. 클라이언트의 호출 어셈블리 내에 포함된 리소스.

` `

2. Aspose 구성 요소 JAR 파일을 포함하는 폴더.

3. 클라이언트의 호출 JAR 파일을 포함하는 폴더.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


현재 스레드에 대한 라이선스 컨텍스트를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 라이선스를 포함하는 스트림입니다. |

