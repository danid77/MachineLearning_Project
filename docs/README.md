<h1> ML_Project</h1>

<h2> 주관: 중소기업벤처부 이어드림 스쿨 2기</h2>

---

<br>

![image](https://user-images.githubusercontent.com/86671456/171619107-8d5506bf-349e-4163-9694-c3ad99adac9d.png)

<h2>주제 : <a href='https://www.kaggle.com/competitions/pubg-finish-placement-prediction/overview'>PUBG Finish Placement Prediction (Kernels Only)</a></h2>

![image](https://storage.googleapis.com/kaggle-media/competitions/PUBG/PUBG%20Inlay.jpg)

<h2> Abstract</h2>
So, where we droppin' boys and girls?

Battle Royale-style video games have taken the world by storm. 100 players are dropped onto an island empty-handed and must explore, scavenge, and eliminate other players until only one is left standing, all while the play zone continues to shrink.

PlayerUnknown's BattleGrounds (PUBG) has enjoyed massive popularity. With over 50 million copies sold, it's the fifth best selling game of all time, and has millions<br> of active monthly players.

The team at PUBG has made official game data available for the public to explore and scavenge outside of "The Blue Circle." This competition is not an official or<br> affiliated PUBG site - Kaggle collected data made possible through the PUBG Developer API.

You are given over 65,000 games' worth of anonymized player data, split into training and testing sets, and asked to predict final placement from final in-game stats<br> and initial player ratings.

What's the best strategy to win in PUBG? Should you sit in one spot and hide your way into victory, or do you need to be the top shot? Let's let the data do the<br> talking!
<br>

<h2> Machine Learning Project </h2>

---


|  프로젝트 순서 |     내용    |
|:------------------:| -----|
|문제 정의|PUGB Bettle Ground 게임의 유저 승률 예측|
|데이터 수집|해당 Kaggle 대회의 제공된 데이터 |   
|데이터 전처리|Feature Engineering, 이상치 제거, 결측치 제거 |
|모델 학습|Modeling : LinearRegression, Lasso, Ridge, LGBMRegressor, XGBRegressor, CatBoostRegressor, RandomForestRegressor|
|모델 평가|캐글 채점|
|모델 성능 향상| 하이퍼파라미터, 데이터 전처리 |


<br>

<h3> Basic information</h3>

**공식기간: 2022.06.03 ~ 2022.06.21**

- 인원 : 5명
- 팀장 : 문석민
- 팀원 : 오세연, 윤상현, 진승범, 최윤아
- 데이터 : PUGB - train_V2.csv, test_V2.csv, simple_submission_V2.csv
- 역할 : EDA, Modeling, Hyperparameter Tuning
- 협업장소 : 스파크 플러스
- 소통 : 스파크 플러스
- 저장소 : git
- 개발환경 : vscode, jupyter notebook, Anaconda
- 언어 : python 3.9
- 라이브러리 : numpy, pandas, sklearn, catboost
- 시각화 라이브러리 : seaborn, matplotlib
