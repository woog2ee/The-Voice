# The-Voice
ETRI 2021 Open API Project Repository   
Check out Presentation at [Link](https://github.com/woog2ee/The-Voice/blob/main/ETRI%202021%20Open%20API%20%EA%B2%B0%EA%B3%BC%EB%B3%B4%EA%B3%A0%EC%84%9C%20(%EA%B7%B8%EB%86%88%EB%AA%A9%EC%86%8C%EB%A6%AC%ED%8C%80).pdf)

## ๐ช Teammates
- Team name: **๊ทธ๋๋ชฉ์๋ฆฌํ**, The Voice
- **Seunguk Yu**: School of Computer Science & Engineering in CAU   
- **Yejin Kwon**: School of Applied Statistics in CAU   
- **Minju Kim**: School of Business & Economics in CAU   
- **Kiseong Lee**: Da Vinci College of General Education in CAU 

## ๐ก Prototype
### ๊ฐ์ฒด๋ช ์ธ์ ๊ธฐ๋ฐ ๋ณด์ด์คํผ์ฑ ํ์ง ๋ชจ๋ธ
์ค์๊ฐ ์ ํ์์ ๊ฐ์ฒด๋ช ์ธ์์ ํตํด ๋ณด์ด์คํผ์ฑ ์ํ๋๋ฅผ ์ค์๊ฐ์ผ๋ก ๊ฒ์ฌ
![thevoice_prototype](https://user-images.githubusercontent.com/80081987/137754280-baed0f39-70a8-4def-b726-b4e499378685.png)

## ๐ Pipeline
### 1. Data Crawling & Collecting
๊ธ์ต๊ฐ๋์ ๋ณด์ด์คํผ์ฑ ์งํด์ด ์ฌ์ดํธ์์ ๋ณด์ด์คํผ์ฑ ํ์คํธ ํฌ๋กค๋ง ๋ฐ ์ ์ฒ๋ฆฌ   
[AI Hub ์๋ด ์์ฑ ๋ฐ์ดํฐ](https://aihub.or.kr/aidata/30711)์์ ์๋ด ๋ฐ์ดํฐ ์์ง ํ ์ ์ฒ๋ฆฌ 

### 2. ETRI NER Tagging
[ETRI NER API](https://aiopen.etri.re.kr/guide_wiseNLU.php)๋ก ๋ณด์ด์คํผ์ฑ ๋ฐ ์ฝ์ผํฐ ํ์คํธ์์ ๋จ์ด๋ค์ NER ํ๊นํด ๋ฐ์ดํฐ ์ผ๊ด์ฑ์ ํ๋ณด

### 3. Sentence N-gram & Embedding
์ ํ ๋งฅ๋ฝ์ ํ์ตํ๊ณ ์ ๋ฐ์ดํฐ๋ฅผ ๋ฌธ์ฅ N-gram์ผ๋ก ๋ณํํ์ผ๋ฉฐ   
๋ฌธ์ฅ ํํ๋ ฅ์ ๊ทน๋ํํ๊ณ ์ Sentence Transformer ๋ฐ KoBERT ์ฌ์ฉ

### 4. Voicephishing Detection
๋น๊ต์  ์ ์ ๋ฐ์ดํฐ์๋ ์ ํฉํ๋ ๋จธ์ ๋ฌ๋ ๋ถ๋ฅ๋ชจ๋ธ ํ์ฉ   
๋ก์ง์คํฑ ํ๊ท, ๋์ด๋ธ ๋ฒ ์ด์ฆ, ๋๋คํฌ๋ ์คํธ๋ก ์คํ ๋ฐ ์ฑ๋ฅ ํ๊ฐ
