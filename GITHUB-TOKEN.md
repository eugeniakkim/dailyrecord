# 🔑 GitHub Token 발급 가이드

GitHub 동기화를 사용하려면 Personal Access Token이 필요합니다.

## 📋 Token 발급 단계

### 1️⃣ GitHub Settings 접속
```
https://github.com/settings/tokens
```
또는
```
GitHub 로그인 → 오른쪽 상단 프로필 사진 클릭 
→ Settings → 왼쪽 메뉴 맨 아래 "Developer settings"
→ Personal access tokens → Tokens (classic)
```

### 2️⃣ Token 생성
1. **"Generate new token"** 클릭
2. **"Generate new token (classic)"** 선택

### 3️⃣ Token 설정
```
Note (설명):
  ✏️ Daily Record Token

Expiration (만료일):
  ⏰ No expiration (만료 없음)
  
Select scopes (권한):
  ✅ gist (이것만 체크!)
```

**중요**: `gist` 권한만 필요합니다. 다른 권한은 체크하지 마세요!

### 4️⃣ Token 생성 및 복사
1. 맨 아래 **"Generate token"** 클릭
2. 생성된 토큰이 표시됩니다
   - `ghp_`로 시작하는 긴 문자열
   - 예: `ghp_1A2b3C4d5E6f7G8h9I0jK1L2M3N4O5P6Q7R`
3. 🔴 **즉시 복사하세요!** (다시 볼 수 없습니다)
4. 안전한 곳에 저장 (메모장, 비밀번호 관리자 등)

---

## ⚙️ 앱에 Token 설정하기

### 1️⃣ 사이트 접속
```
https://eugeniakkim.github.io/dailyrecord
```

### 2️⃣ 설정 열기
1. 오른쪽 상단 **⚙️ 버튼** 클릭
2. "GitHub 동기화 설정" 패널 표시

### 3️⃣ Token 입력
1. "GitHub Personal Access Token" 필드에 토큰 붙여넣기
2. 자동으로 저장됩니다
3. **"완료"** 버튼 클릭

---

## 🎯 사용 방법

### 첫 번째 저장
```
1. "GitHub에 저장" 버튼 클릭
2. Gist ID가 자동으로 생성됩니다
3. 성공 메시지: ✅ GitHub에 저장 완료!
```

### 다른 기기에서 불러오기
```
1. 같은 Token을 설정
2. "GitHub에서 불러오기" 버튼 클릭
3. 데이터가 자동으로 동기화됩니다
```

### 데이터 업데이트
```
📱 휴대폰: 데이터 입력 → "GitHub에 저장"
💻 컴퓨터: "GitHub에서 불러오기" → 최신 데이터!
```

---

## 🔐 보안 주의사항

### ✅ 해도 되는 것
- Token을 비밀번호 관리자에 저장
- Token을 자신의 개인 메모에 보관
- 여러 기기에서 같은 Token 사용

### ❌ 절대 하지 말아야 할 것
- Token을 다른 사람과 공유
- Token을 공개 게시판에 올리기
- Token을 스크린샷 찍어서 SNS에 올리기
- Token이 포함된 코드를 GitHub에 푸시

### 🚨 Token이 유출되었다면?
1. 즉시 https://github.com/settings/tokens 접속
2. 해당 Token 삭제 (Delete)
3. 새 Token 재발급
4. 앱에서 새 Token으로 교체

---

## 🛠️ 문제 해결

### Token을 잃어버렸어요
→ 재발급 가능합니다. 위 단계를 다시 따라하세요.
→ 새 Token을 앱에 다시 입력하면 됩니다.

### "저장 실패" 오류가 나요
- Token이 올바른지 확인
- `gist` 권한이 있는지 확인
- Token이 만료되지 않았는지 확인

### "불러오기 실패" 오류가 나요
- Token이 올바른지 확인
- 먼저 "GitHub에 저장"을 한 번 실행했는지 확인
- Gist ID가 설정되었는지 확인

### Gist ID를 잃어버렸어요
→ https://gist.github.com 에서 "daily-record-data.json" 찾기
→ URL의 마지막 부분이 Gist ID입니다
→ 예: `https://gist.github.com/username/abc123def456` → `abc123def456`

---

## 💡 추가 팁

### Token 이름 잘 짓기
```
좋은 예:
- Daily Record Token
- 일상 기록 앱 전용
- Personal Tracker Sync

나쁜 예:
- test
- token1
- my_token
```

### 여러 앱에서 사용
- 하나의 Token으로 여러 기기 가능
- 각 기기마다 새로 발급할 필요 없음
- Token 하나로 평생 사용 가능

### 백업 추천
- Token을 안전한 곳에 백업
- 정기적으로 CSV도 백업 (이중 안전장치)

---

## 📱 실제 사용 예시

### 시나리오 1: 휴대폰 → 컴퓨터
```
1. 휴대폰에서 운동 기록 입력
2. "GitHub에 저장" 클릭
3. 집에서 컴퓨터로 사이트 접속
4. "GitHub에서 불러오기" 클릭
5. 휴대폰 데이터가 그대로!
```

### 시나리오 2: 여러 기기 동시 사용
```
📱 출근길: 야식 기록 → GitHub 저장
💼 회사: GitHub 불러오기 → 청약 추가 → GitHub 저장
🏠 집: GitHub 불러오기 → 모든 데이터 확인
```

### 시나리오 3: 백업 및 복원
```
정기 백업:
- 매주 일요일 "GitHub에 저장"
- 추가로 CSV도 다운로드

휴대폰 교체 시:
- 새 휴대폰에서 사이트 접속
- Token 입력
- "GitHub에서 불러오기"
- 모든 데이터 복원 완료!
```

---

## ✅ 체크리스트

설정 완료 확인:
- [ ] GitHub Token 발급
- [ ] Token을 안전한 곳에 저장
- [ ] 앱에서 Token 설정
- [ ] "GitHub에 저장" 한 번 실행
- [ ] Gist ID 자동 생성 확인
- [ ] 다른 기기에서 불러오기 테스트

---

완료! 이제 모든 기기에서 데이터를 동기화할 수 있습니다! 🎉
