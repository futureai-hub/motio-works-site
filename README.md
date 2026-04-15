# Motio Work — Developer Site

Motio Work의 통합 개발자 사이트입니다. GitHub Pages로 호스팅됩니다.

## 구조

```
motio-work-site/
├── index.html                          ← 개발자 랜딩 페이지
├── app-ads.txt                         ← AdMob 광고 인증 (전체 앱 공통)
├── README.md                           ← 이 파일
│
├── flexzen-motio/                      ← FlexZen Motio 앱
│   └── privacy-policy.html
│
├── (새 앱 이름)/                        ← 새 앱 추가 시
│   └── privacy-policy.html
```

## 새 앱 추가 방법

1. 앱 이름으로 폴더를 만듭니다 (예: `my-new-app/`)
2. `flexzen-motio/privacy-policy.html`을 복사해서 내용을 수정합니다
3. `index.html`의 `<!-- Coming Soon Placeholder -->` 부분을 복사해서 앱 정보로 수정합니다
4. push 하면 자동으로 배포됩니다

## 배포 체크리스트

- [ ] Privacy Policy에서 연락처 이메일 `your-email@example.com`을 실제 이메일로 교체
- [ ] GitHub에 push
- [ ] Settings → Pages → Source: main branch 활성화
- [ ] Google Play Console에 URL 설정:
  - 개발자 웹사이트: `https://<username>.github.io/motio-work-site/`
  - 개인정보처리방침: `https://<username>.github.io/motio-work-site/flexzen-motio/privacy-policy.html`
- [ ] AdMob 콘솔에서 app-ads.txt 크롤링 상태 확인
