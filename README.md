# FF14 이벤트 매니저 디스코드 봇

이 디스코드 봇은 공식 웹사이트에서 FF14(파이널판타지14)의 이벤트 정보를 스크래핑하여 자동으로 이벤트를 관리하고 업데이트합니다. 봇은 여러 디스코드 서버에서 이벤트를 생성하고 종료할 수 있습니다. 해당 봇은 코파일럿을 통해 제작 되었습니다.

## 기능

- 공식 웹사이트에서 FF14 이벤트 정보를 자동으로 스크래핑합니다.
- 스크래핑한 정보를 바탕으로 디스코드 서버에서 일정 이벤트를 생성합니다.
- 단일 명령어로 모든 기존 이벤트를 종료합니다.
- 5시간마다 새로운 이벤트를 자동으로 확인합니다.
- 여러 디스코드 서버를 지원합니다.

## 명령어

### `/서버등록`

현재 서버를 이벤트 관리 목록에 등록합니다.

### `/이벤트생성`

수동으로 이벤트 생성 프로세스를 트리거하여 FF14 웹사이트에서 최신 정보를 기반으로 이벤트를 생성합니다.

### `/이벤트종료`

현재 서버의 모든 기존 이벤트를 취소합니다.

## 설정

### 사전 요구 사항

- Python 3.7 이상
- 디스코드 봇 토큰
- 필요한 Python 패키지 ( `requirements.txt` 파일에 명시됨)

### 설치

1. 저장소를 클론합니다:
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. 필요한 Python 패키지를 설치합니다:
    ```bash
    pip install -r requirements.txt
    ```

3. 디스코드 봇을 설정합니다:
    - [디스코드 개발자 포털](https://discord.com/developers/applications)로 이동하여 새로운 애플리케이션을 만듭니다.
    - 애플리케이션에 봇 사용자를 생성하고 봇 토큰을 복사합니다.
    - OAuth2 URL 생성기를 사용하여 봇을 서버에 초대합니다.

4. 봇을 구성합니다:
    - 코드에서 `YOUR_DISCORD_BOT_TOKEN`을 실제 디스코드 봇 토큰으로 교체합니다.

5. 봇을 실행합니다:
    ```bash
    python bot.py
    ```

## 사용법

1. 서버 등록:
    ```bash
    /서버등록
    ```

2. 수동으로 이벤트 생성:
    ```bash
    /이벤트생성
    ```

3. 모든 이벤트 종료:
    ```bash
    /이벤트종료
    ```

## TODO
커버 이미지 업로드

## 기여

기여는 언제나 환영합니다! 버그나 기능 요청이 있는 경우 풀 리퀘스트를 제출하거나 이슈를 열어주세요.

## 라이센스

이 프로젝트는 MIT 라이센스를 따릅니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.
