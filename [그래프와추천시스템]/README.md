# 그래프와 추천 시스템

## 학습 주제

| 순서 | 주제                      |
| :--- | :------------------------ |
| 1    | 그래프와 추천 시스템 개요 |
| 2    | 그래프의 패턴 분석        |
| 3    | PageRank                  |
| 4    | 정보 확산과 Cascade       |
| 5    | 커뮤니티 탐지             |
| 6    | 기본 추천 시스템          |
| 7    | Node Embedding            |
| 8    | 고급 추천 시스템          |
| 9    | Graph Neural Network 기초 |
| 10   | Graph Neural Network 심화 |

## 학습 현황

| 자료                                                                                                     | 핵심 내용 요약                                                                                                                                     |
| :------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------- |
| [1. introduction](https://drive.google.com/file/d/1NXA00DG-bQA0SJzZwe1Ut47FB2eDdpnw/view?usp=sharing)    | 복잡계의 상호작용을 그래프로 표현하는 이유와, 정점·링크·그래프 수준의 대표적인 그래프 머신러닝 과제를 익혔다.                                      |
| [2. patterns](https://drive.google.com/file/d/1HLYY9xXDGgMWuVoCDlhlfY78emfxdhzm/view?usp=sharing)        | 실제 그래프가 무작위 그래프와 달리 작은 세상 효과, 두터운 꼬리의 차수 분포, 거대 연결 요소와 높은 군집 계수를 보인다는 점을 이해했다.              |
| [3. pagerank](https://drive.google.com/file/d/1jl9msk8CsffN87PM-ek82IYYDi2eyh2S/view?usp=sharing)        | 임의 보행 관점에서 링크 구조로 정점의 중요도를 계산하고, 감쇠 계수와 순간이동으로 스파이더 트랩과 막다른 정점 문제를 해결하는 PageRank를 학습했다. |
| [4. cascade](https://drive.google.com/file/d/13yEB5Ldn1nD7kWiqukrWaU-dxKmrUcey/view?usp=sharing)         | 정보·행동·고장의 전파를 독립 전파 모형과 선형 임계치 모형으로 설명하고, 탐욕 알고리즘으로 영향력 최대화 시드 집합을 찾는 방법을 익혔다.            |
| [5. community](https://drive.google.com/file/d/1qEpkyBl1QeCADIRtW390PKy88zsjyXW7/view?usp=sharing)       | 내부 연결이 밀집한 커뮤니티의 정의와 탐색 문제를 이해하고, 확률적 커뮤니티 모형과 중첩 커뮤니티를 다루는 방법을 학습했다.                          |
| [6. recommend_basic](https://drive.google.com/file/d/1Z_ePCivJCX_k1DJkG5vV3WiCrtDRnRQ4/view?usp=sharing) | 상품·사용자 프로필의 유사도를 쓰는 내용 기반 추천과 취향이 비슷한 사용자를 활용하는 협업 필터링, 그리고 MSE·RMSE 기반 평가를 익혔다.               |
| [7. node_embedding](https://drive.google.com/file/d/1MEB9LpDIUjAw7mkVQXPf6hEH5lY8GfXk/view?usp=sharing)  | 인접성·경로·이웃 중첩·임의 보행으로 정점 유사도를 정의하고, DeepWalk·node2vec으로 정점 임베딩을 학습하는 방식을 이해했다.                          |
| [8. recommend_adv](https://drive.google.com/file/d/1NY8P5EuVbBAh3cJ988P4hlUyn3ixE7Zh/view?usp=sharing)   | 사용자와 상품의 잠재 요인을 행렬 분해로 학습하고, 정규화·편향·시간 정보를 반영해 추천 정확도를 높이는 방법을 익혔다.                               |
| [9. gnn_basic](https://drive.google.com/file/d/1YuKPt4srQZ0azdQOFOBnaQd0f7l7dJXv/view?usp=sharing)       | 이웃 정점의 정보를 반복 집계하는 귀납식 표현 학습으로서 GNN의 구조·학습·활용을 이해하고, GCN과 GraphSAGE를 학습했다.                               |
| [10. gnn_adv](https://drive.google.com/file/d/1NsBO0HE-NzSPE8Z6-lNFpHqh89PXJs_q/view?usp=sharing)        | GAT와 그래프 수준 표현 학습을 다루고, 지나친 획일화와 그래프 데이터 증강처럼 기본 GNN의 한계를 보완하는 방법을 익혔다.                             |
