---
title: License.SetLicense
second_title: .NET API 참조용 Aspose.Page
description: License 방법. 구성 요소에 라이선스를 부여합니다.
type: docs
weight: 30
url: /ko/net/aspose.page/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

구성 요소에 라이선스를 부여합니다.

```csharp
public void SetLicense(string licenseName)
```

### 비고

다음 위치에서 라이센스를 찾으려고 시도합니다.

1. 명시적 경로.

2. 컴포넌트 어셈블리의 폴더.

3. 클라이언트의 호출 어셈블리 폴더.

4. 엔트리 어셈블리의 폴더.

5. 클라이언트의 호출 어셈블리에 포함된 리소스.

**메모:**.NET Compact Framework에서는 다음 위치에서만 라이선스를 찾으려고 시도합니다.

1. 명시적 경로.

2. 클라이언트의 호출 어셈블리에 포함된 리소스.

2. 구성 요소 jar 파일의 폴더.

### 예

이 예에서는 가 포함된 폴더에서 MyLicense.lic 라는 라이선스 파일을 찾으려고 시도합니다. 호출 어셈블리가 포함된 폴더의 구성 요소, 항목 어셈블리의 폴더 및 호출 어셈블리의 포함 리소스.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

구성 요소 jar 파일:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

전체 또는 짧은 파일 이름일 수 있습니다. 또는 임베디드 리소스의 이름. 평가 모드로 전환하려면 빈 문자열을 사용하십시오.

### 또한보십시오

* class [License](../)
* 네임스페이스 [Aspose.Page](../../license/)
* 집회 [Aspose.Page](../../../)

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

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### 또한보십시오

* class [License](../)
* 네임스페이스 [Aspose.Page](../../license/)
* 집회 [Aspose.Page](../../../)


