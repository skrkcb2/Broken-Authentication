# Broken-Authentication
#### 특징: 사용자의 신원을 제대로 검증하지 못하는 문제로, 사용자가 인증을 우회하거나 부적절한 인증 절차를 거쳐 시스템에 접근할 수 있게 됩니다.
- ## 공격 유형:
  - ### 1. Broken-Authentication 취약 코드
      ![image](https://github.com/user-attachments/assets/36a1069f-e5e4-4a72-8059-ab9c9bf7b3cf)
  - ### 공격 체크 / 버프 수트를 통한 무차별 공격
      ![auth](https://github.com/user-attachments/assets/38228f5f-22f8-457c-bdf1-ac3c4cac6310)
  - ## 보안 유형:
    ```
    1. 로그인 횟수 제한(계정 잠금, 대기 시간 부여) 
    2. 비밀번호 정책 변경(8자이상 대소문자, 숫자, 특수문자 조합)
    3. 인증 정보(세션, 토큰) 노출 방지(https, http only)
    4. MFA(다단계 인증 사용)
    5. 세션 관리
    ```
    #### 이 중 로그인 횟수 제한, MFA적용 두 부분으로 방어를 해보겠습니다.  
    - ### 1. 로그인 횟수 제한  
        ![login](https://github.com/user-attachments/assets/567cb081-533e-4810-a3bb-ec3f3fc10a88)
    - ### 1.1 시큐어 코드(개발자 취향에 따라 각자 구현)
        ![image](https://github.com/user-attachments/assets/2580ee5e-46fd-434a-8153-390f8bd7d050)
        ![image](https://github.com/user-attachments/assets/4279d523-c431-47e5-b1ec-41ec5ff8c913)
    - ### 2. Google Re-Captcha(MFA) 적용
        ![recapcha](https://github.com/user-attachments/assets/54feeaa1-dbd2-48a4-9653-281f8b5f4619)
    - ### 2.1 시큐어 코드  
        #### 화면 추가  
        ![captcha](https://github.com/user-attachments/assets/a378fdd7-4f02-4ac4-b0de-db2f8c88ba4e)
        #### API 추가 컨트롤러
        ![captcha-con](https://github.com/user-attachments/assets/15970529-33d6-4322-90b9-35cdd288884a)
        #### API 추가Service
        ![captcha-serv](https://github.com/user-attachments/assets/1e9e7c00-f106-4282-8b9c-7076fab6fa95)
        #### API 추가 VO
        ![captcha-vo](https://github.com/user-attachments/assets/b22e3cfe-e5a1-45b9-a3ef-e7dd08406e85)

#### MFA 추가 시 인증 우회 방지, 봇 방지(무차별 공격), 계정 잠금 및 타임아웃, 로그인 시도 제한, 로그인 요소 이중화, 실패 시 패턴 진화 등 Broken-Authentication에 문제점을 매우 효과적으로 막아준다.(개발자의 설정에 따라 다르다).











