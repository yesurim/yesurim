# 노유림 | Data · AI 

##  Interests

- Data Analysis & Machine Learning
- Data Engineering & Preprocessing
- LLM / AI Agent / RAG  

---


##  Tech Stack

**Language**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-025E8C?style=flat-square)

**AI / Modeling**

![Machine Learning](https://img.shields.io/badge/Machine%20Learning-2E5C8A?style=flat-square)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-1C3D5A?style=flat-square)
![NLP](https://img.shields.io/badge/NLP-3B7A57?style=flat-square)

**LLM Application**

![RAG](https://img.shields.io/badge/RAG-1C7C54?style=flat-square)
![Prompt Engineering](https://img.shields.io/badge/Prompt%20Engineering-4B4B4B?style=flat-square)
![AI Agent](https://img.shields.io/badge/AI%20Agent-4B4B4B?style=flat-square)

**Backend / Infra**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logo=meta&logoColor=white)



---

##  Featured Projects

###  AI 에이전트 기반 응급실 병렬 통화 및 매칭 시스템 (팀 4인)
> 2025.11 ~ 2026.01 (3개월) · `Python` `Streamlit` `FastAPI` `WebSocket/SSE` `STT` `LLM` `Function Calling`

구급대원이 병원 수용 가능 여부를 확인하기 위해 **"병원 탐색 → 전화 확인 → 거절 시 재탐색"** 을 반복해야 하는 구조적 비효율에 주목한 프로젝트입니다.
**AI Agent 프로세스 설계 · 실시간 STT 기반 환자 정보 구조화 · 통화 자동화 로직**을 담당했습니다.

- **문제 재설계**: 반복 병목을 `입력–이해–판단–도구 실행–결과 반영` 흐름의 AI Agent 프로세스로 재정의
- **실시간 정보 구조화**: 음성 입력을 STT로 전사하고, LLM이 증상·활력징후·기본 정보·추가 요청사항 등 구조화된 필드로 변환
- **Context State 관리**: 새로 들어온 발화만 환자 상태에 누적·갱신 → 전체 발화 재분석 대신 **증분 처리로 응답 지연과 API 비용 절감**
- **Agent Action Loop**: 병원 후보 탐색 → 자동 발신 → 수용·거절·미응답 결과 저장 → 화면 반영 → 후속 탐색 판단
- **병렬화**: 병원별 독립 통화 세션을 구성해 여러 병원에 동시 확인 가능한 구조로 확장
- **피드백 루프**: STT 오인식·누락 정보를 사용자가 즉시 확인·보정할 수 있도록 UI 구성 (음성은 WebSocket, 상태 업데이트는 SSE)

---

###  RAG 기반 고령층 맞춤 복지 추천 서비스 (팀 5인)
> 2026.03 ~ 2026.06 (4개월) · `Python` `FastAPI` `MySQL` `FAISS` `OpenAI API`

여러 기관에 흩어진 복지 정보를 고령층이 **검색 대신 대화로 찾을 수 있게** 한 서비스입니다.
**RAG Baseline 설계 · Generation 고도화 / Prompt Engineering**을 담당했습니다.

- **하이브리드 검색**: FAISS 벡터 검색 + BM25 키워드 검색 결합 → 제도명·자격 조건처럼 키워드 일치가 중요한 항목 보완, 이후 **리랭킹**으로 답변 생성 단계 문서 품질 개선
- **응답 흐름 설계**: `질문 재작성 → 의도 분류 → 하이브리드 검색 → 리랭크 → 답변 생성 → 대화 요약`
- **프롬프트 고도화**: GPT-4.1 공식 Prompting Guide를 참고해 역할 부여·출력 형식·금지 규칙·Few-shot을 단계적으로 적용하고, **Answer Correctness / Faithfulness** 기준으로 비교·실험
- **멀티턴 & 예외 처리**: 직전 대화와 요약 정보로 조건을 유지해 연속 상담 가능 / 복지와 무관한 질문·부적절한 입력은 검색 단계로 넘기지 않고 별도 안내 응답
- **데이터 구조화**: 복지 정책 데이터를 수집·정제해 MySQL 저장, 문서 임베딩 후 FAISS 인덱스 구축


---

##  Education Experience

| 기간 | 기관 | 내용 |
| --- | --- | --- |
| 2025.07 ~ 2026.01 (6개월) | T아카데미 [SK플래닛] 빅데이터 분석가 과정 9기 | Python·SQL 등 데이터 분석 툴 학습, EDA·ML·DL 프로젝트, 기업 연계 프로젝트 |
| 2025.01 ~ 2025.02 (2개월) | LG Aimers 6기 | AI 교육 및 LG 실제 데이터 기반 AI 해커톤 (난임 환자 임신 성공 여부 예측) |

##  Awards

| 일자 | 수상 | 내용 |
| --- | --- | --- |
| 2024.11 | 개방형 클라우드 플랫폼 기반 서비스 개발 아이디어 공모전 | 아이디어 부문 **과학기술정보통신부장관상** |

##  Activities

| 기간 | 단체 | 내용 |
| --- | --- | --- |
| 2026.03 ~ 현재 | 데이터 분석 동아리 **MOMENTUM** | 스터디·공모전·프로젝트 참여, 정규 데이터 분석 세션 참여 및 후속 기수 세션 운영 예정 |
| 2023.05 ~ 현재 | 독서 토론 동아리 **Minerva** | 부회장 2년·회장 1년, 공식 Notion 페이지 제작·관리(일정·회의록·독서 목록·토론 자료 정리) |

##  Certifications

| 자격 | 취득 | 주관 |
| --- | --- | --- |
| 빅데이터분석기사 | 2025.07 | 한국데이터산업진흥원 |

---

##  Contact

- **Email**: [nyr97830506@gmail.com](mailto:nyr97830506@gmail.com)
- **GitHub**: [@yesurim](https://github.com/yesurim)
