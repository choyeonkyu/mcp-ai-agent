# MCP AI Agent

Yeon-kyu-MCP-Agent 기반의 개인 맞춤형 AI 비서입니다. 날씨, 뉴스, KBO 야구 순위, 구글 캘린더 일정 등 일상에 필요한 정보들을 종합하여 브리핑을 제공합니다.

## 🚀 주요 기능 (Tools)

이 AI 에이전트는 다음과 같은 도구들을 사용하여 다양한 작업을 수행할 수 있습니다.

-   **`brief_today`**: 날씨, 뉴스, 야구 순위, 오늘 일정을 종합하여 하루를 브리핑합니다.
-   **`get_weather`**: 특정 도시의 현재 날씨 정보를 제공합니다.
-   **`get_news_headlines`**: 구글 뉴스 RSS 피드에서 최신 헤드라인을 가져옵니다.
-   **`get_kbo_rank`**: KBO 프로야구 리그의 최신 순위를 보여줍니다.
-   **`today_schedule`**: 구글 캘린더에서 오늘 등록된 일정을 가져옵니다.
-   **`daily_quote`**: 영감을 주는 명언을 생성합니다.
-   **`scrape_page_text`**: 지정된 URL의 웹페이지에서 텍스트 콘텐츠를 추출합니다.
---
## 시연 예시


---

## ⚙️ 설치 및 설정

### 1. 프로젝트 준비

```bash
# 가상환경 생성 및 활성화
python -m venv mcp-ai-agent
source mcp-ai-agent/Scripts/activate
```

### 2. 의존성 설치

필요한 라이브러리를 설치합니다.

```bash
pip install mcp fastmcp fastapi geopy feedparser beautifulsoup4 httpx langchain_openai python-dotenv google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client langchain-mcp-adapters jinja2
```

### 3. Google Calendar API 설정

`today_schedule` 기능을 사용하려면 Google Calendar API 설정이 필요합니다.

1.  **Google Cloud Console**에서 OAuth 2.0 클라이언트 ID를 생성합니다.
    -   [Google Cloud Console](https://console.cloud.google.com/apis/credentials)에 접속하여 새 프로젝트를 생성합니다.
    -   **API 및 서비스 > OAuth 동의 화면**에서 필요한 정보를 입력하고 테스트 사용자로 본인의 구글 계정을 추가합니다.
    -   **API 및 서비스 > 사용자 인증 정보**에서 **사용자 인증 정보 만들기 > OAuth 클라이언트 ID**를 선택합니다.
    -   애플리케이션 유형을 **데스크톱 앱**으로 선택하고 클라이언트를 생성합니다.
    -   생성된 인증 정보를 JSON 형식으로 다운로드하여 프로젝트 루트 디렉토리에 `credential.json` 파일명으로 저장합니다.
2.  **Google Calendar API 활성화**
    -   프로젝트의 **API 및 서비스 > 라이브러리**에서 "Google Calendar API"를 검색하여 활성화합니다.

---

## ▶️ 실행 방법

1.  **MCP 서버 실행**
    -   MCP 에이전트 서버를 시작합니다.

    ```bash
    python mcp_server.py
    ```

2.  **채팅 클라이언트 실행**
    -   별도의 터미널에서 채팅 클라이언트를 실행하여 에이전트와 상호작용합니다.

    ```bash
    python chat_agent.py
    ```
---

## 기술 포인트

* **//**
* **//**
* **//**
* **//**

---

## 향후 확장 계획

* [ ] //
* [ ] //
* [ ] /

---

## 👨‍💻 Author

**조연규 (Data Engineer @ Samsung Electronics Logitech)**
