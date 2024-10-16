<p align="right">
  [한국어]
  [<a href="README.md">English</a>]
</p>

# BooxResizer

BooxResizer는 Onyx Boox 전자책 리더기의 해상도에 맞게 이미지를 리사이즈하고 크롭하는 Python 스크립트입니다.

> 현재 인기있는 Onyx Boox 모델에 최적화되어 있으며, 향후 모든 Onyx Boox 모델을 지원할 예정입니다.

### Onyx Boox

- Go 10.3 (2480x1860)
- Tab X (1650×2200)
- Page (1264x1680)
- Note Air 2 Plus (1404x1872 )
- Go 6 (1072×1448)
- Palma (824x1648)
- Go Color 7 (1264x1680)
- Note Air 3 C (2480x1860)
- Tab Ultra C Pro (2480x1860)
- Tab Mini C (1872x1404)

### 기능

- 단일 이미지 또는 전체 디렉토리의 이미지를 한 번에 처리
- 인터랙티브 모드 지원 (대화형으로 쉬운 진행)
- 지원하는 이미지 포맷(`jpg`, `jpeg`, `png`)

<img width="682" alt="ss" src="https://github.com/user-attachments/assets/2c593a12-eb98-4d0d-a115-22089b6d40be">

### 설치

프로젝트를 클론합니다:

```bash
git clone https://github.com/micronzone/BooxResizer.git
cd BooxResizer
```

실행 권한 부여:
```bash
chmod +x booxresizer
```

별칭 추가 (선택 사항):

```bash
nano ~/.zshrc   # macOS ~/.zshrc, Linux `~/.bashrc` or `~/.zshrc`
alias booxresizer='/path/to/booxresizer'
```

```bash
source ~/.zshrc
```

### 종속성

[FFmpeg 공식 웹사이트](https://ffmpeg.org/download.html)에서 다운로드할 수 있습니다.

또는 MacOS의 경우:
```bash
brew install ffmpeg
```

### 사용법

BooxResizer는 명령줄 인터페이스(CLI)를 통해 사용하거나, 인터랙티브 모드를 통해 사용할 수 있습니다.

```bash
# booxresizer를 별칭에 추가한 실행 방법입니다(설치 참고) 또는 BooxResizer 디렉토리에서 ./booxresizer 실행
booxresizer
booxresizer [파일 또는 디렉토리]
```

### 예제

배경화면 디렉토리에 있는 단일 이미지 변환
```bash
booxresizer ~/배경화면/고양이.png
```

배경화면 디렉토리에 있는 모든 이미지 일괄 변환
```bash
booxresizer ~/배경화면
```

### 업데이트

BooxResizer 리포지토리 업데이트를 확인하는 것이 좋습니다!

```sh
cd BooxResizer
git status
```

변경 사항 가져오기:

```sh
git pull origin main
```

### 라이센스

이 프로젝트는 MIT 라이센스 하에 배포됩니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참고하세요.