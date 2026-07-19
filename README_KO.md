# Hojun Jeong Research Website

GitHub Pages에 바로 올릴 수 있는 정적 연구자 웹사이트입니다.

## 가장 쉬운 배포 방법

1. GitHub에서 `본인아이디.github.io`라는 **Public** repository를 만듭니다.
2. 이 폴더 안의 파일을 모두 repository 최상위에 업로드합니다.
3. GitHub repository에서 `Settings → Pages`로 이동합니다.
4. `Source: Deploy from a branch`, `Branch: main`, `Folder: /(root)`를 선택합니다.
5. 저장 후 `https://본인아이디.github.io/`에 접속합니다.

## 수정 위치

- 소개 및 News: `index.html`
- 논문: `publications.html`
- 연구 프로젝트: `research.html`
- 스타일: `assets/styles.css`
- 상호작용: `assets/script.js`
- CV PDF: `assets/pdf/Hojun_Jeong_CV.pdf`

## GitHub / Google Scholar 링크 추가

각 HTML 파일의 다음 부분을 찾습니다.

```html
<div class="link-row">
```

아래 링크를 추가하면 됩니다.

```html
<a href="https://github.com/YOUR_ID" target="_blank" rel="noopener">GitHub</a>
<a href="https://scholar.google.com/citations?user=YOUR_ID" target="_blank" rel="noopener">Google Scholar</a>
```

## 논문 링크 추가

`publications.html`과 `index.html`에서 `Preprint pending`, `Code pending` 부분을 다음처럼 교체합니다.

```html
<a href="PREPRINT_URL" target="_blank" rel="noopener">Preprint</a>
<a href="CODE_URL" target="_blank" rel="noopener">Code</a>
```

홈페이지와 Publications 페이지에 논문 마크업이 각각 있으므로 두 파일을 함께 수정해야 합니다.

## 이미지 사용

현재 버전은 프로필 사진과 논문·연구 썸네일을 사용하지 않는 텍스트 중심 구성입니다. 논문은 제목, 저자, 학회 정보, 링크 순으로 표시됩니다.

## 확인이 필요한 내용

- 기존 CV에서 수상 내역의 행사명이 HCLT와 KCC로 서로 다르게 적혀 있어 사이트에서는 Award를 제외했습니다.
- Preprint, Code, GitHub, Google Scholar URL은 제공되지 않아 연결하지 않았습니다.
