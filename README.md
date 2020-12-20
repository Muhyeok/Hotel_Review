# Hotel_Review

학번: 201604045

이름: 김 무 혁

##### 중국문화데이터포트폴리오

## 호텔 리뷰 분석
### **분석 배경**

 최근 빅데이터를 활용하여 소비자에게 소비재 정보를 추천하거나 소비재를 이용한 다른 고객의 리뷰를 실시간으로 확인할 수 있는 등의 앱 기반의 비즈니스 시장의 변화가 빠르게 이루어지고 있는데, 호텔의 경우도 호텔의 시설이나 서비스 수준을 사전에 확인하는 것은 제한적이기 때문에 다른 사람의 온라인 리뷰에 대한 의존도가 높은 분야 중 하나임.

---

### **분석 목적**

 호텔 예약 사이트 내의 호텔 리뷰를 텍스트마이닝 방법을 통해 
만족과 불만족으로 강하게 나타난 단어들을 추출하고 분석해 
시설, 서비스, 입지 등 여러측면에서 호텔 만족도에 영향을 미치는
요인들을 다각도로 탐색해보고자 함. 이를 통해 최근 여행자들에게서 나타난 새로운 니즈가 무엇이고, 
호텔 만족도에 큰 영향을 미치는 요인이 무엇인지에 대해 파악하고자 함.

---

### **분석 대상 및 방법**

+ 데이터 수집 대상 : 트립어드바이저(호텔예약사이트) 내 제주도 호텔 리뷰(2019.01-2020.10)

+ 총 수집 건수 : 2,014

+ 분석 대상에 관한 형태소 분석 진행

**데이터스키마**

![데이터스키마_크기조절](https://user-images.githubusercontent.com/74213615/102676326-66510e80-41e0-11eb-8b1d-1de82b959b6e.png)

**형태소분석결과 피벗테이블 완성**

![형태소분석결과_크기조절](https://user-images.githubusercontent.com/74213615/102676423-d069b380-41e0-11eb-9ccf-1442bfa6782f.png)

---

### **데이터 분석**

* 명사/형용사/동사 별로 데이터 추출 진행_품사별 형태소분석

![품사별 형태소 분석](https://user-images.githubusercontent.com/74213615/102675759-f2ae0200-41dd-11eb-876f-facc8eea0c6f.png)

* 명사 추출 데이터의 시각화_워드클라우드

![호텔리뷰_시각화_워드클라우드](https://user-images.githubusercontent.com/74213615/102675847-491b4080-41de-11eb-9aa4-a7d6a27aebd9.png)

* Grouping 진행
  * 명사로 추출된 상위 20개 단어에 관하여 Grouping을 진행함. 
  * 분류의 기준은 시설/직원/사용자/지역/금액/해당사항 없음의 구분으로 나눔.
  
![image](https://user-images.githubusercontent.com/74213615/102676004-f0987300-41de-11eb-8bde-899746d7d8dc.png)

  * 상위 20개 명사의 명사에 관한 빈도 백분율_시각화 차트

![image](https://user-images.githubusercontent.com/74213615/102676090-453bee00-41df-11eb-9c5e-6cb29742b804.png)      



```
데이터스키마를 제외한 위의 모든 데이터 분석 진행에 관한 파일은 아래 파일에 시트(sheet)별로 정리하였음.

- 호텔리뷰_201604045_김무혁_형태소분석결과.xlsx
```

---

### **데이터의 해석 결과**

 호텔 사용자들은 호텔의 리뷰를 작성할 때, 해당 호텔의 시설(45%)에 대하여 가장 많은 후기를 작성하는 것으로 나타남. 특히, 객실(방)의 상태와 부대시설 등의 본인들이 사용한 시설에 관하여 후기를 남겨 다른 이용자가 도움이 될 수 있을만한 정보를 리뷰로 남김. 뿐만 아니라, 직원의 친절도 및 서비스와 관련된 리뷰(31%)가 다음의 빈도를 나타내었으며, 해당 호텔의 위치와 뷰 등이 소수의견(4%)으로 작성됨을 알 수 있음.
이로 미루어 볼 때, 호텔의 사용자들은 기본적인 호텔자체의 시설과 인프라에 관심을 가지며, 추후 재방문의 여부에서도 이러한 점을 가장 우선적을 고려한 다는 것도 확인됨. 호텔측에서도 이러한 점에 주목하여 객실의 청소상태와 어메니티, 부대시설의 노후화 등의 개선 및 시설 확충 등에 더욱 투자를 해야 할 것으로 예상할 수 있음.

---

##### **본 프로젝트 관련 발표영상**

[https://youtu.be/JGJVNthSVmA](https://youtu.be/JGJVNthSVmA)





