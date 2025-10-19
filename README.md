# 모바일 우선(iPhone 최적) 원페이지 스타터

## 빠른 편집
`index.html`에서 다음 부분만 바꾸세요.
- `PROJECT_NAME` → 사이트/프로젝트 이름
- `HEADLINE_TEXT` → 히어로 한 줄 메시지
- 연락처
  - `href="tel:+821012345678"` → 실제 전화번호
  - `mailto:you@example.com` → 실제 이메일
  - `https://open.kakao.com/o/yourLink` → 오픈채팅/채널 링크

이미지 교체는 `/assets` 폴더의 이미지들을 원하는 것으로 바꾸면 됩니다.
- 소셜 미리보기: `og-image.png` (권장 1200x630)
- 앱 아이콘(iOS 홈 화면): `apple-touch-icon.png` (권장 180x180)
- 히어로 이미지: `hero-640.jpg`, `hero-960.jpg`, `hero-1280.jpg`

## GitHub Pages 배포(가장 쉬움)
1. GitHub에서 새 레포를 만듭니다.
2. 이 폴더의 파일들을 업로드(또는 `git push`).  
3. 레포 **Settings → Pages**에서 브랜치를 `main`으로 지정 후 저장.
4. 잠시 후 `https://<your-username>.github.io/<repo>/` 로 접속 가능합니다.
   - 루트 도메인을 쓰려면 레포 이름을 `<your-username>.github.io` 로 만드세요.

## iPhone 최적화 포인트
- `viewport-fit=cover` + safe-area 패딩으로 노치/홈 인디케이터 대응
- 큰 터치 영역(최소 44px), 하단 고정 CTA 바
- Web Share API(미지원 브라우저는 자동 복사 폴백)
- 시스템 폰트 스택으로 빠른 렌더링
