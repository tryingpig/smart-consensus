# Smart Consensus

증권사 목표주가 컨센서스 추적·분석 사이트 (GitHub Pages).

epic.ai.kr 에서 종목별 주가 시계열 + 증권사별 목표주가 리포트를 수집해
`EpicAI-Monitor` 실행 시 매일 스냅샷을 떠서 이 레포에 누적 저장한다.

- `data/{code}.json` — 종목별 { price(주가 시계열), reports(증권사 목표가 이력) }
- `data/index.json` — 종목 목록(코드·이름·업종)
- `index.html` — 종목 선택 → 주가+목표가 마커 / 증권사별 목표가 추이 / 반응성·선행성 분석

주가 시계열은 epic API에서 매번 최신으로 갱신, 리포트는 dedup 누적(약 1년 보관).

공개 URL: https://tryingpig.github.io/smart-consensus/
