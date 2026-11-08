# wolho-oss — 월호(月狐) 오픈소스 고지·소스 제공

월호(月狐)가 만든 프로그램에 함께 들어 있는 오픈소스 가운데, 라이선스가 **소스 코드 제공**을 요구하는 것(GPL·LGPL 등)의 **바이너리 사본과 대응 소스(Corresponding Source)** 를 이 저장소의 [Releases](https://github.com/sminhyeong/wolho-oss/releases) 에 둡니다. 누구나 무료로 받을 수 있습니다.

월호 프로그램 자체의 코드는 이 저장소에 없습니다. 여기에는 함께 배포하는 오픈소스 부분만 있습니다.

## 지금 있는 것

| 프로그램 | 함께 쓰는 오픈소스 | 라이선스 | 받는 곳 |
|---|---|---|---|
| Cutline (동영상 편집기, Windows) | FFmpeg — 별도 실행 파일로 불러 씀 | GPL v3 (함께 빌드된 라이브러리 포함) | 첫 배포 전에 Releases 에 올립니다 |

## Releases 규칙

- 태그 이름: `ffmpeg-<빌드 날짜>` (예: `ffmpeg-2026-10-31`) — 앱에 넣은 빌드와 같은 날짜
- 한 Release 에 들어가는 파일
  - 바이너리 사본 — 앱에 넣은 것과 똑같은 파일(원본 빌드: [BtbN/FFmpeg-Builds](https://github.com/BtbN/FFmpeg-Builds))
  - 대응 소스 — 그 빌드의 FFmpeg 소스, 함께 빌드된 모든 라이브러리 소스, 빌드 스크립트
  - `SHA256SUMS.txt` — 위 파일들의 SHA-256
- 받은 파일 확인(Windows PowerShell): `Get-FileHash <파일 이름> -Algorithm SHA256` 의 값이 `SHA256SUMS.txt` 와 같으면 올린 파일 그대로입니다.

## 고지와 문의

- 각 프로그램의 오픈소스 고지: 설치 폴더의 `THIRD_PARTY_NOTICES.txt`, 프로그램 안 「도움말 → 오픈소스 라이선스」
- 소스 제공에 관한 문의는 이 저장소의 [Issues](https://github.com/sminhyeong/wolho-oss/issues) 에 남겨 주세요.

## English

This repository hosts, in its [Releases](https://github.com/sminhyeong/wolho-oss/releases), binary copies and the complete Corresponding Source of open-source components that Wolho (月狐) apps distribute under licenses that require source availability (for example FFmpeg under the GPL). Downloads are free of charge. Each release is tagged `ffmpeg-<build date>` and contains the binary archive, the source archive and `SHA256SUMS.txt`. Questions about source availability: please open an [issue](https://github.com/sminhyeong/wolho-oss/issues).
