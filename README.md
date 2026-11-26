# OrderLab

Python 테스트와 GitHub Actions CI/CD 실습 프로젝트

## 로컬 실행

가상환경을 활성화한 뒤 패키지를 설치

    python -m pip install -r requirements-dev.txt

코드검사 및 테스트

    ruff check .
    ruff format --check .
    python -m pytest -q

## 보고서 생성

    python generate_report.py

`site/index.html`에서 확인

## CI/CD

- Push와 Pull Request에서 코드 검사와 테스트
- main에 Push할 경우 품질 검사후 GitHub Pages에 보고서 배포
