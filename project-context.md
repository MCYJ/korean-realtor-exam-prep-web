# KOR-0240 marketing site context

## Scope

- Independent public marketing and study site for released app `KOR-0240` only.
- App source is read-only: `/Users/youngjunma/Documents/various test prep apps project/services/kor/02/kor-0240`.
- Android package and iOS bundle identifier: `app.mcyj.examprep.kor0240`.
- Production target: `https://mcyj.github.io/korean-realtor-exam-prep-web/`.

## Verified Store state — 2026-09-19

- Google Play resolves publicly for the exact package.
- Apple lookup resolves the exact bundle to track ID `6797284357` in KR.
- Both official Store badges are active and use the same 194 × 75 px outer frame without distorting artwork.

## Content and official facts

- Korean and English routes with 10 substantive guides per locale.
- Official qualification: 공인중개사 (`jmCd=9630`).
- Stage 1: real estate principles and civil law, 40 items each; 80 items in 100 minutes.
- Stage 2: brokerage law/practice, public real-estate law, and registration/tax; 120 items in 150 minutes over two sessions.
- Each stage requires at least 40 in every subject and a stage average of 60.
- A Stage 1 pass provides an exemption at the next exam, subject to the current official implementation notice.
- The 37th examination is October 31, 2026. Standard application is August 3–7 and vacancy application October 1–2.
- Canonical sources:
  - `https://www.q-net.or.kr/site/junggae`
  - `https://www.q-net.or.kr/crf005.do?gId=36&gSite=Q&id=crf00503s02&jmCd=9630&jmInfoDivCcd=B0`
  - `https://www.q-net.or.kr/man004.do?ARTL_SEQ=5270524&BOARD_ID=Q001&gId=08&gSite=L&id=man00402`

## Design and implementation

- Visual thesis: an indigo cadastral worksheet with terracotta legal markers and a clear 1st-stage/2nd-stage score architecture.
- Global Korean-safe wrapping uses `word-break: keep-all` and `overflow-wrap: break-word`.
- Dependency-free static generator; GitHub Actions builds, checks and deploys `dist/` to Pages.

## Verification log

- 2026-09-19: project initialized from the proven static-site system and retargeted to KOR-0240 content, assets and Store identities.
- 2026-09-19: local build generated 34 indexable routes and 36 HTML files; the checker passed metadata, links, both exact Store identities, `keep-all` and equal marketplace frames.
- 2026-09-19: local HTTP QA returned 200 for all 34 sitemap routes and five key assets; an unknown route returned 404.
- 2026-09-19: live Store recheck returned Google Play 200 and Apple bundle `app.mcyj.examprep.kor0240`, track ID `6797284357`.
