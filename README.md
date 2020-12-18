# Best Practice

SETB 소프트웨어 개발에 필요한 Best Practice를 만들었습니다. 
Best Practice에는 개발 프로세스, 테스팅, 이슈 관리, 품질 관리, 형상 관리, 프로젝트 관리, 개발 도구, 통합 및 배포등을 포함하고 있습니다.

# 목차

- [Best Practice](#Best-Practice)
- [목차](#목차)
- [팀원 소개](#팀원-소개)

- [소프트웨어 개발](#소프트웨어-개발)
    - [개발 프로세스](#개발-프로세스)
    - [테스팅](#테스팅)
    - [이슈 관리](#이슈-관리)
    - [품질 관리](#품질-관리)
    - [형상 관리](#형상-관리)
    - [프로젝트 관리 및 협업 도구](#프로젝트-관리-및-협업-도구)
    - [개발 도구](#개발-도구)
    - [통합 및 배포](#통합-및-배포)
            
  
 - [Space Invader](#Space-Invader)
    - [pause](#pause)
    - [난이도 선택](#난이도-선택)
    - [멀티플레이](#멀티플레이)
    - [점수 기록](#점수-기록)
    - [점수 리셋](#점수-리셋)
    - [인터페이스 수정](#인터페이스-수정)

----------


# 팀원 소개
> 길정민_2019095414_[kjmin622](https://kjmin622.github.io)<br>
> 김동우_2019042351_[kim-dong-woo](https://github.com/kim-dong-woo)<br>
> 김혜원_2019028313_[iopopoi](https://iopopoi.github.io)<br>
> 이성민_2019000773_[Lee-SungMin](https://lee-sungmin.github.io)<br>
> 이현지_2019052251_[huskycat1202](https://huskycat1202.github.io)
<br>

# 소프트웨어 개발
## 개발 프로세스
* Scrum

>계획, 개발 등 최소 단위의 사이클인 스프린트를 활용해 수행한다. 백로그를 통해 목표와 그를 위한 작업목록을 확인한다.

<!-- 스크럼 -->
* Kanban

>작업 목록을 간판에 적어 시각화 해 업무 파악을 쉽게 돕는다. 

<!-- 칸반 -->

### 개발 프로세스 :  Scrum & Kanban
>1~4주 정도의 기간을 하나의 sprint(개발주기)로 하여 작업을 진행한다. 개발 기간이 길고 작업의 우선 순위가 분명하다면 sprint로 나누어 작업을 진행한다. 하나의 sprint(주기) 안에서는 보드를 통해 작업, 일정 등을 공유한다. 각 보드에는 진행중, 완료됨 등의 표시를 통해 프로젝트의 진행과정을 표현한다.

## 테스팅
* Junit

>자바 전용 유닛 테스트 프레임워크이다.  단위 모듈별(메소드 등) 테스트가 가능하여, 코드의 품질이 보장된다. 정확한 단위 테스트가 가능하여, 통합 테스팅 시 모듈통합에 의해 발생하는 결함을 줄인다. 다른 모듈에 의존하지 않고, 원하는 모듈만 임의의 순서대로 수행할 수 있다. JFeature(요구사항,개발도구)와 통합되어 요구사항의 정확한 구현 비율을 알 수 있다.	

<!-- Junit -->

* EMMA

>JAVA 프로그램을 위한 Code coverage 도구로, Code coverage를 클래스, 메소드, 라인, 블록 단위로 측정 및 보고한다.( Code coverage는 테스트를 수행했을 때 실제로 실행된 코드의 비율을 측정하여 그 테스트의 효과를 평가하는 기법이다.) 또한 개별 클래스 파일이나 jar 파일 전체, 또는 그 일부를 선택적으로 검사할 수 있다. 정적, 동적 분석이 가능하고 결과를 Text, HTML, XML 등 형태의 보고서로 출력해 준다.
 
### EclEmma & JUnit
>프로그램 실행 또는 테스팅에 따른 Coverage 테스트 결과를 표로써 출력해준다. Coverage 결과를 소스코드 위에서 색으로 보기 쉽게 나타내준다.  (검증됨 : 녹색, 부분적으로 테스트됨 : 노란색, 테스트가 안됨 : 빨간색)HTML, XML, text 등으로 Export할 수 있다. 

<!-- Emma-->

## 이슈 관리
* JIRA
>Atlassian사에서 개발한 issue Tracking System으로,  버그 추적 시스템에서 시작되어서 현재는 버그뿐만 아니라 일반적인 이수와 프로젝트 관리를 지원한다. 이슈 관리,버그추적, 프로젝트 관리등의 기능이 제공되는 소프트웨어이며, 최대 10명까지 무료로 프로젝트를 진행 할 수 있다. 다양한 언어를 지원한다. 특정 이슈를 누가 발견했는지, 누가 해결하는지, 이슈는 현재 어떤 상태인지 한눈에 확인하고 관리 할 수 있고, 이슈에 대한 역할과 임무를 분명히 할 수 있다. 소스 혹은 이미지 수정 내역을 남길 수 있다는 점이 편리하다. 이슈 관리를 통해 프로젝트관리 또한 진행 할 수 있다. 칸반, 스크럼등 보드의 종류를 선택하여 프로젝트를 진행 및 관리한다.
 
<!-- Jira -->

## 품질 관리
* PMD ( IntelliJ Plug-in )

>자바 컴파일러가 잡아내지 못하는 버그나 잘못된 코드 패턴을 찾아주는 정적 코드 분석 도구이다.
IntelliJ에서 PMD Plug-in을 설치해 사용한다. 

<!-- PMD -->



## 형상 관리
* Git
>Git은 컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 분산 버전 관리 시스템이다. 소프트웨어 개발에서 소스 코드 관리와 변경사항의 지속적 추적을 위해 사용된다. 빠른 수행 속도와 브랜치를 이용한 작업이 유용하다.

branch 종류

>master : release가 일어나는 branch<br>
develop : 다음 버전을 개발하는 branch<br>
feature : 특정기능을 개발하는  branch<br>
release : 이번 버전을 준비하는 branch<br>
hotfix : master에서 발생한 버그를 수정하는 branch<br>
bugfix : release branch에서 발생한 버그를 수정하는 branch
 
<!-- Git -->

## 프로젝트 관리 및 협업 도구
* Jira
>버그 추적, 이슈 추적, 프로젝트 관리 기능을 제공하는 소프트웨어로 특정 이슈를 누가 발견했는지, 누가 해결해야 하는지, 이슈는 현재 어떤 상태인지 파악하고 한 눈에 해결 및 관리할 수 있다. 단순히 메일이나, 구두로 업무를 진행하는 것보다 한눈에 프로젝트 팀원들의 작업 현황을 확인하고 스케줄이나 우선순위를 조절할 수 있다. 실무자의 경우는 이슈에 대한 역할과 임무를 분명히 할 수 있으며, 협업 시 불필요한 커뮤니케이션 비용을 줄일 수 있다. 또한, 이슈 해결에 대한 히스토리가 남기 때문에 후에 비슷한 이슈가 발생했을 때 처리 과정을 되짚어 볼 수 있다. 작업 진행(Workflow)은 ‘이슈’가 생성되고 완료될 때까지의 상태 변화를 의미하며 강력한 트래킹을 제공한다.

<!-- Jira -->
 
* Jandi
>업무용 협업툴로 업무 / 팀별 그룹 채팅, 프로젝트 관리, 파일 공유 및 관리, 외부 서비스 연동 기능을 지원하는 클라우드 기반 협업 소프트웨어다.

<br>

생산성 향상을 위한 핵심 기능
> * 스마트 검색 기능<br>
> * 메시지 / 파일 히스토리로 업무 파악<br>
> * 즐겨찾기 기능<br>
> * 잔디 드라이브 기능으로 파일관리<br>
> * 토픽, 멘션, 파일 댓글, 파일 공유, 외부 게스트 초대 등 협업기능<br>
> * 관리자의 접근 권한 조정 기능<br>
> * 기존 타 서비스 연동<br>
> * PC, 모바일 기기에 최적화
<!-- Jandi --> 
 
## 개발 도구
* IntelliJ
>IntelliJ는 JetBrains사에서 제작한 상용 자바 통합 개발 환경이다. 모든 기능을 사용할 수 있는 얼티밋 에디션은 유료로 제공되지만, 학생임을 인증하면 무료로 사용할 수 있다. 상용 IDE인 만큼 기능이 많아, 빠른 개발이 가능하다. IntelliJ의 성장에 따라, 이클립스에서만 사용가능하던 프레임워크들도 오늘날에는 대부분 IntelliJ 또한 지원한다.

## 통합 및 배포
* GIthub Action
>Github의 소프트웨어 WorkFlow 자동화 도구로, YAML을 기반으로 사용하는 만큼 간단한 코드로 workflow를 짤 수 있다. Github에 push/pull request되거나 특정 시간마다 작동하는 등, Github에서 지원하는 기능인 만큼 Git & Github와 호환성이 우월하다.
<!-- GIthub Action --> 
<br>

# Space Invader
## pause
>ESC키를 누르면 일시정지가 된다. 일시정지 상태에서 다시 ESC키를 누르면 게임을 다시 진행한다. 일시정지 상태에서 Q키를 누르면, 진행중인 게임을 즉시 종료하고 결과화면으로 넘어간다. 죽었을 때와 같은 판정으로 점수가 매겨진다.

<img src = "https://github.com/kjmin622/Invaders/blob/develop/img/space_invader/pause.png">
<br><br>

## 난이도 선택
>easy, normal, hard, extra hard로 구성된다. setting의 난이도 설정 기능에서 좌우 방향키로 난이도를 조정할 수 있다.

<img src = "https://github.com/kjmin622/Invaders/blob/develop/img/space_invader/difficulty.png">
<br><br>

## 멀티플레이
>두 명이서 게임을 할 수 있다. setting의 playermode 설정 기능에서 좌우 방향키로 모드를 바꿀 수 있다.

<img src = "https://github.com/kjmin622/Invaders/blob/develop/img/space_invader/multiplay.png">
<br><br> 
 
## 점수 기록
>각 난이도와 플레이어모드 별로 점수가 기록된다.

<img src = "https://github.com/kjmin622/Invaders/blob/develop/img/space_invader/highscores.png">
<br><br>

## 점수 리셋
>high scores에서 R키를 누르면 각 난이도와 플레이어모드 별로 점수를 리셋할 수 있다.

<img src = "https://github.com/kjmin622/Invaders/blob/develop/img/space_invader/reset.png">
<br><br> 

## 인터페이스 수정
>space키로만 이동이 되는 것에 ESC키, ENTER키도 추가하였다. setting에서 플레이어의 색깔을 바꿀 수 있다.

<img src = "https://github.com/kjmin622/Invaders/blob/develop/img/space_invader/interface.png">

