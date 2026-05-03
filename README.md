# Kangxi-MBA-Association-Rule-Mining-
## Abstract

This project applies unsupervised association rule mining to the *Veritable Records of the Kangxi Emperor* (聖祖仁皇帝實錄, 1661–1722) to uncover co-occurrence patterns among classical Chinese terms reflecting institutionalized ritual and administrative structures.

A four-stage pipeline was constructed: (1) 759 monthly word-frequency CSVs were merged into 102,861 entries (35,100 unique terms); (2) each term was classified via DeepSeek into eight NER categories (PER, LOC, OFF, GRP, DATE, SYS, EVT, NONE), yielding 4,903 analytically meaningful terms; (3) 758 monthly transactions were constructed (mean ≈ 28 items); (4) FP-Growth (min_support=0.05, min_confidence=0.5, min_lift=1.5) produced 1,475 association rules.

The principal finding concerns *朝鮮國王* (King of Joseon): in 98.2% of months in which this term appears, *堂子* (the Manchu imperial shrine) and *正月* / *元旦* / *朔* (the lunar New Year) co-occur, with five rules attaining confidence = 1.0 and lift = 12.85–13.06. This quantitatively demonstrates that Joseon tributary memorials were structurally embedded within the Manchu New Year rites of the Qing court, rather than functioning as a discrete diplomatic protocol — providing empirical support for the New Qing History thesis that Qing governance retained a distinctly Manchu ritual framework even in its handling of Sino-centric tributary relations.

---

## 초록 (한국어)

본 프로젝트는 청 강희제 통치기(1661-1722)의 『성조인황제실록』(聖祖仁皇帝實錄)을 대상으로 비지도 연관규칙 분석을 수행하여, 한문 단어 간의 동시 출현 패턴이 반영하는 의례적·행정적 구조를 정량적으로 추출하였다.

분석은 4단계 파이프라인으로 구성된다. 월별 단어 빈도 CSV 759개를 통합하여 102,861행, 35,100 고유 단어 코퍼스를 구축하였고, DeepSeek 언어모델을 활용해 8개 개체명 범주(인물·지명·관직·집단·날짜·제도·사건·기타)로 분류하였다. NONE 제외 후 4,903 단어를 758개 월별 트랜잭션(평균 28개 단어)으로 재구성한 뒤, FP-Growth 알고리즘(min_support=0.05, min_confidence=0.5, min_lift=1.5)을 적용하여 1,475개의 연관규칙을 도출하였다.

핵심 발견은 *朝鮮國王*(조선국왕) 관련 패턴이다. 동 단어가 등장하는 월의 98.2%에서 *堂子*(만주 황실 제사장)와 *正月*/*元旦*/*朔*(정월 초하루)이 동시 등장하며, confidence=1.0의 룰이 5건, lift는 12.85-13.06에 달한다. 이는 조선의 외번 표문 의식이 청 조정의 만주식 신년 의례 구조에 정형화되어 편입되어 있었음을 정량적으로 입증하는 결과로, 청 황실이 중화적 조공 관계조차 만주식 의례 틀 안에서 운용했다는 New Qing History 학파의 가설에 경험적 근거를 제공한다.

---
<img width="2520" height="1979" alt="01_network" src="https://github.com/user-attachments/assets/d96814cf-4817-48f2-8717-a82268c02faf" />
---


## Citation

If you use this code or data in your research, please cite:

[김형민] (2026). 청성조실록 한문 장바구니 분석.
[https://github.com/a26532198-collab/Kangxi-MBA-Association-Rule-Mining-/tree/main]

