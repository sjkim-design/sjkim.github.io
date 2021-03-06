---

layout: post
title:  "캐글 타이타닉 생존자 예측 "
summary: "Titanic"
author: KSJ
date: '2021-03-05 09:41:00 +0900'
categories: analytics
thumbnail: /imgages/ship-3401500_1920.png
---

캐글 필사를 시작하면서, 클래식한 Titanic data를 활용하여 DATA HANDLING, EDA, MODELING을 진행해 보려고 합니다.

-----







## Contents

1. [데이터 분석 문제 정의](#1-문제 정의)

2. [데이터 핸들링](#2. 핸들링)

3. [데이터 EDA](3.데이터EDA)

4. [모델링](#4. 모델링)

5. [마무리](#5.마무리)

   -----

   ## 1. 문제 정의



   타이타닉호에 탑승한 승객들의 데이터를 바탕으로 생존자를 예측하는 문제이다.

   ***

   ## 2. 데이터 핸들링

   핸들링에 필요한 파이썬 라이브러리인 `numpy`, `pandas` 등의 기본 라이브러리를 import하고 

   train/test데이터를 업로드한다.

   

   {% highlight python %}
   import pandas as pd
   import numpy as np

   train = pd.read_csv('train.csv')
   test = pd.read_csv('test.csv')

   {% endhighlight %}

데이터를 확인하기 위한 head를 실행한다.

{% highlight python %}

train.head()

{% endhighlight %}  



PassengerIdSurvivedPclassNameSexAgeSibSpParchTicketFareCabinEmbarked0103Braund, Mr. Owen Harrismale22.010A/5 211717.2500NaNS1211Cumings, Mrs. John Bradley (Florence Briggs Th...female38.010PC 1759971.2833C85C2313Heikkinen, Miss. Lainafemale26.000STON/O2. 31012827.9250NaNS3411Futrelle, Mrs. Jacques Heath (Lily May Peel)female35.01011380353.1000C123S4503Allen, Mr. William Henrymale35.0003734508.0500NaNS



ㅇㅇ

***
