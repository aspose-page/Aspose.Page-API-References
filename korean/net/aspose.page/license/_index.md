---
title: Class License
second_title: .NET API 참조용 Aspose.Page
description: Aspose.Page.License 수업. 구성 요소에 라이선스를 부여하는 방법을 제공합니다.
type: docs
weight: 270
url: /ko/net/aspose.page/license/
---
## License class

구성 요소에 라이선스를 부여하는 방법을 제공합니다.

```csharp
public class License
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [License](license/)() | 이 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Embedded](../../aspose.page/license/embedded/) { get; set; } | 라이선스 번호가 임베디드 리소스로 추가되었습니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [SetLicense](../../aspose.page/license/setlicense/#setlicense)(Stream) | 구성 요소에 라이선스를 부여합니다. |
| [SetLicense](../../aspose.page/license/setlicense/#setlicense_1)(string) | 구성 요소에 라이선스를 부여합니다. |

### 예

이 예에서는 가 포함된 폴더에서 MyLicense.lic 라는 라이선스 파일을 찾으려고 시도합니다. 호출 어셈블리가 포함된 폴더의 구성 요소, 항목 어셈블리의 폴더 및 호출 어셈블리의 포함 리소스.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

구성 요소 jar 파일:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### 또한보십시오

* 네임스페이스 [Aspose.Page](../../aspose.page/)
* 집회 [Aspose.Page](../../)


