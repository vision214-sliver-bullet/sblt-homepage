# SBLT Homepage Static Export

`sblt.ai`에 배포되는 정적 웹사이트 저장소입니다. Next.js 정적 export 결과와 별도 SEO 랜딩 페이지를 포함합니다.

## 페이지

- `/` — 메인 홈페이지
- `/performance-test/` — 성능테스트 서비스
- `/whatap-apm/` — WhaTap APM 서비스
- `/troubleshooting/` — 트러블슈팅 서비스

## 로컬 확인

루트 절대 경로(`/_next`, `/assets`)를 사용하므로 HTML 파일을 직접 열지 말고 웹 서버로 실행합니다.

```powershell
python -m http.server 8080
```

브라우저에서 `http://127.0.0.1:8080/`을 엽니다.

## 배포

저장소 전체를 GitHub Pages 루트에 배포합니다. `_next` 디렉터리가 그대로 제공되도록 `.nojekyll` 파일을 유지하고, 사용자 도메인은 `CNAME`에서 관리합니다.

## 유지보수 주의사항

- 이 저장소에는 원본 Next.js 프로젝트가 없으며 빌드 산출물만 있습니다.
- `_next/static` 파일명 또는 내용을 변경하면 `index.html`, `404.html`의 참조도 함께 확인해야 합니다.
- 변경 후 데스크톱·모바일 화면, 브라우저 콘솔, 내부 링크와 정적 자산 경로를 확인합니다.
