https://www.awskr.org/speakers/{certification_id}

# 인증서 관련 요구사항 
- certification_id는 2025-014 (연도-번호) 형식으로 이루어져 있습니다.
- /speakers 폴더에 스피커 정보를 포함한 인증서 메타정보가 json으로 정의 되어 있음. 해당 json 파일을 읽어서 고유한 인증서 페이지를 생성함
    - json 예시
    ```
        {
            "id": "2025-014",
            "name": "소성운",
            "role": "Speaker",
            "event": "AWSKRUG AI엔지니어링 소모임",
            "date": "2025-12-22",
            "title": "Certificate of Appreciation",
            "description": "In recognition of your valuable contribution as a speaker at AWSKRUG AI엔지니어링 소모임."
        }
    ```
- 인증서 페이지에는 Add to LinkedIn 버튼이 있으며, 이 버튼을 클릭하면 LinkedIn에 인증서를 추가할 수 있습니다. (Voluntarily Section)
- AWSKRUG LinkedIn Company ID: 14523830

# 시스템 요구사항
- 순수 정적 웹사이트 (HTML5, vanilla CSS/JS, jQuery, Bootstrap) 유지