# 🔄 GitHub Pages 업데이트 방법

기존에 배포된 사이트를 새 버전으로 업데이트하는 방법입니다.

## 방법 1: 웹에서 직접 업데이트 (가장 쉬움)

### 1️⃣ GitHub 리포지토리 접속
```
https://github.com/eugeniakkim/dailyrecord
```

### 2️⃣ index.html 파일 교체
1. 리포지토리에서 기존 `index.html` 클릭
2. 오른쪽 상단 **쓰레기통 아이콘** (Delete) 클릭
3. 하단에 "Delete index.html" 커밋
4. 메인 페이지로 돌아가기
5. **Add file** → **Upload files** 클릭
6. 새 `index.html` 파일 드래그
7. **Commit changes** 클릭

### 3️⃣ README.md도 업데이트 (선택)
- 같은 방법으로 `README.md`도 교체

### 4️⃣ 완료!
```
2-3분 기다리면 자동으로 배포됩니다.
https://eugeniakkim.github.io/dailyrecord
```

---

## 방법 2: Git으로 업데이트 (개발자용)

```bash
# 1. 리포지토리 클론 (처음 한 번만)
git clone https://github.com/eugeniakkim/dailyrecord.git
cd dailyrecord

# 2. 파일 교체
# index.html을 새 파일로 교체

# 3. 커밋 & 푸시
git add index.html
git commit -m "Update to dark mode with new features"
git push

# 4. 완료! (자동 배포)
```

---

## ⚠️ 업데이트 전 주의사항

### 데이터 백업
현재 사이트에서 사용 중이라면:
```
1. 기존 사이트 접속
2. "CSV로 저장" 클릭
3. 백업 파일 다운로드
4. 새 버전 배포 후
5. "CSV 불러오기"로 복원
```

### 캐시 문제
업데이트 후에도 예전 버전이 보이면:
```
1. Ctrl + F5 (강력 새로고침)
2. 또는 브라우저 캐시 삭제
```

---

## 🆕 새 버전의 주요 변화

### 추가된 기능
✅ 다크 모드  
✅ 1주일 보기 - 달력 형식  
✅ 드래그 앤 드롭 CSV 업로드  
✅ 데이터 초기화 버튼  
✅ CSV 내보내기 - 모든 컬럼 포함  

### 기본 샘플 데이터
- 타이드 - 청약 - 반포 래미안 트리니원
- 타이드 - 야식 - 떡볶이, 김1개
- 누렁이 - 소화제 - 파인애플
- 타이드 - 운동 - pt 30분

---

## 🎯 체크리스트

업데이트 전:
- [ ] 현재 데이터 CSV로 백업
- [ ] 새 index.html 파일 다운로드 확인

업데이트:
- [ ] GitHub 리포지토리 접속
- [ ] 기존 index.html 삭제
- [ ] 새 index.html 업로드
- [ ] Commit changes

확인:
- [ ] 2-3분 대기
- [ ] 사이트 접속 (Ctrl+F5로 새로고침)
- [ ] 다크 모드 확인
- [ ] 기본 샘플 데이터 4개 확인
- [ ] CSV 백업 파일 불러오기 (필요시)

---

## 🆘 문제 해결

**예전 버전이 계속 보여요**
→ Ctrl + F5 (강력 새로고침)
→ 시크릿 모드로 접속해보기

**데이터가 사라졌어요**
→ 백업한 CSV 파일로 복원
→ "CSV 불러오기" 또는 드래그 앤 드롭

**404 에러가 나요**
→ 파일 이름이 정확히 `index.html`인지 확인
→ Settings > Pages에서 배포 상태 확인

---

## 💡 추천 워크플로우

```
1. 기존 사이트에서 CSV 백업
2. GitHub에 새 버전 업로드
3. 2-3분 대기
4. 새 사이트 접속 (Ctrl+F5)
5. "데이터 초기화" 클릭 (기본 4개만 남김)
6. 필요한 데이터만 CSV에서 불러오기
```

이렇게 하면 깔끔하게 시작할 수 있습니다! 🎉
