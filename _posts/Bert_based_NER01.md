---
layout: single
title:  "BERT 모델 기반 개체명 인식(NER)"
categories: DeepLearning
tag: [Python, MachineLearning, DeepLearning, BERT]
toc: true
author_profile: false # true
sidebar:
    nav: "docs"
search: true
---

**[주의]** [개인 연구 기록 목적의 게시글로 비공개될 예정임]
{: .notice--danger}

# 딥러닝 기반 문서 유형 분류, 주소 인식 및 정제

**연구를 진행할 때, 기록하면서 정리를 해왔어야 했는데, 거의 완성되어 갈 때즈음 정리하려니 머리 아프다.**



<div class = "notice--success">
<h4>코드는 모두 모듈화하였으며, 구성은 다음과 같다.</h4>
<ul>
    <li>config - 문서 유형 분류와 주소 정제를 위한 공통 환경 설정(중요)</li>
    <li>model - 문서 유형 분류와 주소 추출 및 검증에 활용할 모델</li>
    <li>classify_doc - 사전 정의 라이브러리 기반 문서 분류 훈련 및 테스트  </li>
    <li>address_Test - 사전 정의 라이브러리 기반 주소 훈련 및 테스트</li>
    <li>ner - 사전 정의 라이브러리 기반 개체명 인식</li>
    <li>bert_address_test_main - 구축한 BERT 기반 주소 검증</li>
    <li>bert_classify_main - 구축한 BERT 기반 유형 분류 검증</li>
    <li>bert_ner_main - 구축한 BERT 기반 개체명 인식 검증</li>
</ul>
</div>

