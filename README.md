# 프로젝트 이름
"사족 보행 로봇 챌린지"

## 프로젝트 설명
Unity 환경에서 로봇 사족 보행 강화 학습 시뮬레이션입니다.
GitHub의 Unity-MLAgents Crawler의 내용을 참고하여 
사족 보행 로봇으로 디자인하여 학습을 진행했습니다.


## 목차
- 사전 설치
- 실행 방법

## 사전 설치
1) Unity Hub 프로그램의 설치가 필요합니다.
      * https://unity.com/kr/download

2) 설치된 Unity Hub에서 추가 - 디스크 프로젝트 추가를 선택합니다.
   첨부된 ml-agents폴더 내 Project 폴더를 선택합니다.
      * LocalPC\ml-agents\Project

   프로젝트를 추가하면 자동 선택되는 Unity 버전을 설치합니다.
      * Unity 버전 : Unity 2022.3.29f1

## 실행 방법
1) 추가한 프로젝트를 실행 후 상단의 플레이 버튼을 누릅니다.
    그러면 기본적으로 Robot_2가 적용된 Agent가 움직이기 시작합니다.

※ 학습된 Agent Asset 변경 방법
1) Unity 메뉴 중 Hierarchy의 DynamicPlatform 토글을 열람합니다.
2) Robot을 선택합니다.
3) Inspector 정보 중 Behavior Parameters 토글을 열람합니다.
4) 해당 정보 내 Model을 찾습니다. (위치 기억)
5) Unity 메뉴 중 Project에서 아래 경로의 폴더를 찾습니다.
      * Assets\ML-Agenst\Robot\TFModels
6) 해당 폴더의 Asset 중 원하는 Asset을 선택하여
   Behavior Parameters의 Model에 Drag&Drop을 진행합니다.
7) 상단 플레이 버튼을 눌러 차이점을 확인합니다.

※ TFModels Asset의 대한 정보
  * Robot_1 : 천만 Step으로 학습한 모델
  * Robot_2 : 약 1억만 Step으로 학습한 모델 

이상입니다.