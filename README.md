# 정문영 · Data Analyst

**숫자의 숨은 뜻을 찾고, 비즈니스 액션까지 이어지게 하는 데이터 분석가입니다.**
통계·ML·엔지니어링을 도구로 다루되, 최종 결과물은 언제나 **현장에서 실행 가능한 의사결정**이어야 한다고 믿습니다.

- **숨은 뜻을 찾는 분석** — 상관 r=0.768의 함정을 넘어 "범죄 → CCTV 설치"의 역인과 구조를 규명하고, GEE·FDR·Cohen's Kappa 등 **데이터 구조에 맞는 통계 도구**를 선택할 수 있습니다.
- **액션으로 이어지는 해석** — R² 0.04를 양보하더라도 Monotone Constraints로 가격 역전을 막아 **매입 담당자가 즉시 사용 가능한 모델**을 만들고, 4사분면 분류로 "어느 자치구에 먼저" 같은 정책 우선순위를 도출합니다.
- **End-to-End 엔지니어링** — 크롤링(Selenium) → 전처리 → ML(XGBoost·RandomForest) → RAG(LangChain·FAISS) → Streamlit 실서비스 배포까지 **5개 프로젝트를 독자적으로 운영**했습니다.

Contact: kobing7122@gmail.com · 010-7122-3794
Portfolio: https://www.notion.so/252404a59bef802b8693d40f30b48d82
Dashboards: https://bit.ly/3PNvBYt

---

## About Me

- 이름: 정문영
- 학력: 호서대학교 컴퓨터공학 (2020.03 ~ 2026.02, 학점 3.85 / 4.5)
- 교육: 커널 데이터 분석 부트캠프 수료 (2025.12 ~ 2026.04)
- 자격: 정보처리기사 필기 합격 (2025.03)
- 관심 분야: 한국어 NLP, LLM 활용 분석, 반복측정·역인과 구조 해석, 정책·비즈니스 의사결정 지원

---

## Tech Stack

| 영역 | 스택 |
|---|---|
| Language & DB | Python, SQL (PostgreSQL) |
| Data & ML | Pandas, NumPy, Scikit-learn, XGBoost, Statsmodels |
| NLP & LLM | LangChain, FAISS, BERTopic, Kiwi, KoNLPy, OpenAI API, Gemini API |
| Web & Viz | Streamlit, Tableau, Plotly, Selenium, BeautifulSoup |

---

## Key Projects

대표 프로젝트 순으로 정렬했습니다. 각 프로젝트의 문제 정의·아키텍처·트러블슈팅 상세는 포트폴리오(Notion)에서 확인하실 수 있습니다.

### 1. 위플래닛 BARO — 중고 매입가 예측 ML 시뮬레이터
**기업 연계 팀 프로젝트 (위플래닛/BARO) · 2026.02 ~ 2026.04 · 기여도 80%**

4,325건 실거래 데이터 기반 2단계 ML 시스템(감가상각 R² 0.94 / 상태보정 R² 0.75)을 구축. R² 0.04를 양보하는 대신 XGBoost Monotone Constraints로 **가격 역전을 원천 차단**하여, 매입 담당자가 즉시 사용 가능한 모델을 실배포했습니다.

| 항목 | 내용 |
|---|---|
| Stack | Selenium, RandomForest, XGBoost(Monotone), Streamlit |
| Impact | 경험·감에 의존하던 매입가 산정을 자동화, 현장 설명 가능성 확보 |
| Key Point | 비정형 텍스트 → 12개 정형 피처(정규표현식 파싱), 매입 전략별(공격·기본·보수) 마진 시뮬레이터 |
| Link | https://github.com/JungMoonYoung/baro-dashboard2 |

---

### 2. Career Insight — 하이브리드 RAG 채용공고 검색 + 연봉 예측
**개인 프로젝트 · 2025.12 ~ 2026.04**

6,332건 채용공고를 로컬 임베딩 + Gemini API 하이브리드 구조로 인덱싱하여 **재임베딩 비용 $0**을 달성. 연봉 예측 모델 R² 0.77로 **직무가 연봉 결정 요인의 60.3%**를 차지함을 입증했습니다.

| 항목 | 내용 |
|---|---|
| Stack | LangChain, FAISS, ko-sroberta, Gemini API, RandomForest, Streamlit |
| Impact | 비용 vs 품질 트레이드오프를 코사인 유사도 80% 임계값으로 분기 처리 |
| Key Point | 4종 ML 모델 비교 후 정확도보다 해석성을 기준으로 RandomForest 채택 |
| Link | https://github.com/JungMoonYoung/career-assistant |


---

### 3. Auto-Insight — E-Commerce 고객 분석 자동화 플랫폼
**개인 프로젝트 · 2025.08 ~ 2025.09**

CSV 한 장만 업로드하면 RFM · 매출 · 리뷰 NLP · SQL까지 자동 실행되는 6단계 파이프라인. 한국어 NLP 감성 분석 정확도 **85%+**, 부정 리뷰만 선별해 전송하는 아키텍처로 **GPT API 비용 95% 절감**.

| 항목 | 내용 |
|---|---|
| Stack | KoNLPy, LDA, TF-IDF, K-Means, OpenAI API, Streamlit |
| Impact | 분석 전 과정을 자동화하여 현업이 데이터팀 대기 없이 직접 활용 가능 |
| Key Point | K-Means 최적 K값 Silhouette 탐색, CTE 3단 + Window Function 8종 자동 생성 |
| Link | https://github.com/JungMoonYoung/auto-insight-platform |

---

### 추가 프로젝트

| 프로젝트 | 기간 | 핵심 결과 |
|---|---|---|
| OLIST 배송 최적화 (부트캠프 팀) | 2026.02 | K-Means MFC 9개 거점 도출, 배송거리 -80.4%, 손익분기 3.7년 |
| 지하철 A/B Test (개인) | 2025.11 ~ 12 | 50만 건 GEE + AR(1) 자기상관 모델로 UI 효과 +5.71%p (p<0.001) 검증 |
| 역세권 상권 분석 (부트캠프 팀) | 2026.01 | 71역 × 5업종 전수조사 + 잔차분석으로 저평가 입지 9곳 발굴 |
| 서울시 CCTV-범죄 분석 (개인) | 2025.10 ~ 12 | r=0.768 표면 해석을 넘어 "범죄 → CCTV" 역인과 구조 규명 |

---

## 분석 철학

> 분석의 최종 산출물은 **의사결정**이라고 믿습니다.
>
> 모델의 정확도(R²)가 높아도 현장에서 설명이 안 되면 쓸 수 없습니다. 정확도를 소폭 양보하더라도 비즈니스 로직에 맞는 결과를 내는 분석이 실무에서는 더 가치 있다는 것을, 기업 연계 프로젝트에서 직접 경험했습니다.
>
> "통계를 돌리는 것"과 "통계를 고르는 것"은 다릅니다. 왜 이 방법을 선택했는지 설명할 수 있는 분석가가 되려고 합니다.


<!--
**JungMoonYoung/JungMoonYoung** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
