# AWSKRUG 홈페이지
본 페이지는 AWSKRUG의 Single Page Application으로 awskr.org의 첫화면입니다. 필요한 정보가 있으시면 업데이트 하시기 바랍니다.
- 홈페이지: https://www.awskr.org
- 관리자: contact@awskr.org

## 발표자 인증서 추가하기
AWSKRUG 소모임 발표자를 위한 디지털 인증서를 발급할 수 있습니다.

### 1. 인증서 데이터 파일 생성
`/speakers` 폴더에 `{연도}-{번호}.json` 형식으로 파일을 생성합니다.

**파일명 예시**: `2025-001.json`

**파일 내용**:
```json
{
    "id": "2025-001",
    "name": "홍길동",
    "role": "Speaker",
    "event": "AWSKRUG 데이터 소모임",
    "date": "2025-09-18",
    "title": "발표 제목",
    "url": "https://example.com/presentation", // url 필드가 있으면 발표 제목이 클릭 가능한 링크로 표시됩니다.
    "description": "In recognition of your valuable contribution as a speaker at AWSKRUG 데이터 소모임."
}
```

### 2. 인증서 URL
생성된 인증서는 다음 URL로 접근할 수 있습니다:

```
https://www.awskr.org/speakers/?id={인증서ID}
```

**예시**:
- `https://www.awskr.org/speakers/?id=2025-001`