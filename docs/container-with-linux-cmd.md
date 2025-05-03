# Linux 컨테이너 실습

[Linux container from scratch](https://michalpitr.substack.com/p/linux-container-from-scratch) 글을 참고하여, 도커 없이 리눅스 컨테이너를 직접 구현해보는 실습

---

## 호스트 환경
- **운영체제**: macOS (Apple Silicon - M3 Pro)
- **가상화 도구**: [UTM](https://mac.getutm.app/)
- **메모리**: 18GB

---

## 가상 머신 환경
- **운영체제**: Ubuntu 22.04 (64-bit)
- **CPU**: 2코어
- **메모리**: 4GB
- **디스크**: 32GB

---

## 실습 환경 구성

### 1. UTM 설치
- [UTM 공식 사이트](https://mac.getutm.app/)에서 다운로드  
  (앱스토어 버전은 유료이나, 무료 버전과 기능 차이 없음)

### 2. 가상 머신 생성
1. [Ubuntu 22.04 ARM ISO 이미지 다운로드](https://cdimage.ubuntu.com/releases/22.04/release/)
2. UTM 실행 후 다음 순서로 가상 머신 생성
   - 새 가상 머신 만들기 → 가상화 → Linux 선택
   - 부팅 ISO 이미지에 위에서 받은 Ubuntu ISO 지정
   - 메모리: 4096MB / CPU: 2코어 설정
   - 디스크: 32GiB 설정
   - 공유 디렉토리: 원하는 폴더 하나 선택
   - 이름 입력 후 저장

### 3. Ubuntu 설치
- 설치 시 기본 설정으로 진행: `Continue` → `Done` 선택
- `display output is not active` 메시지가 보이더라도 5~10초 후 설치 화면이 나타남
- 설치 완료 후 `Reboot` 선택 → 화면이 멈춘 것처럼 보여도 정상  
  → UTM의 가상 머신 목록에서 해당 머신을 **중지**한 뒤 CD/DVD 제거 → 다시 시작
- 설치 시 설정한 계정으로 로그인하여 Ubuntu 접속

---

## 사전 학습
- [링크]()

## 실습 과정
