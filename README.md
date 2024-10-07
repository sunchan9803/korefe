# 코리페

**코리페**는 공공데이터포털의 전국문화축제 표준데이터 API를 기반으로 한 웹 애플리케이션으로, 사용자가 전국의 다양한 문화축제를 탐색하고, 검색 및 공유할 수 있는 기능을 제공합니다.

## 🛠️ 기술 스택

- **언어:** Python, JavaScript, HTML5, CSS
- **프레임워크:** Django
- **데이터베이스:** MySQL
- **외부 API:**
    - [공공데이터포털 전국문화축제 표준데이터](https://www.data.go.kr/data/15013104/standard.do)
    - 카카오 로그인
    - 카카오 맵 API
- **서버 환경:** AWS EC2 (Linux, Ubuntu)
- **개발 도구:** Docker, Docker Compose

## 📌 주요 기능

- **카카오 소셜 로그인:** Django Allauth를 활용한 카카오 계정 연동
- **전국 지도 기반 문화축제 탐색:** 카카오 맵 API를 사용하여 전국 축제 위치 시각화
- **반응형 UI:** 모바일과 PC 환경에 최적화된 반응형 웹 디자인
- **좋아요 및 공유 기능:** 각 축제에 대한 좋아요 및 소셜 미디어 공유 가능
- **검색 기능:** 다양한 필터를 통해 축제 검색 가능

## 🚀 로컬 개발 환경 실행 방법

1. **Docker 설치**
    - [Docker 공식 사이트](https://www.docker.com/)에서 Docker 및 Docker Compose를 설치합니다.

2. **Docker Compose로 애플리케이션 실행**
    - 프로젝트 루트 디렉토리에서 다음 명령어를 실행하여 컨테이너를 빌드 및 실행합니다:
      ```bash
      docker-compose -f docker-compose.dev.yml up --build
      ```

3. **애플리케이션 접속**
    - 브라우저에서 [http://localhost:8000](http://localhost:8000)으로 접속하여 애플리케이션을 확인할 수 있습니다.

4. **MySQL 설정 확인**
    - MySQL은 로컬 호스트의 `3307` 포트에서 실행되며, 기본 데이터베이스 정보는 `festival`, 사용자 `root`, 비밀번호 `root`로 설정되어 있습니다.
