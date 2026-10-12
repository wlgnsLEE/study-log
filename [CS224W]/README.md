# CS224W: Machine Learning with Graphs

## 학습 주제

| 순서        | 주제                                         |
| :---------- | :------------------------------------------- |
| 1           | 그래프 머신러닝 개요와 그래프 표현           |
| 2           | 전통적인 그래프 머신러닝과 특성 설계         |
| 3           | Random Walk 기반 Node Embedding              |
| 4           | PageRank와 개인화된 노드 중요도              |
| 5           | 관계 기반 반지도 학습과 라벨 추론            |
| 6           | GNN 기초와 GCN·GraphSAGE                     |
| 7           | GNN의 메시지 전달·Attention과 깊은 모델 설계 |
| 8           | GNN 예측 과제별 설계와 학습·평가             |
| 9           | GNN의 표현력과 GIN 및 1-WL 검사              |
| 10          | 이종 그래프와 지식 그래프 완성               |
| 11          | 지식 그래프의 다중 홉 / 복합 질의 추론       |
| 12          | Motif 분석과 빈번한 부분 그래프 탐색         |
| 13          | Modularity와 중첩 커뮤니티 탐지              |
| 14          | 전통적인 그래프 생성 모델                    |
| 15          | GraphRNN·GCPN 기반 그래프 생성               |
| 16          | GNN의 표현력 강화와 적대적 공격              |
| 17          | 샘플링과 모델 단순화를 통한 대규모 GNN 학습  |
| 18 (보너스) | AliGraph와 산업 현장의 그래프 머신러닝       |
| 18 (보너스) | 생명과학 및 의료 분야의 그래프 머신러닝      |
| 19          | GNN 사전학습과 쌍곡 공간 표현과 모델 설계    |

## 학습 현황

