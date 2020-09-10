---
title:  "문장수준 임베딩(LDA)"
excerpt: "문장수준 임베딩 모델"
header:
  teaser: /assets/images/nlp/LDA.png

categories:
  - NLP
tags:
  - LDA
last_modified_at: 2020-09-10T10:00
---

##### 문장수준 임베딩     

| <center>구분</center>	| <center>종류</center>	|
| :--------------------	| :--------------------	|
| 1. 행렬분해		| 잠재의미분석(LSA)		|
| 2. 확률모형		| 잠재 디리클레 할당(LDA)	|
| 3. 뉴럴네트워크기반 모델	| Doc2Vec		|
|			| ELMo			|
|			| GPT			|
|			| BERT			|

##### 1. LDA (잠재 디리클레 할당)      

토픽별 단어의 분포, 문서별 토픽의 분포를 모두 추정  

![]({{ site.url }}{{ site.baseurl }}/assets/images/nlp/LDA.png   ){: .align-center} 

![]({{ site.url }}{{ site.baseurl }}/assets/images/nlp/LDA_1.png   ){: .align-center} 

![]({{ site.url }}{{ site.baseurl }}/assets/images/nlp/LDA_2.png   ){: .align-center} 

##### 1.1. LDA와 깁스 샘플링   

LDA가 각 단어에 잠재된 주제를 추론하는 방식을 살펴보자  

단어5개로 구성된 문서1의 모든단어에 주제(z)가 이미 할당돼 있다고 가정, 토픽수는 3개로 지정  

![]({{ site.url }}{{ site.baseurl }}/assets/images/nlp/LDA_3.png   ){: .align-center} 