## 안녕하세요, 코드짜는 회계사 김준현입니다.

회계법인 실무와 프로그래밍을 결합해 반복 업무를 자동화하고,  
실질적인 문제를 코드로 직접 해결하는 데 관심이 있습니다.

---

## Projects

### 1. 미국 상무부 ACCESS 문서 자동 수집기
**[ACCESS-document-crawler](https://github.com/gimjunhyeon87-maker/ACCESS-document-crawler)**

반덤핑·상계관세(CVD) 조사 대응 업무 중, 실무자가 직접 클릭하며 수일이 걸리던
문서 수집 작업을 무인 자동화했습니다.

- 한국 관련 CVD 조사 24건(C-580-602~989), 약 23,000건의 조사 문서를 Selenium으로 자동 수집
- 체크포인트 저장으로 중단 후 재시작 가능, 바코드 기반 중복 감지로 재다운로드 방지
- 손상 파일 자동 복구 및 다운로드 완료 후 무결성 검증 스크립트 별도 작성
- 케이스번호·제출일·제출자·문서유형을 Excel로 자동 정리해 검색 가능한 형태로 재구성

**기술:** Python · Selenium · pandas · openpyxl

---

### 2. 무역구제 동향 자동 모니터링 시스템
**[trade-monitoring-system](https://github.com/gimjunhyeon87-maker/trade-monitoring-system)**

매일 수동으로 확인하던 주요 기관 동향 모니터링을, 별도 서버 없이 상시 자동 운영되는
시스템으로 전환했습니다.

- 미국 CBP, 무역위원회(KTC), 인도 DGTR 등 주요 기관 동향을 매일 오전 6시 자동 수집
- Gemini API로 원문을 AI 요약·분류 후 이메일 자동 발송
- Google Apps Script 트리거 기반으로 별도 인프라 비용 없이 상시 운영
- 팀원 대상 사용법 교육을 진행하고 실제 업무 프로세스에 도입

**기술:** Gemini API · Naver News API · Google Apps Script

---

### 3. 계정과목 자동 표준화 도구
**[account-standardizer](https://github.com/gimjunhyeon87-maker/account-standardizer)**

감사 실무에서 회사마다 제각각인 계정과목 표기를 표준 체계로 통일하는 전처리 작업을,
두 가지 방식으로 정량 비교하며 검증했습니다.

- 문자열 유사도 baseline(90.7%)과 생성형 AI(Claude API) 기반 의미 매핑을 비교
- 이름은 비슷하지만 회계적으로 다른 개념(미수수익 vs 매출채권 등), 표준 목록에 없는 항목을
  섞은 함정 케이스로 검증 신뢰도를 높임
- 1차 검증 95.3% 결과의 오답 원인을 "프롬프트 판단 지침 문제"와 "기준 데이터 정의 문제"로
  진단 → 프롬프트와 기준 데이터 수정 → 2차 검증 100% 달성
- 결과 확인에 그치지 않고 오류 원인을 구조적으로 진단·수정하는 과정을 정량적으로 검증

**기술:** Python · Claude API · difflib

---

## Skills

**프로젝트에서 사용**

| 분야 | 기술 |
|---|---|
| 언어 | Python |
| 플랫폼 | Google Apps Script |
| 라이브러리 | pandas, NumPy, Selenium, openpyxl |
| API 연동 | Gemini API, Claude API, Naver News API, ScraperAPI |

**자격증 과정에서 학습**

| 분야 | 기술 |
|---|---|
| AI / ML | Random Forest, SVM,  (AICE Associate) |
| 정량 분석 | 유전 알고리즘 기반 최적화, 몬테카를로 시뮬레이션, 이항트리 옵션가치평가 (재무빅데이터분석사 1급) |

## Certifications

한국공인회계사(KICPA) &nbsp;·&nbsp; 재무빅데이터분석사 1급 &nbsp;·&nbsp; SQLD &nbsp;·&nbsp; ADSP &nbsp;·&nbsp; AICE Associate
