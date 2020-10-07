---
title:  "문장수준 임베딩(ELMo)"
excerpt: "문장수준 임베딩 모델"
header:
  teaser: /assets/images/nlp/ELMo.png

categories:
  - NLP
tags:
  - ELMo
last_modified_at: 2020-09-13T13:00
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

##### 1. ELMo(Embeddings from Language Models)        

전이학습(transfer learning): 이미 학습된 모델을 다른 딥러닝 모델의 <span style="color:blue">입력값</span> 또는 부분으로 <span style="color:blue">재사용</span>하는 기법을 일컫는다.    

![]({{ site.url }}{{ site.baseurl }}/assets/images/nlp/ELMo.png   ){: .align-center} 

ELMo는 입력단어 시퀀스 다음에 어떤 단어가 올지 맞추는 과정에서 학습된다.  

![]({{ site.url }}{{ site.baseurl }}/assets/images/nlp/ELMo_1.png   ){: .align-center} 
