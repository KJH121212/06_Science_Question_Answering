[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/f0ZBPJID)

# 과학 상식 RAG 기반 질의응답 시스템

## Team

| 김지후 | 팀원2 | 팀원3 | 팀원4 |
| :----: | :----: | :----: | :----: |
| [github.com/KJH121212](https://github.com/KJH121212) | [github.com/UpstageAILab](https://github.com/UpstageAILab) | [github.com/UpstageAILab](https://github.com/UpstageAILab) | [github.com/UpstageAILab](https://github.com/UpstageAILab) |
| 질문 분류기, 검색 흐름, 프롬프트 구성, UI 설계 | FAISS 색인 및 검색 로직 | Streamlit 앱 구성 | Solar API 연동 및 응답 처리 |

---

## 0. Overview

### Environment

- Python 3.10+
- FAISS
- LangChain
- Streamlit
- Upstage Solar API

### Requirements

pip install faiss-cpu  
pip install langchain  
pip install streamlit  
pip install openai  

---

## 1. Competition Info

### Overview

- 질문 및 대화 히스토리를 바탕으로 과학 문서를 검색하고, 해당 내용을 기반으로 적절한 응답을 생성하는 Retrieval-Augmented Generation 시스템 개발

### Timeline

- 2025.04.16 - Start  
- 2025.04.21 - Final Submission  

---

## 2. Components

- 질문 도메인 분류기  
- FAISS 기반 문서 벡터 검색기  
- LangChain PromptTemplate 설계  
- Solar API 응답 생성기  
- Streamlit 사용자 인터페이스  

---

## 3. Data description

### Dataset overview

- JSONL 형식의 과학 상식 문서  
- 제목, 본문 등 텍스트 기반 구성  

### EDA

- 문서 길이 분포 분석  
- 키워드 기반 문서 구성 확인  

### Data Processing

- 정규화, 문장 분리, 불용어 제거  
- 벡터 임베딩 및 색인화  

---

## 4. Modeling

### Model description

- RAG 구조 기반  
- 문서 검색 → Prompt 구성 → LLM 응답 생성  

### Modeling Process

1. 입력 질문 정규화 및 과학 도메인 여부 판별  
2. FAISS로 관련 문서 검색  
3. LangChain으로 프롬프트 템플릿 구성  
4. Solar API를 사용해 응답 생성  
5. UI에 출력 및 출처 문서 제공  

---

## 5. Result

### Leader Board

- MAP: 0.89  
- MRR: 0.89  
- 최종 순위: 1위  

### Presentation

- (발표자료는 제출 시 첨부 예정)  

---

## etc

### Meeting Log


### Reference

- LangChain Docs: https://docs.langchain.com/  
- FAISS: https://github.com/facebookresearch/faiss  
- Upstage Solar API: https://docs.upstage.ai/ko/solar
