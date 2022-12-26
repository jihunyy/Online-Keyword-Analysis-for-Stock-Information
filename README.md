## 💡 Prototype
Designed by [Adobe XD](https://www.adobe.com/kr/products/xd.html)

### 1. M-able mini와 오해가 만나다
MZ세대를 타겟으로 kb증권에서 런칭된 M-able mini에 **오늘의 해시태그** 서비스 추가
![image](https://user-images.githubusercontent.com/80081987/132034685-32163dc5-3ab3-41b2-8253-cb12c27e871a.png)

### 2. 일별 언급량으로 많이 언급된 종목이 무엇인지 한눈에
네이버뉴스, 다음뉴스, 디시인사이드 주식갤러리, 네이버 종토방, 유튜브에 언급된 종목의 일별 언급량을 한번에 확인
![image](https://user-images.githubusercontent.com/80081987/132034702-2a4d3a87-5cdd-42c6-afe1-6cead4833829.png)

### 3. 종목에 대한 키워드 분석과 감성분석을 한눈에
종목별 **오늘의 해시태그**와 그에 따른 연관어가 무엇이며 감성분석 결과가 어떻게 되는지 한번에 확인
![image](https://user-images.githubusercontent.com/80081987/132034722-42c1078f-a2de-464e-be03-2f40d85d977f.png)

## 🚂 Pipeline
### 1. Data Crawling & Preprocessing
네이버뉴스, 다음뉴스, 디시인사이드 주식갤러리, 네이버 종토방, 유튜브에   
종목이 언급된 게시글 및 영상의 제목/본문/댓글을 Selenium과 BeautifulSoup으로 크롤링

### 2. Text Analyzing
각 종목당 일별 언급량 및 제시된 기간의 언급량 변동 추이 시각화   
빈도수를 기반으로 오늘의 해시태그, 오해 선정 및 오해 연관어 선정

### 3. Sentiment Analysis
직접 얻은 10일치 데이터와 kb-albert를 이용하여 감성분석 모델 학습을 진행   
오늘의 해시태그, 오해 연관어가 포함된 텍스트에 모델을 적용해 주식 종목의 오피니언 마이닝
