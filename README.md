# direct-shop-frontend

## 직거래 쇼핑몰

### 사용자가 직접 승용차를 올릴 수 있는 플랫폼

## 개발전

### GITHUB Commit convention

- [feat] ⇒ 새로운 기능추가 및 구현관련
- [fix] ⇒ 버그가 생겼을때의 수정RE
- [misc] ⇒ 간단한 코드수정 [ 기타 ]
- [design] ⇒ CSS및 사용자 UI나 디자인 변경

### 사용자 요구사항

1. 회원가입이 되야한다.
2. 로그인, 로그아웃할 수 있다.
3. 회원정보 수정, 탈퇴가 된다.
4. 브랜드별, cc기준별(대형 중형 소형 경형), 연식, 키로수, (등급, 신차가격, 옵션 등은 추후)
5. 지역, 자동차명, 설명, 사진 기입이 가능하다.
6. 판매중, 예약, 판매완료 확인이 가능하다.
7. (추가)구매문의를 1:1 채팅으로 가능하다.
8. (추가)채팅이 신청되었을 시 신청알림이 뜬다.
9. (추가)마이페이지에서 판매중, 예약, 판매완료, 채팅내역을 확인할 수 있다.

### 기능적 요구사항 정의서

|요구사항ID|요구사항명|기능ID|기능명|상세설명|필수데이터|선택데이터|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|M001|회원가입|M001_SINGUP_01|회원가입 입력정보|회원가입할 시 정보를 입력할 수 있다.|ID, PWD, NAME, PHONE|ADDR, BIRTH, DESC|
|M001|회원가입|M001_SIGNUP_02|회원가입 검증|회원가입 입력정보를 검증한다.|ID, PWD, NAME, PHONE| ADDR, BIRTH, DESC|
|M002|로그인|M002_SIGNIN_01|로그인 요청|로그인정보를 입력하여 로그인할 수 있다.|ID, PWD||
|M002|로그인|M002_SIGNIN_02|로그인 실패|로그인정보입력이 잘못됬을 때 검증할 수 있다.|ID, PWD||
|M002|로그인|M002_SIGNIN_03|아이디, 비밀번호 찾기|로그인 정보를 분실했을 시 찾을 수 있다.|ID, NAME, PHONE||
|M003|회원정보 수정|M003_EDIT_01|회원정보 수정|선택정보를 수정할 수 있다.|PWD, NAME, PHONE|ADDR, DESC|
|M003|회원정보 수정|M003_EDIT_02|회원정보 수정 검증|선택정보를 검증하여 오류처리|PWD, NAME, PHONE|ADDR, DESC|
|M004|회원탈퇴|M004_DEL_01|회원탈퇴|회원탈퇴를 할 수 있다.|회원탈퇴 시 일정정보를 입력하여 탈퇴가능하다.|PWD||
|M004|회원탈퇴|M004_DEL_02|회원탈퇴 알림|탈퇴면 회원이 로그인이나 가입시도 시 알려줄 수 있다.|MEMBER_STATE||
|M005|로그아웃|M005_LOGOUT_01|로그아웃|로그아웃 시 권한이 필요한 동작의 경우 로그인이나 회원가입 안내|||
|P001|상품|P001_CREATE_01|상품 등록|차량을 등록할 수 있다.|TITLE, CONT, BRAND, SIZE, YEAR, USED_KM|PIC|
|P001|상품|P001_EDIT_01|상품 수정|등록한 차량을 수정할 수 있다.|TITLE, CONT, BRAND, SIZE, YEAR, USED_KM|PIC|
|P001|상품|P001_DEL_01|상품 삭제|등록한 차량을 삭제할 수 있다.|PWD||
|P002|상품조회|P002_READ_01|상품 조회|전체 리스트에 내 차량이 등록되면 조회가 가능하다.|||
|P002|상품조회|P002_READ_02|상품 상세 조회|차량에 상세 정보를 조회할 수 있다.|||
|P002|상품조회|P002_READ_03|내 상품 조회|마이페이지에서 내가 등록한 상품을 조회할 수 있다.|||
|S001|상품상태|S001_READ_01|상품 상태|상품의 상태에 따라 구분할 수 있다.|PRD_STATE: 0(판매중), 1(예약중), 3(판매완료)||
|S001|상품상태|S002_EDIT_01|상품 상태 변경|내가 등록한 차량의 판매상태를 수정할 수 있다.|PRD_STATE: 0(판매중), 1(예약중), 3(판매완료)||

### [USERS FLOWS](https://www.figma.com/file/Nc7NMyaTX7E69h41p1TtIL/Untitled?node-id=0%3A1&t=uN6EgjRcS723hvLJ-1)

완성 후 사진첨부

### [PROTOTYPE](https://www.figma.com/file/GSCfLZMBhV06qwJobiQgCO/Dev_Direct_ShoppingMall?t=uN6EgjRcS723hvLJ-1)

완성 후 사진첨부

#### MAIN

#### SINGUP

#### SIGNIN

#### LOGOUT

#### MEMBER_EDIT

#### PRODUCT_CREATE

#### PRODUCT_EDIT

#### PRODUCT_DELETE

#### PRODUCT_LIST

##### PUBLIC_LIST

##### MYPAGE_LIST

#### PRODUCT_DETAIL

#### PRODUCT_STATE

## 개발

진행전

1. 배포방식 결정해야됨

## 개발 후

진행전

1. 변경사항 문서 최신화
2. 기능 붙을거 추가논의
