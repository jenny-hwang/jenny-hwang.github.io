# Jihyun Jenny Hwang — Academic Homepage

Jekyll 기반 아카데믹 홈페이지입니다.

## 파일 구조

```
├── _config.yml          # 이름, 이메일 등 기본 설정
├── _layouts/
│   └── default.html     # 모든 페이지에 적용되는 레이아웃
├── _pages/
│   ├── research.md      # Research 페이지
│   ├── publications.md  # Publications 페이지
│   └── cv.md            # CV 페이지
├── assets/
│   ├── css/main.css     # 스타일시트
│   ├── photo.jpg        # 본인 사진 (교체 필요)
│   └── cv.pdf           # CV PDF 파일 (추가 필요)
├── index.md             # 홈 페이지
└── Gemfile
```

## 빠른 설정 가이드

### 1. 사진 추가
`assets/` 폴더에 본인 사진을 `photo.jpg`로 저장하세요.

### 2. 기본 정보 수정
`_config.yml`에서 department, description 등을 수정하세요.

### 3. 내용 채우기
각 `[대괄호]` 안의 플레이스홀더를 실제 내용으로 교체하세요.

### 4. GitHub Pages 배포

```bash
# 1. GitHub에서 새 저장소 생성: username.github.io
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
git push -u origin main
```

GitHub 저장소 설정(Settings → Pages)에서 Source를 `main` 브랜치로 설정하면
`https://USERNAME.github.io`로 자동 배포됩니다.

### 5. 로컬에서 미리보기

```bash
bundle install
bundle exec jekyll serve
# http://localhost:4000 에서 확인
```

## 커스텀 도메인 연결 (선택)

GitHub Pages Settings → Custom domain에 도메인을 입력하고,
도메인 제공업체에서 CNAME 레코드를 `USERNAME.github.io`로 설정하세요.
