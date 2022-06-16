1. 1차 모델링(ML0607_originData) : 원본데이터에서 object 자료형의 feature를 제거한 데이터를 활용해서 다양한 모델링을 진행했다.
    LinearRegression : 0.09749725456174148
    Lasso            : 0.12611457976813364
    Ridge            : 0.09749726114862003
    lightGBM         : 0.0640798346537524
    XGBoost          : 0.06293506258407007
    CatBoost         : 0.061975692337954684

2. 1차 EDA(ML0608_EDA_1) : 팀원들의 각자 EDA를 진행하여 얻은 인사이드를 활용하여 전처리를 진행했다. 
3. 2차 모델링(ML0609_featureData_1) : 1차 EDA에서 전처리한 데이터를 활용하여 다양한 모델링을 진행했다. 
    LinearRegression : 0.1048
    Lasso            : 0.1263
    Ridge            : 0.1048
    lightGBM         : 0.0674
    XGBoost          : 0.0681
    CatBoost         :

4. 캐글제출(ML0609_featureData_2) : 1차 EDA에서 전처리한 데이터를 미흡한 부분을 정리하여 데이터를 생성했다. 
   이를 활용하여 다양한 모델링을 진행했다. 또한 캐글에 재출하기 위하여 Test 데이터를 활용하여 각 아이디에 대한 승률의 최종 결과값을 얻었다. 
    점수 : 0.068

4. 2차 EDA(ML0612_EDA_2) : 성능을 개선 시키기 위해서 캐글을 참조하여 인사이트를 얻었다. 각자 진행한 EDA를 취합하여 전처리를 진행하였다. 
   전처리는 groupId 별로 groupby를 진행한 다음 각 feature의 이상치를 제거하였다. 
5. 3차 모델링(ML0614_featureData_3) : 2차 EDA에서 전처리한 데이터를 활용하여 다양한 모델링을 진행하였다. 
    LinearRegression : 0.1058
    Lasso            : 0.2588
    Ridge            : 0.1058
    lightGBM         : 0.0808
    XGBoost          : 0.0795
    CatBoost         : 0.0795

6. 3차 EDA : 2차 모델링보다 성능이 떨어졌다. 다음 과정을 진행하기 위해서는 성능이 이전보다 더 좋게 나와야한다. 때문에 캐글의 전치리가 잘 된 코드를 참고하여 전처리를 진행하였다. 
   전처리는 groupId 별로 groupby를 진행한 다음 각 group의 feature 평균값을 적용하여 데이터를 생성했다.  

7. 4차 모델링(ML0614_featureData_4) : 3차 EDA에서 전처리한 데이터를 활용하여 다양한 모델링을 진행하였다.
    LinearRegression : 0.0581
    Lasso            : 0.2589
    Ridge            : 0.0581
    lightGBM         : 0.0466
    XGBoost          : 0.0436
    CatBoost         : 0.0417
   
   처음 모델링보다 약 0.02가량 값이 낮아져 성능이 더 좋아졌다. 

8. 나는 lightGBM과 CatBoost의 hyperParameter Tuning을 진행한다. 
