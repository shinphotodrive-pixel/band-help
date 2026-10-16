# 네이버 밴드 해킹 긴급 대처 센터 (Emergency Response Center)

네이버 밴드 계정 도용 및 리더(방장) 권한 탈취 피해 발생 시 즉각적인 초동 대처 및 1:1 고객센터 신고, 사이버수사국 신고 가이드를 제공하는 웹 서비스입니다.

## 주요 기능
- **현재 피해 상황 요약**: 피해 밴드, 탈취자(해커 닉네임), 확인된 밴드 URL 제공
- **긴급 초동 조치 가이드**: 전 기기 강제 로그아웃 및 2단계 인증 설정 안내
- **1:1 문의 내용 자동 생성기**: 밴드 헬프센터 제출용 텍스트 클립보드 원클릭 복사
- **경찰청 사이버수사국(ECRM) & KISA 신고 안내**: 2차 피해 예방 가이드

## GitHub Pages 배포 방법

### 1. GitHub에서 신규 리포지토리 생성
1. [GitHub](https://github.com/new)에 로그인하여 새 리포지토리(`band-emergency-help` 등)를 생성합니다.
2. `Public` 또는 `Private`을 선택합니다. (무료 계정에서 GitHub Pages 배포는 `Public` 권장)

### 2. 로컬 저장소와 원격 저장소 연결 및 푸시
터미널에서 아래 명령어를 실행하여 생성한 GitHub 리포지토리로 코드를 업로드합니다:

```bash
git remote add origin https://github.com/shinphotodrive-pixel/band-help.git
git push -u origin main
```

### 3. GitHub Pages 설정 활성화
1. GitHub 리포지토리 페이지의 **Settings > Pages** 메뉴로 이동합니다.
2. **Build and deployment > Source** 항목에서:
   - **GitHub Actions** 를 선택합니다. (제공된 `.github/workflows/deploy.yml`에 의해 자동 배포됩니다)
3. 푸시가 완료되면 몇 초 뒤 상단에 생성된 배포 URL (`https://<아이디>.github.io/<리포지토리>/`)로 웹페이지가 즉시 공개됩니다.