| 자료                                                                                                                                    | 핵심 내용 요약                                                                                                                                                                                                                                                                                                    |
| :-------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [01-intro.pdf](https://drive.google.com/file/d/1_lwX5-uwunPxatYlW6ZxH5xL9dhahzwY/view?usp=drive_link)                                   | - 관계와 상호작용을 표현하는 그래프의 기본 개념 소개<br>- 문제에 맞는 노드·간선 정의와 그래프 표현 방식                                                                                                                                                                                                           |
| [02-tradition-ml.pdf](https://drive.google.com/file/d/1R8VDqGkwkptvDk_72R-Jw9RrSXs2m_-y/view?usp=drive_link)                            | - 노드·링크·그래프 수준의 수작업 특성 설계와 전통적인 머신러닝 모델 적용<br>- Graphlet과 WL kernel을 이용한 그래프 구조 비교                                                                                                                                                                                      |
| [03-nodeemb.pdf](https://drive.google.com/file/d/1-pv03uRKxHuFwWnNrDCDAjopCyItKmb5/view?usp=drive_link)                                 | - Random Walk를 이용한 노드 유사도 정의와 노드 임베딩 학습<br>- DeepWalk·node2vec으로 학습한 노드 표현을 다양한 예측 과제에 활용하는 방법                                                                                                                                                                         |
| [04-pagerank.pdf](https://drive.google.com/file/d/1DOAeSL1CMxlTd-nco9Jx3lWacAi3258F/view?usp=drive_link)                                | - 연결된 노드의 중요도를 반영하는 PageRank와 Random Walk의 정상 분포를 구하는 Power Iteration<br>- Teleportation으로 Dead end·Spider trap 문제를 해결하는 원리<br>- Personalized PageRank·Random Walk with Restart를 이용한 관련 노드 추천                                                                        |
| [05-message.pdf](https://drive.google.com/file/d/1sm2dr5-e8lRhi0G-l6px7Zc7Ko1kaJUo/view?usp=drive_link)                                 | - 일부 라벨과 이웃 노드의 상관관계를 이용한 반지도 노드 분류<br>- Relational Classifier·Iterative Classifier·Belief Propagation을 통한 라벨 추론                                                                                                                                                                  |
| [06-GNN1.pdf](https://drive.google.com/file/d/1F08KBnJnWL8MBmTHx0CWysaIumE4n7_A/view?usp=drive_link)                                    | - Shallow Embedding의 한계와 이웃 메시지 집계를 통한 다층 GNN의 노드 표현 학습<br>- GCN·GraphSAGE의 집계 방식과 지도·비지도 목적 함수를 이용한 학습                                                                                                                                                               |
| [07-GNN2.pdf](https://drive.google.com/file/d/187Jg0Ca2pJ0PrhC4k0tF7zQj103b_06k/view?usp=drive_link)                                    | - 메시지 계산과 집계를 기준으로 GCN·GraphSAGE·GAT의 차이를 비교<br>- Attention·Multi-head attention으로 이웃별 중요도를 반영하는 방법<br>- 깊은 GNN의 Over-smoothing 문제와 Skip connection을 통한 완화                                                                                                           |
| [08-GNN-application.pdf](https://drive.google.com/file/d/1e6xSsKsDs6fllmEhOab7pY-2lGgLXO9B/view?usp=drive_link)                         | - 노드 특성·그래프 구조 보강과 노드·간선·그래프 수준의 Prediction head<br>- 전역·계층적 Pooling과 과제에 맞는 목적 함수·평가 지표<br>- Inductive·Transductive 데이터 분할 및 링크 예측에서 메시지 전달용 간선과 정답용 간선을 구분하는 방법                                                                       |
| [09-theory.pdf](https://drive.google.com/file/d/1Kcz3pkXv2mC4aaNVtLBEq4As2hSbtwv8/view?usp=drive_link)                                  | - 이웃 다중집합 집계 함수의 단사성과 GNN의 표현력 관계<br>- Mean·Max aggregation의 구조 구분 한계와 Sum aggregation·MLP를 사용하는 GIN<br>- 1-WL 검사와 메시지 전달 GNN의 표현력 및 한계                                                                                                                          |
| [10-kg.pdf](https://drive.google.com/file/d/1Ecj0nG-zqOtopqhs5VH-_mbL6d-idbw8/view?usp=drive_link)                                      | - 이종 그래프에서 관계별 메시지 집계를 수행하는 R-GCN과 파라미터 공유<br>- TransE·TransR·DistMult·ComplEx를 이용한 지식 그래프 완성<br>- 대칭·역관계·합성 등 관계 패턴에 따른 임베딩 모델의 표현력 비교                                                                                                           |
| [11-reasoning.pdf](https://drive.google.com/file/d/1CVl5GAi8Gfsse25Bj12EWXFcgBhC7da1/view?usp=drive_link)                               | - 불완전한 지식 그래프에서 다중 홉 경로와 복합 조건 질의의 답을 추론하는 방법<br>- Query2box의 Box embedding과 관계 투영·교집합 연산<br>- AND / OR 질의를 논리합 정규형(DNF)으로 변환해 저차원 공간에서 처리하는 원리                                                                                             |
| [12-motifs.pdf](https://drive.google.com/file/d/1BTIfV2UB_cdxH3mP3rZbROJniD0wBLQL/view?usp=drive_link)                                  | - 반복되는 부분 그래프와 Motif의 개념 및 구조적 의미<br>- 차수를 보존한 Null model과 Z-score를 이용한 Motif의 통계적 유의성 평가<br>- Order embedding으로 부분 그래프 포함 관계를 학습하고 빈번한 구조를 탐색하는 방법                                                                                            |
| [13-communities.pdf](https://drive.google.com/file/d/1bE5jRcycOSSdmk5Vx9rpTdGXSjgaMBPS/view?usp=drive_link)                             | - Triadic closure, Weak/Strong edge 등 실제 커뮤니티에서 볼 수 있는 구조 소개<br>- Null model 대비 내부 연결의 밀도를 평가하는 Modularity와 이를 최대화하는 Louvain 알고리즘<br>- Community-Affiliation Graph Model, BigCLAM Model을 이용한 중첩 커뮤니티 탐지                                                    |
| [14-traditional-generation.pdf](https://drive.google.com/file/d/13c0h4TGRw3NlDmZVPFejglpw-r1FQT_K/view?usp=drive_link)                  | - 네트워크를 구분짓는 특성 (Degree distribution, Cluster coefficient, Path length, Connected component)<br>- 규칙적 연결에 무작위 연결을 더하는 Small-World 모델과 재귀적 Kronecker 그래프                                                                                                                        |
| [15-deep-generation.pdf](https://drive.google.com/file/d/1nV5-LdDCsMnpKSuIXFRFhEtlc9eDX0Cf/view?usp=drive_link)                         | - GraphRNN으로 그래프 생성을 노드·간선의 순차 생성 문제로 모델링<br>- GCPN에서 그래프 표현 학습과 강화학습을 결합해, 구조적 유효성을 지키면서 원하는 분자 특성을 최적화하는 목표 지향적 생성을 간략히 설명                                                                                                        |
| [16-advanced.pdf](https://drive.google.com/file/d/1RNXNlCSC014CI6a0pw9TjFe-WcRoGy_o/view?usp=drive_link)                                | - Anchor set과의 거리로 노드 위치를 표현하는 방법과 중심 노드를 구분하는 ID-GNN을 통해, GNN의 표현력을 강화하는 방법<br>- 노드 특성 및 간선을 조작하는 직접/간접 적대적 공격을 살펴보고, 작은 그래프 변화가 노드 분류 예측에 미치는 영향을 확인                                                                   |
| [17-scalable.pdf](https://drive.google.com/file/d/1f8fIiWjex2iWYi8z4l4c11d7N0X3d6Rs/view?usp=drive_link)                                | - 대규모 그래프에서 이웃 확장에 따른 계산량 증가를 소개하고, Neighbor Sampling과 Cluster-GCN으로 학습 범위와 메모리 사용을 줄이는 원리를 비교<br>- 비선형성을 제거한 Simplified GCN 및 미니배치 학습                                                                                                              |
| [18_GuestLecture_alibaba-aligraph-stanford.pdf](https://drive.google.com/file/d/1SwVX8ZIsO2BDHtRy9Rv0n4X37fhwB7e9/view?usp=drive_link)  | - 보너스 게스트 강의 <br> - 산업 현장에서의 그래프 머신러닝 실제 활용 사례 (AliGraph)                                                                                                                                                                                                                             |
| [18_BonusGuestLecture_marinka-zitnik-cs224w.pdf](https://drive.google.com/file/d/19J-FPhq9gCZG-4WVaOsJw9ZnF8oSSEIT/view?usp=drive_link) | - 보너스 게스트 강의 <br> - 그래프 머신러닝의 생명과학·의료 응용                                                                                                                                                                                                                                                  |
| [19-science.pdf](https://drive.google.com/file/d/1kzUZo9VVoZOBLT0NUDIVMEqtCiPLK4M4/view?usp=drive_link)                                 | - 라벨 부족 등의 제약이 있는 과학 분야에서 노드 및 그래프 수준의 사전학습을 결합해 도메인 지식을 학습하고 성능을 강화하는 원리<br>- 계층적·트리형 구조에 적합한 Hyperbolic space와 Hyperbolic GNN<br>- GNN design space와 task similarity를 체계적으로 비교해 새로운 과제에 적합한 모델 설계를 선택·전이하는 방법 |

## Colab 실습

| 자료                                                 | 실습 내용 요약                                                                                                                                                                                                                                                                             |
| :--------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [NetworkX.ipynb](./Colab/NetworkX.ipynb)             | 무방향·방향 그래프에서 노드와 간선, 가중치가 관계를 표현하는 방식을 실습했다.<br>노드의 차수와 이웃 집합을 살펴보며 그래프의 기본 구조를 이해했다.                                                                                                                                         |
| [CS224W_Colab_0.ipynb](./Colab/CS224W_Colab_0.ipynb) | GCN이 이웃 정보를 여러 층에 걸쳐 집계해 노드 임베딩을 학습하는 과정을 확인했다.<br>일부 노드의 라벨만 사용하는 반지도 학습을 통해 커뮤니티를 분류하고, 학습에 따른 임베딩 공간의 변화를 살펴봤다.                                                                                          |
| [CS224W_Colab_1.ipynb](./Colab/CS224W_Colab_1.ipynb) | 평균 차수·군집 계수·PageRank·근접 중심성을 계산하며 그래프의 연결 구조와 노드 중요도를 해석했다.<br>연결된 노드 쌍과 음성 샘플을 구분하는 링크 예측을 통해, 임베딩 내적이 연결 가능성을 나타내도록 노드 표현을 학습했다.                                                                   |
| [CS224W_Colab_2.ipynb](./Colab/CS224W_Colab_2.ipynb) | GCN으로 이웃 정보를 집계해 노드 특성을 예측하고, 평균 풀링으로 노드 임베딩을 하나의 그래프 표현으로 통합해 그래프 전체의 특성을 예측했다.<br>노드 분류와 그래프 분류의 예측 단위 차이를 이해하고, 정확도와 ROC-AUC로 모델을 평가했다.                                                      |
| [CS224W_Colab_3.ipynb](./Colab/CS224W_Colab_3.ipynb) | GraphSAGE의 이웃 평균 집계와 GAT의 이웃별 어텐션을 비교하며 메시지 전달을 통한 노드 표현 학습을 실습했다.<br>Inductive·transductive 학습의 데이터 분할 차이를 익히고, 링크 예측에서 메시지 전달용 간선과 학습 정답용 간선을 분리하는 방식을 살펴봤다.                                      |
| [CS224W_Colab_4.ipynb](./Colab/CS224W_Colab_4.ipynb) | 이종 그래프에서 노드·관계 유형에 따라 메시지를 구분하고, 유형별 이웃 정보를 집계해 노드 표현을 학습했다.<br>메시지 유형 간 평균 집계와 의미 수준 어텐션을 비교하며, 관계별 중요도를 학습해 노드 분류에 반영하는 원리를 살펴봤다.                                                           |
| [CS224W_Colab_5.ipynb](./Colab/CS224W_Colab_5.ipynb) | Neighbor Sampling으로 각 층의 이웃 일부만 집계하는 미니배치 학습을 실습하고, 샘플링 비율에 따른 예측 성능을 전체 그래프 학습과 비교했다.<br>Cluster-GCN의 클러스터 단위 학습을 통해 대규모 그래프 학습의 계산 범위를 줄이는 원리를 익히고, 커뮤니티 분할 방식에 따른 성능 차이를 살펴봤다. |
