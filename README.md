# TFVision

ThinkingFriends의 비전 분석 데스크톱 애플리케이션입니다.

Windows와 macOS 설치 파일은 소스 저장소의 릴리스 워크플로에서 자동으로 빌드되어 이 저장소의 [GitHub Releases](https://github.com/kimgangmin-thinkingfriends/tfvision-release/releases)에 게시됩니다.

> 아직 Release가 없다면 아래 최신 다운로드 링크는 첫 버전이 배포된 뒤 활성화됩니다.

## 최신 버전 다운로드

| 운영체제 | 패키지 | 다운로드 |
|---|---|---|
| Windows 10/11 x64 | EXE 설치 프로그램 (권장) | [TFVision-windows-x64-setup.exe](https://github.com/kimgangmin-thinkingfriends/tfvision-release/releases/latest/download/TFVision-windows-x64-setup.exe) |
| Windows 10/11 x64 | MSI 패키지 | [TFVision-windows-x64.msi](https://github.com/kimgangmin-thinkingfriends/tfvision-release/releases/latest/download/TFVision-windows-x64.msi) |
| macOS 10.15+ Intel | DMG | [TFVision-macos-intel.dmg](https://github.com/kimgangmin-thinkingfriends/tfvision-release/releases/latest/download/TFVision-macos-intel.dmg) |
| macOS 10.15+ Apple Silicon | DMG | [TFVision-macos-apple-silicon.dmg](https://github.com/kimgangmin-thinkingfriends/tfvision-release/releases/latest/download/TFVision-macos-apple-silicon.dmg) |

[전체 버전과 릴리스 노트 보기](https://github.com/kimgangmin-thinkingfriends/tfvision-release/releases)

## 설치 안내

### Windows

일반 사용자는 `TFVision-windows-x64-setup.exe`를 권장합니다. 조직의 소프트웨어 배포 도구를 사용하는 경우 MSI 패키지를 사용할 수 있습니다.

### macOS

Mac의 **이 Mac에 관하여**에서 프로세서를 확인한 뒤 Intel 또는 Apple Silicon용 DMG를 내려받습니다. DMG를 열고 TFVision을 Applications 폴더로 이동합니다.

## 파일 무결성 확인

각 Release에는 모든 설치 파일의 SHA-256 값이 담긴 [SHA256SUMS.txt](https://github.com/kimgangmin-thinkingfriends/tfvision-release/releases/latest/download/SHA256SUMS.txt)가 포함됩니다.

Windows PowerShell:

```powershell
Get-FileHash .\TFVision-windows-x64-setup.exe -Algorithm SHA256
```

macOS:

```bash
shasum -a 256 TFVision-macos-apple-silicon.dmg
```

출력된 값이 `SHA256SUMS.txt`의 값과 같은지 확인합니다.

## 코드 서명 안내

현재 배포 패키지는 정식 게시자 인증서로 서명·공증되지 않을 수 있습니다. 따라서 Windows SmartScreen 또는 macOS Gatekeeper 경고가 나타날 수 있습니다. 정식 코드 서명 적용 여부는 각 Release의 안내를 확인하세요.
