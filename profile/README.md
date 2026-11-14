<p align="center">
  <a href="https://finquest.space"><img src="./banner.png" alt="FinQuest — 대화로 만드는 나만의 주식 화면" width="100%"></a>
</p>

<p align="center">
  <a href="https://finquest.space"><b>웹 서비스</b></a>
  &nbsp;·&nbsp;
  <a href="https://mcp.finquest.space/"><b>MCP 안내</b></a>
  &nbsp;·&nbsp;
  <a href="https://mcp.finquest.space/demo"><b>데모 영상</b></a>
</p>

<br>

**FinQuest** 는 국내 주식을 대화로 리서치하는 서비스를 만듭니다.
공시·재무·시세를 **출처와 함께** 답하고, 필요한 카드·차트를 대화로 만들어 둡니다.

## 두 가지로 쓸 수 있습니다

| | |
|---|---|
| **FinQuest 웹** <br> [finquest.space](https://finquest.space) | 종목을 물어보면 공시 원문을 근거로 답하고, 원하는 카드·차트를 나만의 화면에 쌓아 둡니다. 내 AI 키로 쓰면 무료입니다. |
| **FinQuest 국내 주식·채권 MCP** <br> [mcp.finquest.space](https://mcp.finquest.space/) | Claude·ChatGPT·Claude Code 에 **주소 하나로** 한국 상장사 공시 데이터를 연결합니다. API 키·설치·로그인이 필요 없습니다. |

## 30초 연결

```
https://mcp.finquest.space/public/mcp
```

| 클라이언트 | 방법 |
|---|---|
| Claude (웹·데스크톱·모바일) | 설정 → 커넥터 → 사용자 지정 커넥터 추가 → 위 주소 |
| ChatGPT | 설정 → 앱·커넥터 → 고급 → 개발자 모드 → 커넥터 만들기 → 위 주소, 인증 "없음" |
| Claude Code | `claude mcp add --transport http finquest-dart https://mcp.finquest.space/public/mcp` |

연결한 뒤 이렇게 물어보세요.

> SK하이닉스 최근 분기 영업이익이 왜 늘었는지 회사 공시 문장으로 알려줘
>
> 최근 보고서에서 '판가 인상'을 실적 증가 이유로 든 회사들 찾아줘

## 데이터

- **코스피·코스닥 약 2,650개 상장사**
- 2016년 이후 DART 사업·반기·분기보고서 **약 9만 건**을 표준 양식으로 정리 — 부문·제품·지역별 매출, 가동률, 시설투자, 연구개발비를 분기 시계열로
- 회사가 보고서에 직접 쓴 **실적 변동 이유를 원문 그대로** 인용하고 DART 링크를 붙입니다
- 금융위원회 공공데이터의 일별 주가·지수, 장내 회사채, 국고채·회사채 금리 곡선

## 원칙

답에 실리는 숫자는 셋 중 하나입니다.

1. **공시 원문 그대로**
2. 원문을 바꿨다면(환산·보정) **바꿨다고 함께 적은 값**
3. 성립하지 않는 계산이면 **내보내지 않음** — 틀린 값보다 빈 값

---

<sub>FinQuest 는 공시를 정리한 참고 정보를 제공하며, 매매를 권하거나 주가를 예측하지 않습니다. 중요한 숫자는 DART 원문으로 확인하세요.</sub>

<sub>**English** — FinQuest builds conversational research tools for Korean equities: a web app at [finquest.space](https://finquest.space) and a hosted, no-API-key MCP server for KOSPI/KOSDAQ ([mcp.finquest.space](https://mcp.finquest.space/)) with ~90k normalized DART filings, segment revenue time series, quoted earnings drivers, prices and corporate bonds.</sub>
