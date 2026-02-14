# neon-shooter
Game-neon_shooter-mobile

🚀 NEON SHOOTER
사이버펑크 세계관을 배경으로 한 HTML5 기반의 모바일 하이브리드 슈팅 게임입니다.
----------------------------------------------------------------------------------
🛠 Tech Stack
Frontend: HTML5, CSS3 (Neon UI), Vanilla JavaScript
Backend: AWS Lambda (Node.js 18.x)
Database: Amazon DynamoDB
API: AWS API Gateway
AI : Google Geminai
-----------------------------------------------------------------------------------
📊 Database Architecture (DynamoDB)
ns_leaderboard: 글로벌 랭킹 (PK: game_id, SK: score_composite)
ns_user_stat: 유저별 상태 및 인벤토리 (PK: user_id)
ns_mission_info: 다단계 미션 마스터 데이터 (성장 로직 포함)
ns_user_mission_stat: 유저별 미션 진행도 (PK: user_id, SK: mission_id)
ns_reward_info: 보상 아이템 정보
ns_banned_word: 비속어 필터링 리스트
-----------------------------------------------------------------------------------
✨ Key Features
Dynamic Background: 기기 시간대에 따라 배경 이미지 자동 전환 (새벽 2~6시 / 밤)
Multi-Mission System: ADD 및 MULT 성장 로직이 적용된 다중 미션 공존
Auto Reward: 미션 단계 클리어 시 인벤토리로 보상 자동 지급
Performance: 적 처치 데이터를 모아서 전송하는 배치 업데이트 로직 (AWS 비용 절감)
Anti-Cheat: 프론트엔드 난독화 및 체크섬 검증 로직 적용
-----------------------------------------------------------------------------------
📱 Mobile Testing
GitHub Pages URL 모바일 브라우저 테스트 진행
-----------------------------------------------------------------------------------
To Do 
- 안드로이드 APK 빌드 및 구글 플레이 스토어 출시
