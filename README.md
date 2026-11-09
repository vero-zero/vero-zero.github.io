# 고테아 포트폴리오

단일 HTML 파일(`index.html`)로 된 정적 포트폴리오입니다. 빌드 과정 없이 GitHub Pages에 그대로 올립니다.

## 배포 (GitHub Pages)

1. 개인 GitHub에 `<아이디>.github.io` 이름으로 **public** 저장소를 만듭니다.
2. `index.html` 맨 아래 스크립트의 `GITHUB_USER`에 아이디를 넣습니다. 넣으면 GitHub 버튼과 플러그인 저장소 링크가 나타납니다.
3. **개인 이메일**로 커밋하고 push합니다.

   ```
   git init
   git config user.email "개인메일@..."
   git config user.name "고테아"
   git add index.html README.md
   git commit -m "포트폴리오 사이트"
   git branch -M main
   git remote add origin https://github.com/<아이디>/<아이디>.github.io.git
   git push -u origin main
   ```
4. 1~2분 뒤 `https://<아이디>.github.io` 에서 확인합니다.

## 공개 원칙

- 회사 소스 코드는 넣지 않습니다. 실무 프로젝트는 구조와 흐름만 설명합니다.
- 공개 사이트이므로 발주처 이름 대신 일반 명칭("국가 연구기관 연구자 포털" 등)을 씁니다.
- 수치는 직접 확인한 것만 씁니다.

## 구성

- 대표 프로젝트 3개: 문제 · 접근 · 결과 + SVG 다이어그램
- 청크 분할 데모: 플러그인의 `chunk_text()`를 JavaScript로 옮긴 것 (Python 원본과 15개 경우에서 결과 일치 확인)
- 라이트/다크 테마, 모바일 대응
