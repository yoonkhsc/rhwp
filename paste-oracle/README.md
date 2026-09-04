# PR #6725 — 붙여넣기 정답지 파일 (재검증 입력 고정)

| 파일 | 역할 |
|---|---|
| `msit-press-release-2026-07-01.original.hwpx` | 공개 원본. 대한민국 정책브리핑(korea.kr)에서 2026-09-04 내려받음. 원본 파일명 `260702 조간 (보도) 대한민국을 명실상부한 피지컬 AI 1강으로,,, 과기정통부, 피지컬 AI 핵심 경쟁력 확보 전략 발표.(수정).hwpx` |
| `msit-press-release-2026-07-01.hancom-saved-oracle.hwpx` | 위 원본을 한글에서 열어 다시 저장한 것. `<hp:linesegarray>`(한컴이 계산한 줄 조판)가 259개 문단 전부에 들어 있어 **줄 단위 대조의 정답지**로 썼다. 본문 텍스트는 원본과 동일(9,854자) |
| `msit-press-release-2026-07-01.rhwp-pasted-result.hwpx` | 한글 `Ctrl+C` → rHWP `Ctrl+V` 결과를 rHWP 로 내보낸 것. linesegarray 없음(로드 시 재조판) — 대조의 비교 대상 |

- 원문 페이지: https://www.korea.kr/briefing/pressReleaseView.do?newsId=156769196
- 파일 URL: https://www.korea.kr/common/download.do?fileId=198518529&tblKey=GMN
- 내려받은 날짜: 2026-09-04 (KST)
- SHA-256: 아래 `SHA256SUMS`
- 대조 방법: 두 문서를 같은 엔진으로 조판해 쪽별 줄 텍스트를 대조(`rhwp-q-text-layout --page N`). 정답지는 저장 조판을 그대로 쓰고, 결과는 재조판된다.
