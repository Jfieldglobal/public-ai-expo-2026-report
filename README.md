# 2026 공공AI 박람회 기술 트렌드 분석 리포트

행정안전부·NIA 주관 **제9회 전자정부의 날 기념 2026 공공AI 박람회** 전체 세션을 분석하고, 공공 AI 시장의 기술 트렌드와 전략적 시사점을 정리한 리포트입니다.

---

## 프로젝트 목적

공공 AI 박람회에서 발표된 5개 세션과 51개+ 참여기업 정보를 체계적으로 분석하여, 기관장·CIO/CDO·기술 전략팀이 **2026~2027 공공 AI 투자 및 도입 전략**을 수립하는 데 필요한 인사이트를 제공합니다.

구체적인 분석 목표는 다음과 같습니다:

- 2026 공공 AI 시장의 핵심 기술 트렌드 식별 및 우선순위 도출
- 토픽별 기술 심층 분석 (아키텍처·성능·공공 적합성)
- 참여기업의 경쟁 포지션 및 솔루션 지형 파악
- Technology Maturity Assessment를 통한 도입 시기 판단
- 기관 유형별 Strategic Implications 및 2027 Outlook 제시

---

## 데이터 구성

```
data/
├── 01_AI이듬_AI통합민원플랫폼/
│   ├── *-Summary.md          # 세션 요약 (텍스트)
│   ├── *-Summary (1).md      # 세션 요약 (이미지 포함)
│   └── *-Highlights.pdf      # 발표 하이라이트 (11.5 MB)
│
├── 02_기관 책임자들에 의한 AI바이드코딩 시현/
│   ├── *-Summary.md
│   ├── *-Summary (1).md
│   └── *-Highlights.pdf      # 바이브 코딩 시연 화면 (3.7 MB)
│
├── 03_LG CNS Exaone 4.5모델 적용 및 Workspace 적용 사례/
│   ├── *-Summary.md
│   └── *-Summary (1).md
│
├── 04_Kakao Kanana Model 적용 시현 및 안내_정부24,KakaoTalk/
│   ├── *-Summary.md
│   └── *-Summary (1).md
│
└── 05_참여기업 분석 및 소개 Directory Book/
    └── Kpaix_2026공공AI_directorybook.pdf   # 참여기업 디렉토리북 (13 MB)
```

| 구분 | 세션 주제 | 주요 발표사 |
|------|----------|-----------|
| Topic 01 | AI 통합민원플랫폼 | 이듬 AI |
| Topic 02 | 기관 책임자들에 의한 AI 바이브코딩 시현 | 행정안전부·NIA·카카오 (기관장 직접 시연) |
| Topic 03 | LG CNS Exaone 4.5 모델 적용 및 Workspace 적용 사례 | LG CNS / LG AI연구원 |
| Topic 04 | Kakao Kanana Model 적용 시현 및 안내 (정부24·KakaoTalk) | 카카오 |
| Topic 05 | 참여기업 분석 및 소개 Directory Book | 51개+ 참여기업 전체 |

---

## 분석 방법

### 1단계: 소스 데이터 수집 및 파싱

각 세션의 Summary.md(텍스트 요약)와 Highlights.pdf(발표 화면·타임라인)를 병행 분석했습니다. PDF에서는 발표자 발언·기술 아키텍처 다이어그램·실제 시연 화면 정보를 추출했습니다.

### 2단계: 토픽별 심층 분석 (topic01~05.md)

각 세션을 다음 5개 축으로 분석했습니다:

- **Executive Summary**: 세션의 핵심 메시지와 전략적 의도 파악
- **Key Technologies**: 기술 아키텍처·구성 요소·성능 지표 상세 분석
- **Technical Keywords**: 카테고리별 핵심 기술 용어 정리
- **Public Sector Impact**: 공공 부문 적용 가능성·기대 효과·한계
- **Strategic Insights**: 경쟁 맥락·리스크·다음 단계 제언

### 3단계: 크로스 토픽 통합 분석

5개 세션을 가로질러 반복 등장하는 기술 키워드의 출현 빈도를 집계하고, **Technology Maturity Assessment**(Production / Early Production / Growing / Emerging)를 수행해 도입 시기 판단의 기준을 제시했습니다.

### 4단계: 최종 리포트 생성

Executive level 독자를 위한 1페이지 분량의 전략 리포트를 Markdown 및 McKinsey 스타일 HTML로 출력했습니다.

---

## 생성된 결과물

