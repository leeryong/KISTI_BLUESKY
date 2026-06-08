# 🌌 BLUESKY

> **BLUESKY: Harmonizing Human and AI Collaboration**

---

## 🆕 최신 소식 (Latest News)

- **[NELLA](https://github.com/leeryong/NELLA)** — 문서만 주면 알아서 모델을 만들어주는 Agentic LLMOps 에이전트. **Docker 기반 설치 코드 공개** — `clone` 후 명령 몇 줄이면 로컬에서 바로 실행할 수 있습니다.
- **[ParserTry](https://github.com/leeryong/ParserTry)** — 21종+ PDF 파서를 웹 UI에서 즉시 실행·비교하는 도구. 텍스트·ML·OCR·VLM 계열 파서를 한 화면에서 돌려보고, 내 문서에 가장 맞는 파서를 직접 확인할 수 있습니다.
- **[Scarlet](https://github.com/leeryong/Scarlet)** — 다양한 문서·데이터를 스스로 탐색·정리하고 근거 기반 추론으로 답하는 멀티에이전트 지식 탐색·추론 시스템. *A Study in Scarlet*의 홈즈–왓슨 콤비처럼 왓슨이 지식베이스를 만들고 홈즈가 근거를 추론해 답변합니다.
- **[rhwp Agent Skills](https://github.com/leeryong/rhwp-Agent-Skills_by_BLUESKY)** — 한글 문서(HWP/HWPX)를 AI 에이전트가 직접 다룰 수 있도록 스킬화. 사람이 손으로 쓴 문서를 에이전트가 인식해 rhwp로 작성하며, 사람과 에이전트가 함께 작성하는 **rhwp-Agent**를 개발 중입니다.

---

## 📑 기술 · 시스템 목차

| 기술 · 시스템 | 소개 |
| --- | --- |
| 🗂️ **[ParserTry](https://github.com/leeryong/ParserTry)** <sub>· NEW</sub> | 21종+ PDF 파서 즉시 실행·비교 로컬 웹앱 |
| 🎩 **[Scarlet](https://github.com/leeryong/Scarlet)** | 멀티에이전트 지식 탐색 및 추론 시스템 (홈즈–왓슨) |
| ✍️ **[rhwp Agent Skills](https://github.com/leeryong/rhwp-Agent-Skills_by_BLUESKY)** | 한글 문서(HWP/HWPX)를 AI 에이전트가 다루는 스킬 |
| 🛠️ **[NELLA](https://github.com/leeryong/NELLA)** | 도메인 특화 LLM 제작 전 과정을 자동화하는 Agentic LLMOps **에이전트** |
| 📄 **[DOREA-X](https://github.com/leeryong/DOREA-X)** | 문서 이해·분석·보고서 작성 문서 중심 AI 에이전트 |

---

# 🤖 ARTWORK

## 🗂️ **ParserTry** &nbsp;<sub>· 최신 (NEW)</sub>

<div align="center">
  <a href="https://github.com/leeryong/ParserTry">
    <img src="https://raw.githubusercontent.com/leeryong/ParserTry/main/frontend/assets/concept_ko.png"
         alt="ParserTry — PDF 파서 비교 도구"
         width="90%"
         style="border: 1.5px solid #333; border-radius: 8px; box-shadow: 0 3px 8px rgba(0,0,0,0.25);" />
  </a>
</div>

<p align="center">
  <a href="https://github.com/leeryong/ParserTry"><b>🔗 ParserTry 바로가기</b></a>
</p>

**ParserTry**는 **21종+ PDF 파서를 웹 UI에서 즉시 실행·비교**하는 로컬 웹앱입니다. 모든 PDF에 하나의 파서가 최고가 아닙니다 — RAG 파이프라인 구축 전, 내 문서에 가장 잘 맞는 파서를 직접 확인할 수 있습니다.

주요 특징:

- 🗂️ **21종+ 파서 지원** — 텍스트(PyMuPDF·pdfplumber 등), ML 레이아웃(Docling·MinerU·Marker), OCR(PaddleOCR·EasyOCR), VLM(Claude·GPT·Gemini·Ollama)
- 📄 **문서 뷰어 + 오버레이** — PDF 원본 위에 파서가 인식한 요소를 색상 박스로 표시, 좌우 비교
- 💡 **파서 추천 분석** — 문서 특성(텍스트 레이어·이미지·표·언어)을 자동 분석해 적합도 순위 제시
- 📊 **실측 기반 비교표** — 샘플 4종 문서 직접 측정, 품질 × 처리속도 산점도 제공
- ⚙️ **확장형 구조** — 새로운 파서를 계속 추가 가능, `python run.py` 한 줄로 즉시 실행

---

## 🎩 **Scarlet**

<div align="center">
  <a href="https://github.com/leeryong/Scarlet">
    <img src="https://raw.githubusercontent.com/leeryong/Scarlet/main/scarlet_concept.png"
         alt="Scarlet 개념도 — 멀티에이전트 지식 탐색 및 추론 시스템"
         width="90%"
         style="border: 1.5px solid #333; border-radius: 8px; box-shadow: 0 3px 8px rgba(0,0,0,0.25);" />
  </a>
</div>

<p align="center">
  <a href="https://github.com/leeryong/Scarlet"><b>🔗 Scarlet 바로가기</b></a>
</p>

**Scarlet**은 다양한 문서와 데이터를 스스로 탐색·정리하고, 근거 기반 추론으로 답변을 생성하는 **멀티에이전트 지식 탐색 및 추론 시스템**입니다. 코난 도일의 *A Study in Scarlet*의 홈즈–왓슨 콤비를 모티프로, 두 에이전트가 역할을 나눠 협업합니다 — **왓슨이 정리하고, 홈즈가 추론합니다.**

주요 특징:

- 🩺 **왓슨(Watson)** — 다양한 문서·데이터를 수집·파싱·구조화해 지식베이스(Watson Journal)를 구축
- 🎩 **홈즈(Holmes)** — Watson Journal에서 근거를 검색하고 다단계 추론으로 신뢰 가능한 답변 생성
- 💬 사용자·홈즈·왓슨이 함께 대화하며 근거(evidence)와 추론 경로(reasoning trace)를 제시
- 🔌 멀티 LLM(Claude·OpenAI·Ollama) 및 다양한 데이터 보관소(VectorDB·DB·검색엔진·MCP 등) 연동

---

## ✍️ **rhwp Agent Skills**

<div align="center">
  <a href="https://github.com/leeryong/rhwp-Agent-Skills_by_BLUESKY">
    <img src="assets/rhwp-agent-skills.png"
         alt="rhwp Agent Skills — 손으로 쓴 문서를 에이전트가 인식해 rhwp로 작성"
         width="90%"
         style="border: 1.5px solid #333; border-radius: 8px; box-shadow: 0 3px 8px rgba(0,0,0,0.25);" />
  </a>
</div>

<p align="center">
  <a href="https://github.com/leeryong/rhwp-Agent-Skills_by_BLUESKY"><b>🔗 rhwp Agent Skills 바로가기</b></a>
</p>

**rhwp Agent Skills**는 한글 문서(HWP/HWPX) 편집기 [rhwp](https://github.com/edwardkim/rhwp)를 AI 에이전트가 직접 다룰 수 있도록 **스킬화(skill)** 한 모음입니다. 위 화면처럼 사람이 손으로 쓴 원문을 에이전트가 인식하고, 이 스킬을 사용해 rhwp 문서로 작성합니다.

주요 특징:

- 🧩 rhwp 편집 기능(글자/문단/표/도형, 페이지 설정 등)을 에이전트가 호출 가능한 스킬로 정리
- 🖥️ `?agent=1` 자동화 브리지로 rhwp 편집기 GUI를 직접 조작·검증
- ✍️ 사람과 에이전트가 함께 문서를 작성하는 시스템(**rhwp-Agent**)을 개발 중

---

## 🛠️ **NELLA**

<a href="https://github.com/leeryong/NELLA">
  <img src="https://raw.githubusercontent.com/leeryong/NELLA/main/assets/NELLA_Concept_Main.png"
       alt="NELLA 시연 이미지"
       width="90%"
       style="border: 1.5px solid #333; border-radius: 8px; box-shadow: 0 3px 8px rgba(0,0,0,0.25);" />
</a>
<p align="center">
<a href="https://github.com/leeryong/NELLA"><b>🔗NELLA 바로가기</b></a>
</p>

**NELLA** (Nifty-Enhanced LLMOps Agent)는 DOREA-X 이후의 새로운 확장 프로젝트로, 문서 기반 지능형 에이전트의 경험을 바탕으로 **도메인 특화 LLM 제작 전 과정을 자동화하는 Agentic LLMOps 에이전트**입니다.

DOREA-X가 문서 이해·분석·보고서 작성을 지원하는 문서 중심 AI 에이전트라면, NELLA는 문서를 기반으로 학습데이터 생성, 모델 선택, 파인튜닝, 평가, 대화 테스트까지 이어지는 **LLM 개발 전주기 자동화**를 목표로 합니다.

주요 특징:

* 문서 업로드만으로 SFT/DPO 학습데이터 자동 생성
* 자연어 대화 기반 모델 제작 요청 및 진행 제어
* 기반 모델 추천, LoRA/QLoRA 학습, 평가 자동화 지원
* Human-in-the-Loop 구조를 통한 자동화와 사용자 통제의 균형
* 기관 내부 문서 기반 도메인 특화 LLM 구축 지원

---

## 📄 **DOREA-X**

<div align="center">
  <a href="https://github.com/leeryong/DOREA-X">
    <img src="https://raw.githubusercontent.com/leeryong/DOREA-X/main/assets/logo.png" 
         alt="DOREA-X Logo" width="90%"/>
  </a>
</div>

<p align="center">
  <a href="https://github.com/leeryong/DOREA-X"><b>🔗 DOREA-X 바로가기</b></a>
</p>

**DOREA-X** (Document-Oriented Reasoning and Explanation Assistant)는 문서 이해부터 분석, 그리고 보고서 작성까지 전 과정을 지원하는 **문서 중심 AI 에이전트 시스템**입니다.

주요 특징:
- 📄 PDF 및 오피스 문서 등 복잡한 문서 구조 이해  
- 🧠 문서 기반 질의응답 및 추론 중심 상호작용  
- ✍️ 보고서 작성 및 지식 정리 지원  

단순한 검색을 넘어,  
**문서를 깊이 이해하고 AI와 함께 사고하는 협업 환경**을 지향합니다.

---

## 🚀 About BLUESKY

**BLUESKY**는 인간과 AI의 조화로운 협력을 탐구하는 공간 입니다. 최신 AI 기술을 탐색하고, 이를 연구 지원과 지식 발견, 실제 문제 해결에 활용할 수 있는 **실용적인 도구와 방법론으로 발전시키는 것**을 목표로 합니다.

이 리포지토리는 다음을 위한 열린 공간입니다:

- 최신 AI 패러다임 실험  
- 연구 업무를 지원하는 지능형 에이전트 설계  
- 인간의 창의성과 생산성을 확장하는 새로운 활용 방식 탐색  

---

## 🔄 Latest Direction

BLUESKY는 DOREA-X의 경험을 기반으로 지속적으로 확장되고 있으며,  
현재는 다음과 같은 방향으로 발전하고 있습니다:

- 자율적이고 적응적인 AI 에이전트  
- 인간의 작업 흐름과 긴밀하게 통합되는 AI 시스템  
- 연구 및 지식 플랫폼을 위한 확장 가능한 아키텍처  

이 리포지토리는 **최신 업데이트, 실험, 아이디어를 반영하는 살아있는 공간**입니다.

---

## 🌱 Vision

> **최신 AI 기술을 탐구하는 실험의 장이자,  
> 연구를 지원하는 플랫폼이며,  
> 혁신적인 AI 활용을 시도하는 살아있는 실험실**

---

## 📞 문의

- 이용 (ryonglee@kisti.re.kr)

