# Auto Instagram Post Generator (Make.com Automation)

Google Sheets의 주제 데이터를 기반으로 Gemini AI가 캡션을 자동 생성하고, Google Drive의 이미지와 조합하여 Instagram for Business에 자동 포스팅하는 Make.com 워크플로우입니다.

## 🔄 워크플로우 흐름

1. **Google Sheets (`filterRows`)**: 금일 날짜 기준 포스팅 키워드 및 데이터 검색
2. **Google Gemini AI (`createACompletionGeminiPro`)**: 핵심 3줄 요약 및 한국어 해시태그 5개 자동 생성
3. **Google Drive (`getAFile`)**: 인스타그램에 첨부할 이미지 파일 다운로드 
4. **Instagram for Business (`CreatePostPhoto`)**: 생성된 캡션과 이미지를 합성하여 자동 게시

## 🚀 시작하기

1. `blueprint.json` 파일을 다운로드합니다.
2. Make.com 대시보드에서 **Scenarios** > **Import Blueprint**를 선택하여 `blueprint.json`을 불러옵니다.
3. 각 모듈의 커넥션(Google, Gemini, Meta/Instagram)을 본인의 계정으로 다시 연결합니다.
4. Google Sheets 및 Google Drive의 Target ID를 사용자 환경에 맞게 수정합니다.

## 🛠️ 요구 사항

* Make.com 계정
* Google Workspace (Drive, Sheets)
* Google Gemini API Key
* Instagram Business 계정 (Facebook 페이지 연동 필수)
