# 📋 개인 정보 마스킹

> 개인정보 보호를 위한 마스킹 서비스입니다. 사용자가 이미지를 업로드하고 민감한 정보를 직접 마스킹할 수 있는 기능을 제공합니다.

<br/><br/>

## 프로젝트 개요

- **기간**: 2024.12 - 진행중
- **역할**: UI 개발
- **팀 구성**: 기획자(1), 디자이너(1), UI개발자(1), 백엔드 개발자(1)
  <br/><br/>

## 🛠 기술 스택

- **Frontend**: HTML5, CSS3, JavaScript
- **Design**: Figma
- **Version Control**: Git
- **Communication**: Redmine
  <br/><br/>

## 💻 주요 기능 구현

### 1. **파일 업로드 및 미리보기**
- FileReader API를 활용한 이미지 미리보기
- 지원 파일 형식 검증

```javascript
function readURL(obj) {
  const reader = new FileReader();
  reader.onload = function (e) {
    // 이미지 미리보기 생성 및 표시
    const containers = document.querySelectorAll(".masking-wrap");
    containers.forEach((container) => {
      // ... 이미지 처리 로직
    });
  };
}
```
<br/><br/>
### 2. **마스킹 기능**
- 마우스/터치 이벤트를 활용한 드래그 방식 마스킹
- 퍼센트 기반 반응형 마스킹 영역 계산
- 실시간 마스킹 영역 시각화

```javascript
// PC 마스킹 이벤트
container.addEventListener("mousedown", function (e) {
  isDrawing = true;
  const rect = this.getBoundingClientRect();
  prevX = ((e.pageX - rect.left) / this.offsetWidth) * 100;
  prevY = ((e.pageY - rect.top) / this.offsetHeight) * 100;
  // ... 마스킹 영역 생성
});

// 모바일 터치 이벤트
container.addEventListener("touchstart", function (e) {
  if (e.touches.length === 1) {
    isDrawing = true;
    // ... 터치 기반 마스킹 처리
  }
});
```
<br/><br/>
### 3. **반응형 디자인**
- PC/모바일 환경 대응
- 터치 이벤트 최적화
- 디바이스별 UI/UX 최적화
  <br/><br/>

## 💡 핵심 구현 사항

### 1. 반응형 마스킹 처리

- 퍼센트 기반 좌표 계산으로 디바이스 크기 대응
- 터치/마우스 이벤트 통합 관리
<br/><br/>

### 2. 사용자 경험 최적화

- 실시간 마스킹 미리보기
- 초기화 및 재작업 기능
- 직관적인 UI/UX 설계
<br/><br/>

### 3. 크로스 브라우징

- PC/모바일 환경 호환성 확보
- 다양한 입력 방식 지원
  <br/><br/>

## 📊 성과

- 직관적인 마스킹 UI로 사용자 편의성 향상
- 안정적인 크로스 브라우징 지원
- 효율적인 개인정보 보호 솔루션 구현
  <br/><br/>

## 📱 UI/UX
![PC Flow (1)](https://github.com/user-attachments/assets/aec2036c-eca7-4edc-b22c-f0a37ab7288c)

개인정보 마스킹 URL : https://bae-song-yi.github.io/Masking/masking
