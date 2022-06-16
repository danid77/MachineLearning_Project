<p>
1. 1차 모델링(ML0607_originData) : 원본데이터에서 object 자료형의 feature를 제거한 데이터를 활용해서 다양한 모델링을 진행했다.<br>
    LinearRegression : 0.09749725456174148 <br>
    Lasso            : 0.12611457976813364 <br>
    Ridge            : 0.09749726114862003 <br>
    lightGBM         : 0.0640798346537524 <br>
    XGBoost          : 0.06293506258407007 <br>
    CatBoost         : 0.061975692337954684 <br>
 </p>

<p>
2. 1차 EDA(ML0608_EDA_1) : 팀원들의 각자 EDA를 진행하여 얻은 인사이드를 활용하여 전처리를 진행했다. <br>
3. 2차 모델링(ML0609_featureData_1) : 1차 EDA에서 전처리한 데이터를 활용하여 다양한 모델링을 진행했다. <br>
    LinearRegression : 0.1048<br>
    Lasso            : 0.1263<br>
    Ridge            : 0.1048<br>
    lightGBM         : 0.0674<br>
    XGBoost          : 0.0681<br>
    CatBoost         : 0.0668<br>
</p>

<p>
4. 캐글제출(ML0609_featureData_2) : 1차 EDA에서 전처리한 데이터를 미흡한 부분을 정리하여 데이터를 생성했다. <br>
   이를 활용하여 다양한 모델링을 진행했다. 또한 캐글에 재출하기 위하여 Test 데이터를 활용하여 각 아이디에 대한 승률의 최종 결과값을 얻었다. <br>
    점수 : 0.068<br>
</p>

<p>    
4. 2차 EDA(ML0612_EDA_2) : 성능을 개선 시키기 위해서 캐글을 참조하여 인사이트를 얻었다. 각자 진행한 EDA를 취합하여 전처리를 진행하였다. <br>
   전처리는 groupId 별로 groupby를 진행한 다음 각 feature의 이상치를 제거하였다. <br>
5. 3차 모델링(ML0614_featureData_3) : 2차 EDA에서 전처리한 데이터를 활용하여 다양한 모델링을 진행하였다. <br>
    LinearRegression : 0.1058<br>
    Lasso            : 0.2588<br>
    Ridge            : 0.1058<br>
    lightGBM         : 0.0808<br>
    XGBoost          : 0.0795<br>
    CatBoost         : 0.0795<br>
</p>

<p>    
6. 3차 EDA : 2차 모델링보다 성능이 떨어졌다. 다음 과정을 진행하기 위해서는 이전보다 좋은성능이 출력되어야 한다. <br>
   때문에 캐글의 전치리가 잘 된 코드를 참고하여 전처리를 진행하였다. <br>
   전처리는 groupId 별로 groupby를 진행한 다음 각 group의 feature 평균값을 적용하여 데이터를 생성했다.  <br>
</p>

<p>
7. 4차 모델링(ML0614_featureData_4) : 3차 EDA에서 전처리한 데이터를 활용하여 다양한 모델링을 진행하였다.<br>
    LinearRegression : 0.0581<br>
    Lasso            : 0.2589<br>
    Ridge            : 0.0581<br>
    lightGBM         : 0.0466<br>
    XGBoost          : 0.0436<br>
    CatBoost         : 0.0417<br>
   
   처음 모델링보다 약 0.02가량 값이 낮아져 성능이 더 좋아졌다. <br>
</p>
 
<p>
8. 나는 lightGBM과 CatBoost의 hyperParameter Tuning을 진행한다. <br>
</p>
