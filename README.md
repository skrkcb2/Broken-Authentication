# Broken-Authentication
### 특징: 사용자의 신원을 제대로 검증하지 못하는 문제로, 사용자가 인증을 우회하거나 부적절한 인증 절차를 거쳐 시스템에 접근할 수 있게 됩니다.
#### 취약 예시:
![image](https://github.com/user-attachments/assets/36a1069f-e5e4-4a72-8059-ab9c9bf7b3cf)
#### 공격 예시 / 버프 수트를 통한 무차별 공격
![auth](https://github.com/user-attachments/assets/38228f5f-22f8-457c-bdf1-ac3c4cac6310)
#### 보안 예시:
#### 로그인 횟수 제한(계정 잠금, 대기 시간 부여), 비밀번호 정책 변경(8자이상 대소문자, 숫자, 특수문자 조합), 인증 정보(세션, 토큰) 노출 방지(https, http only), MFA(다단계 인증 사용), 세션 관리 등이 있지만 그 중 로그인 횟수 제한, MFA적용 두 부분으로 방어를 해보겠습니다.  
#### 1. 로그인 횟수 제한  
![login](https://github.com/user-attachments/assets/567cb081-533e-4810-a3bb-ec3f3fc10a88)
#### 1.1 시큐어 코드(개발자 취향에 따라 각자 구현)
![image](https://github.com/user-attachments/assets/2580ee5e-46fd-434a-8153-390f8bd7d050)
![image](https://github.com/user-attachments/assets/4279d523-c431-47e5-b1ec-41ec5ff8c913)
#### 2. Google Re-Captcha(MFA) 적용
![recapcha](https://github.com/user-attachments/assets/54feeaa1-dbd2-48a4-9653-281f8b5f4619)
#### 2.1 시큐어 코드(구글 api 임으로 어느 개발자든 복붙 가능 / 초록색 박스가 추가 내용 or 없을 시 전체추가)  
#### 화면 추가  
![captcha](https://github.com/user-attachments/assets/a378fdd7-4f02-4ac4-b0de-db2f8c88ba4e)
#### API 추가 컨트롤러
![captcha-con](https://github.com/user-attachments/assets/15970529-33d6-4322-90b9-35cdd288884a)
#### API 추가Service
![captcha-serv](https://github.com/user-attachments/assets/1e9e7c00-f106-4282-8b9c-7076fab6fa95)
#### API 추가 VO
![captcha-vo](https://github.com/user-attachments/assets/b22e3cfe-e5a1-45b9-a3ef-e7dd08406e85)











