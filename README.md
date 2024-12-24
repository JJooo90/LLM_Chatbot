# LLM_Chatbot

1. 유튜브 특정 채널에 대한 안내를 하는 챗봇 생성

## About Project
유튜버 AI 질의응답 챗봇 서비스 개발은  
AI 서비스를 1인 기획 및 개발한 프로젝트입니다.  

## Background knowledge
Llama 2: Open Foundation and Fine-Tuned Chat Models https://arxiv.org/pdf/2307.09288
<!-- - LLaMA (https://brunch.co.kr/@harryban0917/293) -->
<!-- https://docs.rbln.ai/ko/software/optimum/tutorial/llama_7b.html -->
## Project Task
- Chatbot 기본 모델은 LLAMA2 모델을 적용, 추가 학습은 한국어대화데이터셋(오피스데이터)를 사용
- Vector DB 사용 예정(학습 데이터 저장용 및 Chatbot 개인별 로그 저장용)
| batch size = 64  
| buffer size = 20000  
|epochs = 50  
- 데이터 수집 및 가공
- 의도 분류 모델 학습
- 질의 응답 내용 작성과 임베딩후 pt파일로 저장
- 사용자의 질문과 구축된 질문 리스트의 유사도 비교
- 챗봇 소켓 서버 구현
- 챗봇 API 서버 구현
- 추가적으로 개선하기

## Result
다음과 같이 챗봇 소켓, API 서버를 구현하고  
React로 구현한 어플리케이션에서 챗봇 서비스를 시연했습니다.  
<br>

<!--
참고 URL https://seokii.tistory.com/146
courpus github : 
1. https://github.com/ko-nlp/Korpora
2. https://github.com/songys/AwesomeKorean_Data

3. LAMMA2 Chatbot 관련 : https://dwin.tistory.com/150
-->