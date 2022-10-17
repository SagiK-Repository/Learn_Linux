문서정보 : 2022.10.17. 작성, 작성자 [@SAgiKPJH](https://github.com/SAgiKPJH)

# Linux 기초

## 목적 
- Linux 기초를 배운다.

<br>

## 목표 
- [ ] 개발자들이 리눅스를 쓰는 이유
- [ ] 리눅스 '커널'이 뭔가요
- [ ] 리눅스 환경 설치
- [ ] 리눅스 사용하기
- [ ] :bookmark_tabs: 교육 관련 총평(비평)

<br>

## 출처
- #1 
- [가장 쉬운 리눅스 강좌](https://www.youtube.com/watch?v=tPWBF13JIVk)

<br><br><br>


# 개발자들이 리눅스를 쓰는 이유

리눅스와 타 OS의 차이는 다음과 같다.
- 타 OS(Windows, Mac OS, Android, IOS)
  - 일반 사용자에게는 배우기 쉽다.
    - 일반인(개발자가 아닌 사람들) 즉, end-user를 대상으로 만들어진 운영체제이다.
  - GUI로 만들어진 화면에서, 개발자들이 다 만들어 놓은 기능을 사용하기만 하면 되도록 환경을 사용자에게 제공한다.
    - GUI : Graphic User Interface, 모든 요소들이 화면에 나타나 사용자들이 마우스 클릭으로 사용할 수 있다.
- 리눅스
  - 개발자들이 직접 만져보고 개조할 수 있도록 할 수 있다.
  - CLI로 이루어져 있다.
    - CLI : Command Line Interface, 모든 요소들이 명령줄 형식으로 나타나는 텍스트 터미널을 통해 컴퓨터와 상호작용을 하는 방식
  - 무료이고, 오픈소스이다.

<br><br><br>


# 개발자들이 리눅스를 쓰는 이유

리눅스와 타 OS의 차이는 다음과 같다.
- 타 OS(Windows, Mac OS, Android, IOS)
  - 일반 사용자에게는 배우기 쉽다.
    - 일반인(개발자가 아닌 사람들) 즉, end-user를 대상으로 만들어진 운영체제이다.
  - GUI로 만들어진 화면에서, 개발자들이 다 만들어 놓은 기능을 사용하기만 하면 되도록 환경을 사용자에게 제공한다.
    - GUI : Graphic User Interface, 모든 요소들이 화면에 나타나 사용자들이 마우스 클릭으로 사용할 수 있다.
- 리눅스
  - 개발자들이 직접 만져보고 개조할 수 있도록 할 수 있다.
  - CLI로 이루어져 있다.
    - CLI : Command Line Interface, 모든 요소들이 명령줄 형식으로 나타나는 텍스트 터미널을 통해 컴퓨터와 상호작용을 하는 방식
  - 무료이고, 오픈소스이다.

<br><br><br>


# 리눅스 '커널'이 뭔가요


<img src="https://user-images.githubusercontent.com/66783849/196072799-4bd18d0b-1380-44ae-9185-247e061bbf7e.png" width="250">  

> 리눅스의 커널 = 리눅스  
> 리눅스 - 칼, 커널 - 칼날

<br>

커널이란?
- 기계(CPU, Memory, Devices)를 최전선에서 직접 다루고 관리하는 것
- 커널 덕분에 기계에 명령을 내리고, 결과를 받아올 수 있다.

<br><br><br>


# 리눅스 환경 설치

리눅스의 가장 대중적인 배포판중 하나인 Ubuntu를 활용한다.  

환경 설치를 위한 방법 3가지  
1. 가상머신 소프트웨어
2. 온라인 IDE/터미널
3. 윈도우 10의 WSL

### 1. 가상머신 소프트웨어

- [VirtualBox 사이트](https://www.virtualbox.org/)에 이동하여 VirtualBox를 설치한다.
- [Ubuntu 사이트](https://ubuntu.com/)에 이동하여 Download > Desktop이 아닌 CLI이 기본으로 되어있는 Server 버전을 다운받는다.
- 설치한 VirtualBox > 새로 만들기 > 이름과 폴더위치 설정 > 종류 : Linux, 버전 : Ubuntu (64-bit) > 만들기 > 만들어낸 머신 시작 > 다운받은 Ubuntu.iso를 선택 > Start > CLI창이 나타나는 것을 확인한다.
- 화면이 작으면, View > Scaled Mode로 변경
- Ubuntu를 처음키면 나타나는 설치옵션들을 설정해준다.

<br>

### 2. 온라인 IDE/터미널

<img src="https://user-images.githubusercontent.com/66783849/196075154-5cb59b1c-3284-48fc-9844-42c820221d59.png" width="350">

- [goormide 사이트](https://ide.goorm.io/)에 가입 > 메인화면 > 대시보드(또는 콘솔로 가기) > + 새 컨테이너 > 이름 및 기타 설정 > 소프트웨어 스택 : Blank 선택 > 생성하기 > 터미널 실행 > 가상 리눅스가 만들어지고, 브라우저에서 바로 할용할 수 있다.  
  <img src="https://user-images.githubusercontent.com/66783849/196077023-c761ed98-e913-4730-ab29-9135ef5612f3.png" width="450">
- 또는 AWS의 Cloud9같은 온라인 IDE, Google Cloud의 Compute Engine 들을 활용할 수 있다.

<br>

### 3. 윈도우 10의 WSL

- 맥은 Linux와의 호환성이 높은데, 같은 Unix라는 운영체제에서 발전되어 왔기 때문이다.
- Windows는 2015년부터 WSL을 통해 리눅스를 돌려볼 수 있다.
- WSL로 윈도우에 리눅스를 설치한다.

<details> <summary>Window WSL2 Linux 설치 방법</summary>


## Window 10 WSL 2 ubuntu 설치

<br>

## 1. WSL2 설치 가능 여부 확인

- 설치 [사이트](https://docs.nvidia.com/cuda/wsl-user-guide/index.html)에 들어가 [A.1. Windows Insider Preview and Windows 10 Support](https://docs.nvidia.com/cuda/wsl-user-guide/index.html#installing-insider-preview-builds) 탭에 서술되어 있는 [ Releasing Windows 10 Build 19043.1263 (21H1) to Release Preview Channel](https://blogs.windows.com/windows-insider/2021/09/23/releasing-windows-10-build-19043-1263-21h1-to-release-preview-channel/)를 통해 Windows 버전을 확인한다.
- ✔버전은 Windows 10 Build 19043.1263(21H1) 이상이어야 가능한데, 확인은 다음과 같이 진행한다.
  - Windows 버전 확인  
    <img src="https://user-images.githubusercontent.com/66783849/195474219-bff6dca8-d131-4f74-988e-d528ee044f77.png" width="350">  
    - Window 탭 > 설정 > 업데이트 및 보안 > OS 빌드 및 시스템 정보 > Windows 사양
    - (또는) 파일 탐색기 > "내 PC" 오른쪽 마우스 > 설정 > Windows 사양
  - 다음을 확인한다.
    - ✔윈도우 에디션 : Windows 10 이상
    - ✔윈도우 버전 : 21H1 이상 확인
    - ✔OS 빌드 확인 : 19043.1263 이상 확인
  - 위 3가지를 만족하면 WSL2를 이용할 수 있다.

<br><br>

## 2. WSL2 설치

### (1). DISM으로 WSL 관련 기능 활설화

- PowerShell을 관리자 권한으로 실행한다.
- ✔Microsoft-Windows-Subsystem-Linux 기능을 활성화한다.
  ```bash
  dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
  ```
- 결과는 다음과 같다.
  ```bash
  $ dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
  버전: 10.0.19041.844
  
  이미지 버전: 10.0.19043.928
  기능을 사용하도록 설정하는 중
  [==========================100.0%==========================]
  ```
- ✔다음으로 dism 명령어로 VirtualMachinePlatform 기능을 활성화한다.
  ```bash
  dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
  ```
- 결과는 다음과 같다.
  ```bash
  $ dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
  배포 이미지 서비스 및 관리 도구
  
  이미지 버전: 10.0.19043.928
  
  기능을 사용하도록 설정하는 중
  [==========================100.0%==========================]
  작업을 완료했습니다.
  ```

<br>

### (2). WSL2 Linux 커널 업데이트

- [x64 머신용 최신 WSL2 Linux 커널 업데이트 패키지](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)를 다운받아 설치한다.
- ✔다음 명령어를 통해 WSL 버전을 WSL2로 변경한다.
  ```bash
  wsl --set-default-version 2
  ```

<br>

### (3). Microsoft Store 앱에서 ubuntu 다운  

<img src="https://user-images.githubusercontent.com/66783849/195476647-2fae4693-f866-4e94-9679-d4fdaae62145.png" width="350">  

- ✔Micorsoft 앱에서 ubuntu20.04, 22.04, 16.04 버전을 설치한다.

<br>

### (4). 설치 완료 확인  

   <img src="https://user-images.githubusercontent.com/66783849/195477457-2fcd3fa9-741c-4008-bcc2-ae3206f83d9b.png" width="350">  

   - ubuntu를 실행하면, 아이디와 비밀번호를 입력한다.
   - 이후 다음과 같이 ubuntu에 접속됨을 확인한다.  
     <img src="https://user-images.githubusercontent.com/66783849/195477264-b71d66fa-53e6-4524-8a19-631e9c899824.png" width="350">  
   - 다음 명령어를 통해 IP 번호를 확인해 둔다.
   ```bash
   ## 3가지 방법 중에 한 가지 활용
   hostname -I
   ip addr show
   ifconfig
   ```
   - IP 번호 예시 (172.26.11.120)

<br>

### (5). ubuntu 기타 설정

- 만일 ubuntu 설치하는 과정에서 비밀번호를 추가하지 않았다면, 다음을 통해 ✔최초 비밀번호를 설정한다.
  ```bash
  passwd
  # 또는
  sudo passwd
  ```

<br>

### (0). 출처 

- [Windows 10에 WSL 설치 | Microsoft Docs](https://learn.microsoft.com/ko-kr/windows/wsl/install#step-4---download-the-linux-kernel-update-package)
- [[Windows 10] WSL2 설치 및 사용법](https://www.lainyzine.com/ko/article/how-to-install-wsl2-and-use-linux-on-windows-10/)

</details> 

<br><br><br>
