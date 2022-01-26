---
layout: page
title: Projects
excerpt: "A List of Projects"
comments: false
---

---

<span style="color:Salmon"> Click the titles to see the details </span>

<br>
<details>
  <summary> <span style="font-size: 20px"> (2021.04~2021.11) 다관절 로봇의 물리적 지능을 위한 교시학습 인공지능기술개발 </span> </summary>
  <div markdown="1">
This project was conducted at <span style="color:#3399ff">Cyber Physical System Control Lab in Kyungpook National University</span> : [Link](http://control.knu.ac.kr/)<br>
본 연구사업은 과학기술정보통신부의 출연금 등으로 수행하고 있는 <b>한국전자통신연구원의 대경권 지역산업 기반 ICT 융합기술 고도화 지원사업 위탁연구과제</b>입니다.
  </div>  
    <span style="font-size: 20px; color:black"> 연구목표 </span><br>
    <div style="border: 1px solid black; padding: 10px; border-color: LightGray; background-color: rgba(211, 211, 211, 0.2);"> 
      <span style="font-size: 13px">
        　■ 　로봇 매니퓰레이터의 Task 적용을 위한 힘/위치 궤적 교시학습 시스템 구축<br>
         　■ 　<b>[맡은 역할] 직접 교시를 통한 사용자 의도 파악(힘/위치)이 가능한 교시학습 알고리즘 개발</b><br>
         　■ 　7축 다관절 로봇을 활용한 실제 작업에 대한 모방학습 알고리즘 적용 및 검증<br>
        </span>
    </div>
    <br>
    <span style="font-size: 20px; color:black"> 연구내용 </span><br>
    
    <p align="center">
    <img height="250" src="/assets/img/2021_ETRI/block.bmp">
    <p style="text-align:center;">그림 1. 다관절 로봇의 힘/위치 교시학습을 위한 프레임 워크 구성 </p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/2021_ETRI/lstm.bmp">
    <p style="text-align:center;">그림 2. 로봇의 교시학습을 위한 LSTM 구조</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/2021_ETRI/demonstration.bmp">
    <p style="text-align:center;">그림 3. ○ 또는 ☆ 모양의 궤적 교시</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/2021_ETRI/cleaning.gif">
    <p style="text-align:center;">그림 4. PANDA 매니퓰레이터 클리닝 태스크 적용</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/2021_ETRI/writing.gif">
    <p style="text-align:center;">그림 5. PANDA 매니퓰레이터 글쓰기 태스크 적용</p>
    </p>
    
<br>
<span style="font-size: 20px; color:black"> 연구결과 </span><br>

본 연구에서는 다관절 로봇의 물리적 지능을 위한 교시학습 인공지능 기술을 제안하였고, 실제 산업용 로봇에 적용하여 제안한 방법의 효율성을 검증하였다. 산업에서 활용되는 대부분의 로봇들은 다양한 동작을 만들어 내기 위하여 6축 이상의 다관절로 이루어져 있다. 물리적 환경이 변화하는 산업 현장에서 다관절 로봇으로 주어진 태스크를 완벽하게 수행하기 위해서는 태스크를 능숙하게 수행할 수 있는 숙련자의 경험적 지식을 활용할 수 있어야 한다. 본 연구에서는 장단기 메모리(long short-term memory, LSTM) 딥러닝으로 로봇이 주어진 태스크를 수행하기에 필요한 물리적 지능(위치 및 힘 정보)을 생성하고, 로봇 제어시스템에 융합하였다. 본 연구에서 제안된 다관절 로봇을 위한 물리적 지능 시스템은 크게 2가지로 구성된다. 첫 번째는 로봇 제어시스템의 안정성을 보장할 수 있는 `임피던스 제어기 부분'이다. 임피던스 제어기를 구현하기 위해서는 로봇들이 가지는 기구학 및 동역학 모델을 실시간으로 계산해야 한다. 본 연구에서는 Franka Emika사의 7축 PANDA 로봇을 이용하였으며, 이 로봇의 기구학 및 동역학 모델을 계산하고 시뮬레이션 및 실험을 통하여 검증하였다. 계산된 로봇 모델을 이용하여 구현된 임피던스 제어기는 위치 및 힘 궤적을 추적할 수 있도록 설계하였다. 물리적 지능 시스템을 구성하는 마지막 부분은 `딥러닝을 이용한 교시학습 시스템'이다. 이 부분에서는 임피던스 제어기에서 추적하려는 궤적을 LSTM 딥러닝 방법으로 생성한다. 딥러닝에 이용되는 로봇의 상태 및 힘 정보는 데이터 수집 시스템을 통하여 로봇에서부터 획득되고 저장된다. 제안된 물리적 지능 시스템의 효율성을 검증하기 위해서 1) Writing 태스크, 2) Cleaning 태스크에 적용하였다. 제안된 시스템은 로봇이 이동해야 할 위치 궤적과 특정 시간에 작용 되어야 할 힘 궤적을 추적하며 태스크를 수행할 수 있는 특징을 가진다. 따라서 본 연구에서 제안된 기술은 위치와 힘 정보가 환경에 따라 변화할 수 있는 실제 산업 현장에서 많이 활용될 수 있으며, 물리적 지능 시스템을 위한 기술발전에 중요한 기여를 할 것이다.
</details>
    
<br>

---

<br>
<details>
  <summary> <span style="font-size: 20px"> (2020.09~) [Paper] Restored Action Generative Adversarial Imitation Learning from Observation for Robot Manipulator - Under Review </span> </summary>
  <div markdown="1">
This project was conducted at <span style="color:#3399ff">Cyber Physical System Control Lab in Kyungpook National University</span> : [Link](http://control.knu.ac.kr/)
      <br>본 논문은 2021년 5월 ISA Transactions (IF 5.468)에 투고하여 Major Revision을 거친 후 22년 1월 기준 <b>Under review</b> 상태 입니다.
  </div>  
   
    <span style="font-size: 20px; color:black"> Motivation </span><br>
    <div style="border: 1px solid black; padding: 10px; border-color: LightGray; background-color: rgba(211, 211, 211, 0.2);"> 
      <span style="font-size: 13px">
          ■ 　일반적으로 로봇에 적용하기 위한 모방학습 알고리즘은 상태-행동 데이터 쌍을 필요로 한다. <br>
　　기구학적 또는 비용적인 면에서 힘/토크 센서를 장착할 수 없는 경우에 시연으로부터 행동 데이터를 수집하기 어렵다.<br>
          ■ 　관측에 의한 모방학습 방법은 상태 데이터만을 활용한 모방학습 방법으로 제안되었지만, <br>
               　　계산복잡성에 의해 실제 로봇에 적용하기 어려운 문제가 있다.<br>
          ■ 　행동 데이터를 수집할 수 없는 상황에 적용할 수 있는 효과적인 모방학습 방법이 필요하다. <br>
        </span>
    </div>
    <br>
    <br>
    <span style="font-size: 20px; color:black"> Contribution </span><br>
    <div style="border: 1px solid black; padding: 10px; border-color: LightGray; background-color: rgba(211, 211, 211, 0.2);"> 
      <span style="font-size: 13px">
          ■ 　복원된 행동을 제안하여 행동 데이터에 접근할 수 없는 경우에 적용할 수 있는 모방학습 방법을 제안한다.<br>
          ■ 　시연자의 궤적 데이터를 효과적으로 학습할 수 있는 Recurrent Generative Adversarial Networks를 제안한다.<br>
          ■ 　제안하는 방법을 7축 매니퓰레이터 'SAWYER' Drawing TASK에 적용하여 제안하는 방법의 우수성을 검증한다.<br>
        </span>
    </div>
    
  <br>
    <span style="font-size: 20px; color:black"> Main Result </span><br>
    
    <p align="center">
    <img height="250" src="/assets/img/paper/motivation.png">
    <p style="text-align:center;">그림 1. 복원된 행동의 필요성</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/paper/ragil.png">
    <p style="text-align:center;">그림 2. 제안하는 RAGAIL 방법의 구성</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/paper/gathering.png">
    <p style="text-align:center;">그림 3. 교시데이터 수집</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/paper/triangle.png">
    <p style="text-align:center;">그림 4. 삼각형 그리기 태스크 수행 궤적</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/paper/triangle2.png">
    <p style="text-align:center;">그림 5. 삼각형 그리기 태스크 수행 궤적 PLOT</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/paper/triangle.gif">
    <p style="text-align:center;">그림 6. 삼각형 그리기 태스크 수행 궤적 영상</p>
    </p>
    
    <p align="center">
    <img height="250" src="/assets/img/paper/table.png">
    <p style="text-align:center;">그림 7. 기존의 방법들과 비교한 제안하는 방법의 우수성</p>
    </p>
    
    <br>
    <span style="font-size: 20px; color:black"> Conclusion </span><br>
    전문가의 행동 데이터에 접근할 수 없는 상황에서 복원된 행동을 이용한 모방학습 방법을 이용하여 태스크를 수행할 수 있음을 확인하고 우수한 성능을 보이는 것을 실험을 통해 검증했다.
</details>
    
<br>

---

<br>
<details>
  <summary> <span style="font-size: 20px"> (2020.04~2020.11) 다관절 로봇을 위한 인공지능 모방학습 기술 개발 </span> </summary>
  <div markdown="1">
This project was conducted at <span style="color:#3399ff">Cyber Physical System Control Lab in Kyungpook National University</span> : [Link](http://control.knu.ac.kr/)<br>
본 연구사업은 과학기술정보통신부의 출연금 등으로 수행하고 있는 <b>한국전자통신연구원의 대경권 지역산업 기반 ICT 융합기술 고도화 지원사업 위탁연구과제</b>입니다.
  </div>  
    <span style="font-size: 20px; color:black"> 연구목표 </span><br>
    <div style="border: 1px solid black; padding: 10px; border-color: LightGray; background-color: rgba(211, 211, 211, 0.2);"> 
      <span style="font-size: 13px">
        　■ 　<b>[맡은 역할] 가상환경을 활용한 로봇 매니퓰레이터의 경로 이동 모방학습방법 개발</b><br>
         　■ 　<b>[맡은 역할] 로봇의 교시 작업 시 사용자 의도 파악(힘+경로)을 위한 모방학습 알고리즘 개발</b><br>
         　■ 　<b>[맡은 역할] 다관절 로봇의 모방학습을 이용한 사용자 의도에 따른 접촉력 및 경로 이동작업 적용</b><br>
         　■ 　<b>[맡은 역할] Gazebo 가상환경 기반의 매니퓰레이터를 위한 학습환경 구축</b><br>
        </span>
    </div>
    <br>
        <span style="font-size: 20px; color:black"> 연구내용 </span><br>
    
    <p align="center">
  <img height="250" src="/assets/img/2020_ETRI/stage.bmp">
    <p style="text-align:center;">그림 1. 알고리즘 적용 순서</p>
    </p>
    
    <p align="center">
  <img height="250" src="/assets/img/2020_ETRI/gathering.PNG">
    <p style="text-align:center;">그림 2. 시연데이터 수집을 위한 환경구성</p>
    </p>
    
    <p align="center">
  <img height="250" src="/assets/img/2020_ETRI/gazebo.bmp">
    <p style="text-align:center;">그림 3. Gazebo환경 에서의 모방학습 테스트</p>
    </p>
    
    <p align="center">
  <img height="250" src="/assets/img/2020_ETRI/experiment2.bmp">
    <p style="text-align:center;">그림 4. 물체의 무게에 따른 분류 작업 태스크 설명</p>
    </p>
    
    <p align="center">
  <img height="250" src="/assets/img/2020_ETRI/experiment.bmp">
    <p style="text-align:center;">그림 5. 무게에 따라 각 관절에 측정되는 토크를 학습</p>
    </p>

    <p align="center">
  <img height="250" src="/assets/img/2020_ETRI/experiment3.PNG">
    <p style="text-align:center;">그림 6. 학습에 의한 무게에 따른 물체 분류 태스크</p>
    </p>
    
    <p align="center">
  <img height="250" src="/assets/img/2020_ETRI/ETRI.gif">
    <p style="text-align:center;">그림 7. 학습에 의한 무게에 따른 물체 분류 태스크 영상</p>
    </p>
    
    
<span style="font-size: 15px; color:black"> 알고리즘 적용 순서<br>1. 토크 센서에서 측정된 외부 토크 데이터를 수집하여 학습한다.<br> 2. 로봇의 각 조인트 각도 데이터를 수집하여 학습한다.<br> 3. 학습된 외력 추정 네트워크와 궤적 생성 네트워크 기반으로 시스템을 구성한다.<br> 4. 실제 로봇에 적용하여 태스크를 수행한다. <br> 실험결과 제안하는 모방학습 은 각기 다른 물병의 무게를 추정하고, 추정된 무게를 바탕으로 분류작업이 가능한 것을 확인하였다.<br>
본 연구에서는 다관절 로봇을 위한 새로운 모방학습 방법을 제안하였고, 모방학습에 필요한 데이터 수집 시스템을 구축하였다. 최근에 연구된 모방학습 기술 중의 하나인 generative adversarial network (GAN)방법을 기반으로 다관절 로봇에 작용하는 외력 추정 네트워크와 목표 궤적을 생성하는 네트워크를 이용하여 외력에 따른 로봇의 경로 이동 테스크를 성공적으로 수행하였다. 외력 추정 네트워크에서는 입력으로 로봇의 각 조인트 각도들과 외력을 이용하고, 출력으로는 0과 1사이의 실수 값을 가진다. 반면에, 목표 궤적을 생성하는 네트워크에서는 입력으로 외력 추정 네트워크에서 계산된 출력과 로봇의 각 조인트 각도들을 이용하고, 로봇의 각 조인트의 목표 각도/각속도를 출력으로 가진다. 목표 궤적 생성 네트워크에서 계산된 출력을 이용하여, 본 연구에서는 로봇의 PD제어기를 구성하였다. 이러한 제어 시스템을 구성함으로써 테스크를 성공적으로 수행할 수 있을 뿐만 아니라, 시스템의 안정성도 보장하게 된다. 제안된 학습방법을 이용하여, 로봇의 도형 그리기 테스크를 가상환경과 실제 환경에서 성공적으로 수행하였고, 또한 외력이 로봇에 작용하는 Pick & Place 테스크도 성공할 수 있었다. 더욱이, 본 연구에서는 모방학습을 위한 데이터 수집 시스템을 가상환경인 Unity에서 구축하였다. Unity에서는 Rethink Robotics사에서 제공한 Sawyer 로봇 unified robotic description format (URDF)파일을 이용하여 로봇의 그래픽을 구현하였고, 기구학/동역학 정보를 이용하여 학습에 필요한 데이터를 얻을 수 있도록 하였다. 가상환경의 데이터 수집 시스템은 실제 로봇이 없는 경우에도 전문가의 학습 데이터를 확보할 수 있다는 장점을 가진다. 따라서 본 연구에서 제안한 알고리즘 및 모방학습을 위한 데이터 수집 시스템은 현재의 모방학습 기술 발전에 많은 기여를 할 것이다. 
</span><br>

</details>
    
<br>

---

<br>
<details>
  <summary> <span style="font-size: 20px"> (2019.04~2019.11) 로봇의 센서리스 기반 외력 추정 및 임피던스 제어 </span> </summary>
  <div markdown="1">
This project was conducted at <span style="color:#3399ff">Cyber Physical System Control Lab in Kyungpook National University</span> : [Link](http://control.knu.ac.kr/)<br>
본 연구사업은 과학기술정보통신부의 출연금 등으로 수행하고 있는 <b>한국전자통신연구원의 대경권 지역산업 기반 ICT 융합기술 고도화 지원사업 위탁연구과제</b>입니다.
  </div>  
    
    <span style="font-size: 20px; color:black"> 연구목표 </span><br>
    <div style="border: 1px solid black; padding: 10px; border-color: LightGray; background-color: rgba(211, 211, 211, 0.2);"> 
      <span style="font-size: 13px">
        　■ 　토크 센서가 없는 로봇 매니퓰레이터에 대한 수학적 모델 기반 외력 추정 알고리즘 개발<br>
         　■ 　모델 불확실성에 강인한 센서리스 임피던스 제어 알고리즘 개발<br>
         　■ 　7축 로봇 매니퓰레이터 대상 태스크 종속적인 임피던스 제어 타당성 검증<br>
         　■ 　<b>[맡은 역할] 실험 환경 구성 및 알고리즘 코드 구현</b><br>
         　■ 　<b>[맡은 역할] ROS 기반의 매니퓰레이터 제어 시스템 구축</b><br>
        </span>
    </div>
    <br>
<br>
    
    
    <span style="font-size: 20px; color:black"> 연구내용 </span><br>
<p align="center">
  <img height="250" src="/assets/img/2019_ETRI/framework.png">
    <p style="text-align:center;">ROS 기반의 RNE 외력 추정 및 제어 시스템 구성</p>
</p>
    
<p align="center">
  <img height="250" src="/assets/img/2019_ETRI/python_c.bmp">
    <p style="text-align:center;">M,C,G 행렬 계산에 소요되는 시간 Python과 C++의 비교</p>
</p>

<p align="center">
  <img height="250" src="/assets/img/2019_ETRI/force-estimation.gif">
    <p style="text-align:center;">0번 조인트에 대한 외력추정 태스크<br>빨간 선 - 토크 센서로부터 측정된 토크, 파란 선 - 외력 추정 알고리즘에 의해 추정된 토크</p>
</p>


<p align="center">
  <img height="250" src="/assets/img/2019_ETRI/force-estimation2.gif">
    <p style="text-align:center;">외력추정 태스크<br>빨간 선 - ESO 알고리즘에 의해 정된 토크, 파란 선 - 센서에 의해 추정된 토크, 검은 선 - SMO에 의해 추정된 토크</p>
</p>

<p align="center">
  <img height="250" src="/assets/img/2019_ETRI/estimation.bmp">
    <p style="text-align:center;">각 조인트의 외력추정 성능 </p>
</p>

<span style="font-size: 20px; color:black"> 연구결과 </span><br>
c++을 이용하여 7축 매니퓰레이터를 위한 recursive Newton-Eulor 방법을 코드로 구현함으로서<br>Python으로 작성된 코드와 비교하여 계산속도 향상<br>
모델 불확실성에도 강인한 sliding mode observer 설계<br>
외력 추정기 기반 Joint space의 임피던스 제어기 설계<br>

</details>
    
<br>

---

<br>
<details>
  <summary> <span style="font-size: 20px"> (2019.03~2019.11) 지능형 이동로봇 추적제어 알고리즘 구현 및 실험 </span> </summary>
  <div markdown="1">
This project was conducted at <span style="color:#3399ff">Cyber Physical System Control Lab in Kyungpook National University</span> : [Link](http://control.knu.ac.kr/)
  </div>  
<p style="font-size:1rem;font-weight:400" onContextMenu="return false;" onselectstart="return false" ondragstart="return false">
　팔로워 로봇은 카메라를 이용하여 리더 로봇를 인식하고, 인식된 팔로워의 속도 및 각속도를 설계된 알고리즘에 의해 추정한다. 해당 프로젝트는 추정된 속도 및 각속도를 활용하여 리더-팔로워 추적 제어 구현을 목표로 한다.
</p>

<br>
<span style="font-size: 20px; color:black"> Leader-Follower 추적 제어를 위한 기구학적 모델링 </span><br>
    
<p align="center">
  <img height="250" src="/assets/img/Leader_follower/state_equation.png">
    <p style="text-align:center;">Leader-Follwer 추적 제어 시스템을 위한 상태 방정식</p>
</p>
<br>
<span style="font-size: 20px; color:black"> Gazebo 상에서 구현된 가상의 Leader 추적 제어 </span><br>
<p align="center">
  <img height="250" src="/assets/img/Leader_follower/gazebo_simulation.gif">
    <p style="text-align:center;">Leader-Follwer 추적 제어 시스템을 사용한 가상의 Leader 로봇 추적 시뮬레이션<br>빨간선 - 가상의 Leader의 궤적, 파란선 - Follwer의 궤적</p>
</p>
<br>
<span style="font-size: 20px; color:black"> Leader 로봇 인식과 속도 및 각속도 추정 </span><br>
<p align="center">
  <img height="250" src="/assets/img/Leader_follower/yolov2.gif">
    <p style="text-align:center;">YOLOv2를 사용한 Leader 로봇 인식</p>
</p>
<br>
<span style="font-size: 15px; color:black"> 1. Leader 로봇을 인식하고 Depth 카메라를 이용하여 거리값을 측정한다.<br> 2. Localization을 통하여 Global 맵상에 Leader 로봇의 궤적을 기록한다.<br> 3. 궤적중 여러 포인트를 샘플링하고 평균필터를 이용하여 리더 로봇의 각도와 각속도를 추정한다.<br> 4. 추정된 Leader 로봇의 각도와 각속도를 리더 추적 제어 시스템에 대입하여 추적제어를 수행한다. </span><br>
<br>
<span style="font-size: 20px; color:black"> 실제 실험을 통한 검증 </span><br>
<p align="center">
  <img height="250" src="/assets/img/Leader_follower/experiment.gif">
    <p style="text-align:center;">실제 실험을 통한 각도 및 각속도 추정기반의 추적 제어 알고리즘 성능 검증<br>Leader 로봇은 선속도 0.2m/s, 각속도 0.15rad/s로 움직인다.<br>실험을 통해 측정한 결과 평균오차 4%~6%를 기록하였다.</p>
</p>
</details>
    
<br>

---

<br>
<details>
  <summary> <span style="font-size: 20px"> (2018.06~2018.11) 2018 R-BIZ challenge  터틀봇3 오토레이스 </span> </summary>
  <div markdown="1">
This project was conducted at <span style="color:#3399ff">Cyber Physical System Control Lab in Kyungpook National University</span> : [Link](http://control.knu.ac.kr/)
  </div>  
<p style="font-size:1rem;font-weight:400" onContextMenu="return false;" onselectstart="return false" ondragstart="return false">
    <div style="border: 1px solid black; padding: 10px; border-color: LightGray; background-color: rgba(211, 211, 211, 0.2);"> 
      <span style="font-size: 13px">
          2018 R-BIZ Challenge 터틀봇 3 오토레이스는 주어진 6개의 미션 (1. 신호등 미션, 2. 삼거리 미션, 3. 공사구간 미션,<br> 
          4. 주차 미션, 5. 차단 바 미션, 6. 터널 미션)을 수행하며 사전에 설계된 경기장을 1회 주행하는 것을 목표로 한다.
        </span>
    </div>
</p>


<br>
<p style="font-size:1.5rem;font-weight:400" onContextMenu="return false;" onselectstart="return false" ondragstart="return false">
　Turtlebot3 AutoRacing Missions
</p>
<p align="center">
  <img height="250" src="/assets/img/Turtlebot3_AutoRacing/traffic.JPG">
</p>
<p align="center">
  <img height="250" src="/assets/img/Turtlebot3_AutoRacing/intersection.JPG">
</p>
<p align="center">
  <img height="250" src="/assets/img/Turtlebot3_AutoRacing/obstacle.JPG">
</p>
<p align="center">
  <img height="250" src="/assets/img/Turtlebot3_AutoRacing/parking.JPG">
</p>
<p align="center">
  <img height="250" src="/assets/img/Turtlebot3_AutoRacing/stop.JPG">
</p>
<p align="center">
  <img height="250" src="/assets/img/Turtlebot3_AutoRacing/tunnel.JPG">
</p>
                                                                      
<p align="center">
    <img height="250" src="/assets/img/Turtlebot3_AutoRacing/racing.gif">
    <p style="text-align:center;">그림 1. 대회주행 영상</p>
</p>
                                 
                                 
<p align="center">
  <img height="250" src="/assets/img/Turtlebot3_AutoRacing/award.jpg">
<p style="text-align:center;"> 학부생 (<b>박종천</b>, 이응창, 김범주, 대학원생 진용식)으로 이루어진 '응창호'팀이 11월 15~17일 3일간 대구 엑스코 전시장에서 열린 '2018 대구국제로봇산업전 R-BIZ Challenge 터틀봇3 오토레이스'부문에서 16일 준결승전에서 4등을 기록하는 등 <b>'매스웍스 코리아 대표이사상'(상금 100만원 등)</b>을 수상</p>
</p>
</details>
    
<br>

---

<br>
<details>
  <summary> <span style="font-size: 20px"> (2018.06~2018.11) 다중주기 센서융합 기반 이동체 실시간 예측 제어 연구 </span> </summary>
  <div markdown="1">
This project was conducted at <span style="color:#3399ff">Cyber Physical System Control Lab in Kyungpook National University</span> : [Link](http://control.knu.ac.kr/)<br>
      본 연구사업은 과학기술정보통신부의 출연금 등으로 수행하고 있는 <b>한국전자통신연구원의 대경권 지역산업 기반 ICT 융합기술 고도화 지원사업 위탁연구과제</b>입니다.

  </div>  
    <span style="font-size: 20px; color:black"> 연구목표 </span><br>
    <div style="border: 1px solid black; padding: 10px; border-color: LightGray; background-color: rgba(211, 211, 211, 0.2);"> 
      <span style="font-size: 13px">
        　■ 　다양한 샘플링 주기를 가지는 시스템의 안정성 및 제어 성능 향상을 위한 기법 연구 <br>
         　■ 　다중 샘플링 주기를 가지는 샘플 데이터 시스템을 위한 상태 추정기 설계 <br>
         　■ 　불확실성 및 왜란에 대응한 실시간 동작을 위한 모델 기반 예측 제어기 설계<br>
         　■ 　<b>[맡은 역할] 모바일 로봇을 위한 라이다센서 기반의 Path Planning 알고리즘 구현 및 적용</b><br>
         　■ 　<b>[맡은 역할] ROS 기반의 모바일 로봇 제어 시스템 구축</b><br>
        </span>
    </div>
    <br>
<br>
<p style="font-size:1.5rem;font-weight:400" onContextMenu="return false;" onselectstart="return false" ondragstart="return false">
라이다센서 기반의 Path Planning 알고리즘 구현 및 적용
</p>

<p align="center">
  <img height="250" src="/assets/img/2018_ETRI/vlp16.png">
    <p style="text-align:center;">라이다는 고출력의 펄스레이저를 이용하여 물체에 반사되어 돌아오는 레이저 빔의 시간을 측정하여 거리정보를 획득
카메라센서만으로 측정이 어려운 거리정보나, 비가 오거나 어두운 환경에서도 주변의 물체를 인식할 수 있다.</p>
</p>

<p style="font-size:1.5rem;font-weight:400" onContextMenu="return false;" onselectstart="return false" ondragstart="return false">
    <b>LiDAR를 이용한 Obstacle detection, Mapping과 A*기반의 Path Planning</b>
</p>

<p align="center">
  <img height="250" src="/assets/img/2018_ETRI/path_planning.png">
</p>
<p align="center">
  <img height="250" src="/assets/img/2018_ETRI/path_planning2.png">
</p>
<p align="center">
  <img height="250" src="/assets/img/2018_ETRI/path_planning3.png">
</p>

<p style="font-size:1.5rem;font-weight:400" onContextMenu="return false;" onselectstart="return false" ondragstart="return false">
    <b>LiDAR를 이용한 Obstacle detection, Mapping과 A*기반의 Path Planning</b>
</p>

<p align="center">
  <img height="250" src="/assets/img/2018_ETRI/autonomous.png">
  <p style="text-align:center;">ROS 기반의 autonomous vehicle control system</p>
</p>

<p align="center">
  <img height="250" src="/assets/img/2018_ETRI/husky-experiment.gif">
    <p style="text-align:center;">Husky로봇 야외 실험영상</p>
</p>
<p align="center">
  <img height="250" src="/assets/img/2018_ETRI/husky-experiment2.gif"> 
    <p style="text-align:center;">라이다 센서 기반의 Path planning </p>
</p>
    
    
</details>
    
<br>

---
