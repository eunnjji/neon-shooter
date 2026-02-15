# 🚀 NEON SHOOTER
> **사이버펑크 세계관 배경의 모바일 하이브리드 슈팅 게임**

---

### 🛠 Tech Stack
* **Frontend**: HTML5 / CSS3 (Neon Style) / JS
* **Backend**: AWS Lambda (Node.js 18.x)
* **Database**: Amazon DynamoDB (NoSQL)
* **Gateway**: AWS API Gateway (REST API)
* **AI**: Google Gemini
---

### 📊 Database (DynamoDB)
| Table Name | Partition Key (PK) | Sort Key (SK) | Description |
| :--- | :--- | :--- | :--- |
| **`ns_rankings`** | `ns_pilot_id` | `ns_score` | 글로벌 랭킹 시스템 |
| **`ns_user_stat`** | `user_id` | - | 유저 상태 및 인벤토리 |
| **`ns_mission_info`** | `mission_id` | - | 미션 마스터 데이터 |
| **`ns_user_mission_stat`** | `user_id` | `mission_id` | 유저별 미션 진행도 |
| **`ns_reward_info`** | `reward_id` | - | 보상 아이템 정보 |
| **`ns_banned_word`** | `word_text` | - | 비속어 필터링 리스트 |

---

### ✨ Key Features
* **🌙 Dynamic Background**: 기기 시간대에 따른 배경 자동 전환 (새벽 02~06시 / 밤)
* **🎯 Multi-Mission**: `ADD` / `MULT` 로직 기반의 다단계 미션 시스템
* **🎁 Auto Reward**: 미션 클리어 시 인벤토리 자동 지급 로직
* **💰 Cost Optimization**: 배치(Batch) 업데이트를 통한 AWS 비용 절감
* **🛡 Security**: 체크섬 검증 및 프론트엔드 난독화 적용

---

### 📱 Testing & Deploy
1.  **GitHub Private** 저장소에 소스 업로드
2.  **GitHub Pages** 설정을 통해 테스트 URL 생성
3.  모바일 브라우저 접속 후 **[홈 화면에 추가]** 기능을 통해 테스트
4.  최종 목표: **Android APK** 빌드 및 스토어 출시

---
Copyright © 2026 NEON SHOOTER Project.
