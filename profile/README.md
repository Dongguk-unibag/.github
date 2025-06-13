## 🚀 학점가방 - **이제는 진짜 스마트하게**

학생 편의 개선 목적의 동국대학교 학사&생활 통합 플랫폼

![학점가방 배너](https://github.com/user-attachments/assets/3c093fb8-f86b-415e-a79f-535431ff4926)


## 📖 서비스 소개

- 기존의 동국대학교 서비스 사용에 있어 느린 속도와 친숙하지 않은 UI/UX로 인해 학생의 입장에서 불편함이 있었습니다.
- 학점가방에서는 동국대학교 서비스의 자원을 활용하여 이러한 불편함을 제거하고 부가적으로 학습 관련 기능을 제공하여 학생들의 대학 생활 편의를 개선하고자 하였습니다.
- 학점가방은 시간표 자동 불러오기, 친한 친구들과의 시간표 공유, 손쉬운 과제 메모, 모바일 학생증 등의 다양한 편의 기능을 제공합니다.

</br>

## ✨ 서비스 기능

### [회원기능]
| <img src="https://github.com/user-attachments/assets/b0abcdcb-99ee-4a63-8bdc-661a8580c6c1" width="160"/> | <img src="https://github.com/user-attachments/assets/59f52c8a-bcb6-47e9-8802-d569d56087cf" width="160"/> | <img src="https://github.com/user-attachments/assets/988a6c8a-a3d4-4360-b802-98a78253fb49" width="160"/> | <img src="https://github.com/user-attachments/assets/413861db-e73d-4214-88b3-e17e0a8190a5" width="160"/> | <img src="https://github.com/user-attachments/assets/c17cff5b-b314-4ea5-a639-504bb252302b" width="160"/> |
| --- | --- | --- | --- | --- |
| 초기 화면 | 로그인 | EMS 로그인 | 로그아웃 | 회원 탈퇴 |

**초기 화면**

- 초기 화면에서는 사용자의 기존 로그인 여부를 확인하는 과정이 진행됩니다. 이 과정 동안 로딩 인디케이터가 표시됩니다. 로그인에 성공하면 메인페이지로 이동합니다.

**OAuth 기반 로그인**

- 사용자의 세션이 만료된 경우 로그인 화면으로 이동하며 카카오 혹은 애플 로그인 버튼을 터치하여 로그인이 가능합니다.

**nDrims 로그인**

- 동국대학교 nDrims 계정으로 로그인하여 본교 학생임을 인증합니다.
- 친구 기능, 학교 시간표 불러오기, 학생증 등 동국대학교 자원이 필요한 기능에 접근할 때  nDrims 로그인이 선행되어야 합니다.

**로그아웃**

- 로그아웃이 완료되면 FlutterSecureStorage 내 저장된 계정 정보(AccessToken, RefreshToken, asid, 학번 등)이 삭제되고 로그인 페이지로 이동합니다.

**회원탈퇴**

- 회원 탈퇴를 하게되면 해당 유저의 모든 정보가 사용자의 디바이스 및 서버에서 삭제되고 로그인 페이지로 이동합니다.

</br>
</br>

### [시간표 기능]

| <img src="https://github.com/user-attachments/assets/3aa4707a-e60d-4f8f-be13-d9d4eb58e66d" width="160"/> | <img src="https://github.com/user-attachments/assets/7d72a4b7-cd08-4724-9282-f196aa63d12d" width="160"/> | <img src="https://github.com/user-attachments/assets/ad735280-ec7b-44aa-86a5-4a917a467d63" width="160"/> | <img src="https://github.com/user-attachments/assets/772c3159-90b1-49b1-b62d-89ac2a57d3ac" width="160"/> |
| --- | --- | --- | --- |
| 시간표 불러오기 | 시간표 직접 등록 | 대표 시간표 설정 | 시간표 삭제 |

**시간표 불러오기**

- 동국대학교 서버에 저장된 유저의 특정 시간표를 크롤링을 통해 불러와 서버에 등록 후 유저에게 보여줍니다.

**시간표 직접 등록**

- 유저가 직접 자신의 시간표를 등록합니다.
- 필터링을 통해 특정 강의를 검색할 수 있습니다.
- 테마를 통해 시간표별로 자신의 원하는 색상을 고를 수 있습니다.

**대표 시간표 지정**

- 여러개의 시간표 중 유저가 제일 먼저 보고 싶은 시간표를 지정할 수 있습니다.
- 해당 시간표는 추후 자신을 친구로 등록한 다른 유저에게도 보여집니다.

**시간표 삭제**

- 등록된 시간표를 목록에서 삭제합니다.

</br>
</br>

### [친구 기능]

| <img src="https://github.com/user-attachments/assets/68a224f1-2519-4ecb-a4c8-fb391943ac66" width="160"/> | <img src="https://github.com/user-attachments/assets/1b2b9fea-ed2c-4598-a0a8-075fb6b4d0a3" width="160"/> | <img src="https://github.com/user-attachments/assets/07df9b6d-1dd0-41d0-a075-ec33a7a9503e" width="160"/> | <img src="https://github.com/user-attachments/assets/db3369b4-0df3-4be6-b8c2-df39e8bf9318" width="160"/> |
| --- | --- | --- | --- |
| 친구 등록 | 친구 삭제 | 공강 찾기 | 친한친구 관리 |

**친구 등록**

- 친구를 이름과 학번으로 조회하여 추가할 수 있습니다.

**친구 삭제**

- 등록된 친구를 목록에서 삭제합니다.

**공강 찾기**

- 친구 목록에서 선택된 친구들 사이에서 겹치는 공강 시간만을 보여줍니다.

**친한 친구 관리**

- 빠르게 확인할 친구 시간표를 친구목록에서 선택할 수 있습니다.
- 보여지는 친구 시간표는 친구가 설정한 대표 시간표입니다.

</br>
</br>

### [과제 기능]

| <img src="https://github.com/user-attachments/assets/fc39d04d-dd54-4021-b883-362259c2a56d" width="160"/> | <img src="https://github.com/user-attachments/assets/860d9fea-e2cb-4683-9f0b-a777c9605035" width="160"/> | <img src="https://github.com/user-attachments/assets/a2641e47-45b4-4c7c-8e98-4f615e4d5e10" width="160"/> | <img src="https://github.com/user-attachments/assets/2580ea1a-bbeb-451d-a6a8-206edca97e08" width="160"/> | <img src="https://github.com/user-attachments/assets/2278e92d-3298-4f89-ad36-eafc1daec43b" width="160"/> |
| --- | --- | --- | --- | --- |
| 과제 등록 | 과제 삭제 | 과제 완료 체크 | 과제 수정 | 과제 일괄 삭제 |

**과제 등록**

- 과목, 기한, 제목, 내용을 작성하여 과제를 등록합니다.
- 마감 기한 전 사용자에게 알림을 전송합니다(백엔드에서만 구현 됨).
- 마감 기한이 설정된 경우 상단의 타임라인에도 과제 제목이 표시됩니다.

**과제 삭제**

- 등록된 과제를 목록에서 삭제합니다.

**과제 완료 체크**

- 과제 완료가 되었으면 해당 과제가 가장 하단으로 이동합니다.
- 또한 마감 기한이 설정된 경우 상단의 타임라인에서 과제 제목이 삭제됩니다.

**과제 수정**

- 등록된 과제에 대해 과목, 기한, 제목, 내용을 수정합니다.

**과제 일괄 삭제**

- 완료된 과제들을 목록에서 전부 삭제합니다.

</br>
</br>

### 신분증 기능

| <img src="https://github.com/user-attachments/assets/a38525d1-2315-476b-bb47-d0ac18786335" width="160"/> |
| --- |
| 신분증 |
- 동국대학교의 학생임을 인증을 신분증을 보여줍니다.
- 신분증에는 유저의 이름, 학번, 전공, QR코드가 표시됩니다.
- QR코드는 30초를 주기로 자동 갱신됩니다.

</br>



## ⚒️ 기술 스택
- **Framework**: `Flutter`, `Spring Boot`

- **Language**: `Python`

- **Database**: `MySQL`, `Redis`

- **Container&Deploy**: `Docker`, `Github Actions`

- **Messaging**: `FCM (Firebase Cloud Messaging)`

- **Monitoring**: `Loki`, `Prometheus`, `Grafana`

</br>

## 🏛️ 서비스 아키텍쳐 
| <img src="https://github.com/user-attachments/assets/05ea7caa-3a6a-4524-af5f-80d783db369a" width="500"/> | <img src="https://github.com/user-attachments/assets/e714fc04-a663-4521-b41f-c44108ad2792" width="500"/> |
| --- | --- |
| 아키텍쳐 | ERD |

</br>

## 🧑🏻‍💻 팀원 구성 & 역할
| ✨김광래 | 김동규 | 김희진 | 임채강 | 최민수 |
| :---: | :---: | :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/c78c754f-02d2-4607-9df9-ac15a9912e0b" width="200"/> | <img src="https://github.com/user-attachments/assets/96574fb1-7b42-45dd-8ad7-21ed4464f119" width="200"/> | <img src="https://github.com/user-attachments/assets/9489e917-c744-4f26-80c8-e077b76e0e15" width="200"/> | <img src="https://github.com/user-attachments/assets/80b1a053-0970-475e-92b8-9a636f51febb" width="200"/> | <img src="https://github.com/user-attachments/assets/a4d37556-d21d-40b6-95fc-f17df8d2e05a" width="200"/> |
| ✨[@kkr010128](https://github.com/kkr010128) | [@KDongGyu1](https://github.com/KDongGyu1) | [@gmlwls768](https://github.com/gmlwls768) | [@chaegang01](https://github.com/chaegang01) | [@최민수](https://github.com/minnnisu) |
| 프로젝트 리더<br>프론트엔드 개발 | 프론트엔드 개발 | 백엔드 개발 | 프론트엔드 개발 | 프론트엔드 개발<br>백엔드 개발 |

</br>
