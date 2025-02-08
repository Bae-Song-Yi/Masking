# 📋 개인 정보 마스킹
> 개인정보 보호를 위한 마스킹 서비스입니다. 사용자가 이미지를 업로드하고 민감한 정보를 직접 마스킹할 수 있는 기능을 제공합니다.

<br/><br/>
## 프로젝트 소개
- **개발 기간**: 2024.12 - 진행중
- **참여 인원**: 기획자1, 디자이너1, UI개발1, 백엔드 개발1
- **담당 업무**: UI 개발
<br/><br/>

## 🛠 사용 기술
- **Frontend**: HTML5, CSS3, JavaScript
- **Design**: Figma
- **Version Control**: Git
- **Communication**: Redmine
<br/><br/>

## 💻 주요 구현 사항
1. **파일 업로드 처리**
   - FileReader API를 활용한 이미지 미리보기
   - 지원 파일 형식 검증
<br/><br/>

2. **마스킹 기능**
   - 마우스/터치 이벤트를 활용한 드래그 방식 마스킹
   - 퍼센트 기반 반응형 마스킹 영역 계산
   - 실시간 마스킹 영역 시각화
<br/><br/>

3. **반응형 디자인**
   - PC/모바일 환경 대응
   - 터치 이벤트 최적화
   - 디바이스별 UI/UX 최적화
<br/><br/>

## 💡 문제 해결 및 핵심 기능
### 1. 직관적인 마스킹 UI/UX
- 드래그 방식으로 마스킹 영역을 지정하여 사용자 편의성 극대화
- 실시간 마스킹 미리보기로 즉각적인 피드백 제공
<br/><br/>

## 📊 성과
- 직관적인 UI로 사용자 진입장벽 최소화
- PC/모바일 크로스 브라우징 지원
- 안정적인 마스킹 기능 구현
>maskingWrap.addEventListener("mousedown", function (e) {
   isDrawing = true;
   const rect = this.getBoundingClientRect();
   prevX = ((e.clientX - rect.left) / this.offsetWidth) 100;
   prevY = ((e.clientY - rect.top) / this.offsetHeight) 100;
   // ... 마스킹 영역 생성 로직
   });

## 📱 UI/UX
![PC Flow](https://github.com/user-attachments/assets/5c38124b-dac5-4f19-946c-538847ba13cc)



개인정보 마스킹 URL : https://bae-song-yi.github.io/Masking/masking



