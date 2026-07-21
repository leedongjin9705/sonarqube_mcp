# sonarqube_mcp
sonarqube_mcp 사용 메뉴얼

part1

power shell, cursor, 도커 데스크탑 기준

SonarQube mcp 설치

파워쉘에 아래 명령어 입력
irm https://raw.githubusercontent.com/SonarSource/sonarqube-cli/refs/heads/master/user-scripts/install.ps1 | iex

파워쉘 재실행

sonar --version로 설치 확인. 버전이 나오면 성공

<img width="343" height="155" alt="image" src="https://github.com/user-attachments/assets/fc37e045-300b-40c6-852b-616f4c63f64b" />
SonarQube Cloud 선택

<img width="501" height="140" alt="image" src="https://github.com/user-attachments/assets/0f863e12-9bfb-494d-9aff-efa2bbc014ae" />
EU 리전 선택

엔터를 또 치면 소나 클라우드 로그인 화면으로 이동됨

로그인 이후 ALLOW Connection 클릭 -> 토큰 복사 -> 파워쉘이 입력 후 엔터.

다음으로 조직키(organization key)를 요구함.

<img width="246" height="229" alt="image" src="https://github.com/user-attachments/assets/8d5b7c83-aafc-4673-baa6-04549ffc0b21" />
<img width="1035" height="343" alt="image" src="https://github.com/user-attachments/assets/cf55b3c4-34e5-4b94-b452-3c4e0439fd44" />
이후 무료 플랜으로 생성해 주었음

<img width="630" height="95" alt="image" src="https://github.com/user-attachments/assets/ee354e88-a69e-4307-b5e2-c1efc559415c" />
완료

로그인 됐는지 확인 명령어
sonar auth status
<img width="817" height="228" alt="image" src="https://github.com/user-attachments/assets/ae09a2a7-ed77-431c-ab44-81305692ceac" />


도커 데스크탑 실행 -> cursor 재실행

<img width="1342" height="54" alt="image" src="https://github.com/user-attachments/assets/cfae4d99-1f0f-428e-b427-e1437de45067" />
자동으로 도커에 추가된 모습

다음으로 프롬프트에 "TV_OD_WEB 전체 Sonar 스캔 실행해줘"

SonarScanner로 전체 스캔

<img width="745" height="51" alt="image" src="https://github.com/user-attachments/assets/2befc1dd-101c-4449-8b18-1ad62c9a93ba" />
무료 플랜은 5만줄 인 듯 하다.

