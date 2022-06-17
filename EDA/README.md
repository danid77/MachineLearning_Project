### 어떤 문제를 해결하고 싶은지

- 회귀 : FPS게임인 베틀그라운드 플레이어의 데이터를 통한 winPlacePerc(승률) 예측

1. 데이터에 대한 EDA를 통해 modeling에 활용 가능한 모양으로 전처리 진행

![image](https://user-images.githubusercontent.com/24274424/91469635-97729f80-e8ce-11ea-9ee5-264c73e94910.png)

  출처: 생활코딩

### EDA
1차 : 승률은 kill의 양에 따라서 바뀔 것이라는 가설을 세웠다. 그래서 killPlace, kills, killStreaks, weaponsAcquired, damageDealt 컬럼에 대해서 EDA를 진행하였다.<br>
  - 킬이 높을수록 승률이 올라갈 것이다.<br>
  - 무기 교체가 많을 수록 승률이 올라갈 것이다.<br>
  - killPlace가 낮을 수록 승률이 높을 것이다. <br>
  - damageDeal이 많을수록 승률이 높을 것이다. <br>
  위와 같은 가설을 세우고 데이터의 상태를 정검하였다. <br>
<br>
<br>

2차 : 1차에서 정검한 데이터에서 내가 맡은 컬럼의 이상치를 제거한다. 
  - kills의 99%가 7킬 이하이므로 나머지 상위 1%를 8로 묶는다.
  - killPlace는 승률과 관계가 매우 깊으므로 제거한다. 
  - weaponsAcquired는 거리과 관련에 있으므로 거리 담당자에게 넘긴다. 
  - killStreaks는 4킬 이상을 모두 4로 묶는다.
  - damageDealt는 이상치가 없다고 판단했다.
