# hobbyPlanet_Final
국비- 파이널 프로젝트

&nbsp;

## 1. 프로젝트 선정배경
코로나 19 발생 이후 취미생활의 폭이 좁아짐에 따라 공간적 , 시간적 영향을 많이 받게 되어버림. (예로 운동시설 운영 중단, 단체활동 제제 등) 
기존의 취미생활 관련 플랫폼의 경우 구독료, 관련재료 구매시 비용적인 면에서 부담스럽고, 문제해결방안에 대한 조언을 구하거나 친목을 하기 어려워짐. 이러한 문제를 해결하고자 기존의 취미생활 플랫폼과는 다른 정말로 다양한 사람들과 함께 취미생활을 즐길 수있는 플랫폼을 개발하는 것을 목표로 잡음


## 2. 제가 맡은 역할 : 
1. 팀장 (PPT 제작 및 발표, Use Case Diagram 제작 등)
2. 로그인/로그아웃/회원가입/탈퇴
3. 마이페이지 구현
                   
&nbsp;

## 3. 사용한 운영시스템(S/W)아키텍쳐
   
  
  
&nbsp;
  
## 4. 개발 일정
2022.10.19 ~ 2022.11.03

&nbsp;
  
## 5. Use Case Diagram 및 ERD / DB Table
### 회원 Use Case Diagram  및 ERD
![image](https://user-images.githubusercontent.com/109445583/199931086-e553c83f-9ab2-4c89-aec4-5e14377bfec2.png)

![image](https://user-images.githubusercontent.com/109445583/199931251-f0aecfa7-79a6-4363-8f8d-c2ca56022136.png)

### 관리자 Use Case Diagram 및 ERD
![image](https://user-images.githubusercontent.com/109445583/199931116-8eb49fd1-7ae2-4c01-b4b0-09b0559f41a4.png)

![image](https://user-images.githubusercontent.com/109445583/199931277-f78cc80c-bb5a-4b73-9292-924d10a09a33.png)

&nbsp;
  
## 6. 실행 방법
<details>
<summary>1. Final-Project용 계정 생성</summary>
계정이름: final 
비번: tiger

![image](https://user-images.githubusercontent.com/109445583/199931963-eb501e11-2495-4d51-b4ff-ea944217dd72.png)


![image](https://user-images.githubusercontent.com/109445583/199933193-a5ecbbdf-3f28-4583-87f5-b21aea6c603c.png)

</details>


<details>
<summary>2. Spring Tool Suit의 Server의 Tomcat에 추가</summary>
context.xml의 하단에 추가

    <Resource auth="Container" driverClassName="oracle.jdbc.driver.OracleDriver" maxActive="100"
    maxIdle="30" maxWait="10000" name="jdbc/oracle" password="tiger" type="javax.sql.DataSource"
    url="jdbc:oracle:thin:@localhost:1521:xe" username="final"  />

</details>

3. CreateSQL를 복사하여 Oracle SQL Developer에 실행 후 커밋

4. final_hobbyplanet.zip 파일 다운 받아 STS에 import후 실행

