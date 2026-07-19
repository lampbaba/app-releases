# app-releases

**한 곳에서 받는 테스트용 APK 모음** — lampbaba가 개발하는 여러 앱의 개발/테스트 빌드를
프로젝트별 릴리스로 배포합니다. (소스는 각 프로젝트의 Private 저장소에 있고, 여기엔 APK만 올립니다.)

## 다운로드 페이지 (QR)
👉 **https://lampbaba.github.io/app-releases/**

폰으로 위 페이지를 열거나 QR을 찍으면 최신 테스트 APK를 바로 받을 수 있습니다.

## 프로젝트별 고정 링크 (항상 최신 빌드)
| 앱 | 다운로드 |
|----|----------|
| VPNPilot | https://github.com/lampbaba/app-releases/releases/download/vpnpilot/vpnpilot.apk |

> 각 프로젝트는 **릴리스 태그 하나**(= 프로젝트명)를 쓰고, 새 빌드는 그 릴리스의 APK를 **덮어씁니다**(롤링).
> 링크는 바뀌지 않습니다. 새 앱이 생기면 리포를 새로 만들지 않고 **릴리스 태그만 추가**합니다.

## 새 빌드 올리기
```powershell
# 프로젝트 폴더에서 flutter build apk --release 후:
powershell -File <경로>\publish-apk.ps1 -Project <프로젝트명> -Apk <app-release.apk 경로>
```

## 참고
- 공개 저장소라 APK는 링크만 알면 누구나 받을 수 있습니다(소스는 비공개). 테스트 배포용입니다.
- 설치 시 "출처를 알 수 없는 앱" 허용이 필요할 수 있습니다.