```
docs/
└── topic_analysis/
    ├── topic01.md    # AI 통합민원플랫폼 상세 분석
    ├── topic02.md    # AI 바이브코딩 시현 상세 분석
    ├── topic03.md    # LG CNS Exaone 4.5 상세 분석
    ├── topic04.md    # Kakao Kanana 상세 분석
    └── topic05.md    # 참여기업 Directory Book 분석 (51개+)

report/
├── 2026_공공AI박람회_기술트렌드리포트.md     # 마크다운 최종 리포트
└── 2026_공공AI박람회_기술트렌드리포트.html   # HTML 최종 리포트 (McKinsey 스타일)
```

**HTML 리포트 주요 구성요소**:

| 섹션 | 내용 |
|------|------|
| Executive Summary | 3대 핵심 메시지 (Agentic AI 기준선화 / 국산 LLM 인프라화 / 보안 조달 기준화) |
| 핵심 기술 트렌드 TOP 5 | 트렌드 카드 레이아웃, 출현 빈도·대표 사례·임팩트 |
| 반복 등장 기술 분석 | 5×9 빈도 테이블 + Technology Maturity Assessment |
| 기업 및 기관 동향 | 대기업 플랫폼화 vs 스타트업 버티컬, 주요 파트너십 |
| Strategic Implications | CIO/CDO 대상 4가지 실행 지침 |
| 2027 Outlook | 5개 영역 전망 |
| Key Takeaways | 기관장·CIO·벤더·정책입안자 독자군별 메시지 |

---

## 주요 발견사항

### 1. Agentic AI가 공공 AI의 새로운 기준선

5개 세션 중 4개에서 Multi-Agent 또는 Agentic AI 키워드가 등장했습니다. 단순 챗봇·검색 보조를 넘어 **계획→실행→검증을 자율 반복하는 Agent 시스템**이 2026 공공 AI의 핵심 패러다임으로 확립됐습니다.

> 이듬 AI Pipeline Orchestrator, LG CNS AgenticWorks, 와이즈넛 WISE Agent Sphere, 제네시스랩 Agentria

### 2. 국산 LLM 4파전 — 공공 채널 선점 경쟁 본격화

Exaone 4.5(LG CNS), Kanana(카카오), Solar Pro 3(업스테이지), CLOVA Studio for GOV(네이버클라우드)가 각각 다른 경로로 공공 조달 채널을 확보하기 시작했습니다. 2026년 8월 AI법 시행과 맞물려 **국산 LLM 우선 조달** 환경이 조성될 전망입니다.

### 3. 보안·거버넌스가 기술과 동등한 조달 기준으로 격상

CSAP 인증, 폐쇄망 지원, AI 가드레일(Safeguard), 데이터 유출 방지를 갖추지 못한 솔루션은 공공 RFP 단계에서 탈락하는 환경이 됐습니다. AI 보안 특화 기업의 비중이 Directory Book 전체 기업의 약 15%를 차지합니다.

### 4. Vibe Coding — 기관장 레벨의 심리적 진입장벽 해소

행정안전부 황규철 실장(Claude), NIA 김영철 원장(Replit), 카카오 김세용 부사장(Lovable)이 직접 시연한 AI 바이브코딩 세션은 기술 데모가 아닌 **변화관리 이벤트**였습니다. 단, 프로토타입과 운영 서비스의 경계를 명확히 구분하는 거버넌스 설계가 다음 과제입니다.

### 5. 스타트업이 공공 AI 생태계의 새로운 주역

Directory Book E 카테고리(스타트업 혁신기술)는 18개 기업으로 전체에서 가장 큰 비중을 차지합니다. 민원 Agent(법틀 민트), 규제 모니터링(코딧 CODIT), 디지털 포용(투아트·닷·망고슬래브)처럼 **특정 공공 문제를 AI로 정밀하게 해결**하는 버티컬 특화 전략이 대기업 플랫폼과 병존하며 시장을 넓히고 있습니다.

---

## 기술 스택 (분석 도구)

- **분석 엔진**: Claude Sonnet 4.6 (Anthropic)
- **소스 파싱**: Markdown 텍스트 분석 + PDF 문서 파싱
- **출력 포맷**: Markdown, HTML (McKinsey 스타일 컨설팅 리포트)

---

## 라이선스 및 출처

본 프로젝트의 분석 결과물은 참고 목적으로 자유롭게 활용할 수 있습니다.  
원본 데이터(발표 자료·PDF)의 저작권은 각 발표사 및 행정안전부·NIA에 있습니다.

- 주관: 행정안전부 / NIA 한국지능정보사회진흥원
- 후원: KLID 한국지역정보개발원, KAIGA 한국인공지능정부협회, Korea Startup Forum
- 분석 기준일: 2026년 6월 24일 (제9회 전자정부의 날)
