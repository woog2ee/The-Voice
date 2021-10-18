# The-Voice
ETRI 2021 Open API Project 
Check out Presentation at [Link](https://github.com/woog2ee/The-Voice/blob/main/ETRI%202021%20Open%20API%20%EA%B2%B0%EA%B3%BC%EB%B3%B4%EA%B3%A0%EC%84%9C%20(%EA%B7%B8%EB%86%88%EB%AA%A9%EC%86%8C%EB%A6%AC%ED%8C%80).pdf)

## 👪 Teammates
- Team name: **그놈목소리팀**, The Voice
- **Seunguk Yu**: School of Computer Science & Engineering in CAU   
- **Yejin Kwon**: School of Applied Statistics in CAU   
- **Minju Kim**: School of Business & Economics in CAU   
- **Kiseong Lee**: Da Vinci College of General Education in CAU 

## 💡 Prototype
### 개체명 인식 기반 보이스피싱 탐지 모델
실시간 전화에서 대화 내용 텍스트화 및 개체명 인식을 통해 보이스피싱 위험도를 실시간으로 게재
![thevoice_prototype](https://user-images.githubusercontent.com/80081987/137754118-ae452db7-ef39-4500-ba0e-b8f4926af780.png)

## 🚂 Pipeline
### 1. Data Crawling & Collecting
금융감독원 보이스피싱 지킴이 사이트에서 보이스피싱 텍스트 크롤링 및 전처리   
[AI Hub 상담 음성 데이터](https://aihub.or.kr/aidata/30711)에서 상담 데이터 수집 후 전처리 

### 2. ETRI NER Tagging
[ETRI NER API](https://aiopen.etri.re.kr/guide_wiseNLU.php)로   
보이스피싱 및 콜센터 텍스트에서 단어들을 NER 태깅해 데이터 일관성을 확보

### 3. Sentence N-gram & Embedding
전화 맥락을 학습하고자 데이터를 문장 N-gram으로 변환했으며   
문장 표현력을 극대화하고자 Sentence Transformer 및 KoBERT 사용

### 4. Voicephishing Detection
비교적 적은 데이터에도 적합하는 머신러닝 분류모델 활용   
로지스틱 회귀, 나이브 베이즈, 랜덤포레스트로 실험 및 성능 평가
