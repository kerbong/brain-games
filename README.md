# 🎮 두뇌 게임 모음

교실용 미니 게임 2종 모음. localStorage로 개인 기록 저장.

## 📂 파일 구성

```
index.html              ← 메인 페이지 (두 게임 입구)
dopamine-brain.html     ← 도파민에 절여진 뇌 구하기
classroom-games.html    ← 학생들과 함께!
```

## 🎯 게임 목록

### 🧠 도파민에 절여진 뇌 구하기 (`dopamine-brain.html`)
- **🎨 색깔과 글자의 싸움 (스트룹 테스트)**: 30초 동안 글자의 색깔을 빠르게 맞히기
- **🔢 3초 전을 기억하라 (숫자 메모리)**: 잠깐 보이는 숫자를 기억하기, 자릿수 늘리기

### 🎓 학생들과 함께! (`classroom-games.html`)
- **🔤 한글 자음 퀴즈**: 8개 카테고리 (동물/음식/나라/스포츠/한국사/연예/과학/속담) + 전체 랜덤
- **🎯 1부터 25까지! (슐테 테이블)**: 3×3, 5×5, 6×6 난이도 선택

## 🚀 깃허브 페이지스 배포 방법

### 1. 새 저장소 만들기
- GitHub에서 새 repository 생성 (예: `brain-games`)
- Public으로 설정

### 2. 파일 업로드
- `index.html`, `dopamine-brain.html`, `classroom-games.html` 세 파일 업로드
- 커밋

### 3. 페이지스 활성화
- Settings → Pages
- Source: `Deploy from a branch` 선택
- Branch: `main` / `(root)` 선택 후 Save
- 1~2분 대기

### 4. 접속
- `https://<유저명>.github.io/<저장소명>/` 으로 접속
- 예: `https://kerbong.github.io/brain-games/`

## 💾 점수 저장 방식

- **localStorage 사용**: 본인 브라우저에만 저장됩니다
- 게임별로 TOP 5 기록 유지
- 시크릿 모드/다른 기기에서는 기록이 보이지 않습니다
- 브라우저 데이터 삭제 시 기록도 함께 삭제됩니다

## 🔧 커스터마이징 팁

### 자음 퀴즈 문제 추가하기
`classroom-games.html` 안의 `QUIZ_DATA` 객체를 찾아 원하는 카테고리에 추가:
```javascript
['ㅇㅇ', '단어'],  // [자음, 정답] 형식
```

### 시간 제한 변경하기
- 스트룹: `stroopTime = 30;` (초)
- 자음 퀴즈: `quizTime = 60;` (초)

### 색상 테마 변경하기
각 HTML 파일 상단 `:root` 안의 CSS 변수 수정:
```css
--accent: #ff5a36;  /* 메인 색상 */
```

## 📱 호환성

- PC / 모바일 / 태블릿 모두 지원
- 최신 Chrome, Safari, Edge, Firefox 권장
- 화면 회전 가로/세로 모두 OK

## 📝 라이선스

자유롭게 사용/수정 가능. 교실 활용 환영.
