# SBLT Official Website

SBLT의 End-to-End Performance Engineering 철학을 하나의 Storytelling Landing Page로 구현한 공식 홈페이지입니다.

## Included

- Hero / 회사 소개 / Vision / Why SBLT
- Core Experience / Core Value
- 6개 Service
- 8단계 Performance Engineering Journey
- Technology Constellation
- Why Customers Choose SBLT / Contact
- Responsive UI, Keyboard Navigation, Reduced Motion
- Metadata, Open Graph, Schema.org, Sitemap, Robots
- 섹션별 설계 근거: `DESIGN-STRATEGY.md`

## Stack

- Next.js App Router
- TypeScript
- TailwindCSS
- React
- Lucide Icons
- Native IntersectionObserver + CSS Motion

GSAP, Lenis, React Three Fiber는 현재 정보 전달에 비해 Bundle Cost와 Accessibility Risk가 더 크다고 판단해 제외했습니다. 새로운 3D Scene이나 복합 Sequence가 필요할 때 Dynamic Import로 추가할 수 있습니다.

## Local development

```bash
npm install
npm run dev
```

## Production validation

```bash
npm run build
npm run validate:artifact
```

## Brand assets

- `public/assets/sblt-logo.png` — 기존 시안의 Logo와 SBLT Wordmark 보존본
- `public/assets/hero-spiral.webp` — 기존 나선형 Identity를 계승한 Hero Visual
- `public/assets/transaction-flow.webp` — 6개 Layer가 Root Cause로 수렴하는 Visual
- `public/assets/technology-constellation.webp` — Technology 관계형 Visual
- `public/assets/og-sblt.jpg` — Open Graph Image

## Contact

- Email: jaeseok@sblt.ai
- Website: https://sblt.ai
