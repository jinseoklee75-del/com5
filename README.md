# 조직역량개발비 관리 시스템 (Web)

GitHub Pages에 **웹 앱**을 배포하는 Next.js 프로젝트입니다.

## GitHub 배포 (필수 설정)

1. 이 저장소를 GitHub에 push (`main` 브랜치)
2. **Settings → Pages → Build and deployment**
   - **Source: GitHub Actions** ← README가 아닌 앱이 배포됩니다
3. Actions에서 **Deploy to GitHub Pages** 워크플로우 성공 확인
4. Pages URL 접속  
   - 예: `https://사용자명.github.io/저장소명/`
   - **로그인/대시보드 화면**이 보이면 성공

> 저장소 메인 화면의 README.md는 문서일 뿐이며, Pages URL과 다릅니다.

## 로컬 실행

```bash
npm install
npm run dev
```

http://localhost:3000

## 화면

| 경로 | 설명 |
|------|------|
| `/` | 홈 · 시작하기 |
| `/dashboard/` | KPI 대시보드 |
| `/budget/` | 사용내역 목록 |
| `/register/` | 사용내역 등록 (AI 분류 데모) |

## 기술

- Next.js 15 (App Router)
- Tailwind CSS 4
- 정적 export → GitHub Pages

## 백엔드 API 추가 (선택)

현재는 **데모 데이터**로 동작합니다. NestJS API를 연결하려면 Render/Railway 등에 API를 배포하고 `NEXT_PUBLIC_API_URL`을 빌드 시 주입하세요.

## 라이선스

Internal use
