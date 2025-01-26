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
#### 2. Google Re-Captcha(MFA) 적용
![recapcha](https://github.com/user-attachments/assets/54feeaa1-dbd2-48a4-9653-281f8b5f4619)




