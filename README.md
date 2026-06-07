# Market Overlay

Windows 데스크톱에서 시장 지표와 개인 포트폴리오 상태를 가볍게 확인하기 위한 투자 보조 오버레이입니다.

이 공개 저장소는 일반 사용자를 위한 배포용 저장소입니다. 설치파일, 사용자 가이드, 릴리즈 노트를 제공합니다.

## 다운로드

최신 설치파일은 GitHub Releases에서 받는 방식을 권장합니다.

- Releases: https://github.com/Link-1214/market-overlay/releases
- v1.9.0 설치파일: https://github.com/Link-1214/market-overlay/releases/download/v1.9.0/MarketOverlaySetup_v1.9.exe

저장소 안에도 동일 설치파일이 포함되어 있습니다.

```text
installer/v1.9/MarketOverlaySetup_v1.9.exe
```

## 주요 기능

- 시장 오버레이: CNN Fear & Greed, VIX, USD/KRW, S&P 500, Nasdaq Composite, KOSPI
- 종합 오버레이: 시장 상태와 포트폴리오 핵심 수치를 한 화면에 압축 표시
- 내 포트폴리오 오버레이: 총평가액, 원금, 수익, 전일대비, 비중 요약
- 포트폴리오별 보유종목, KRW/USD 예수금, 매수/매도/수정 기록 관리
- 매매기록과 배당기록 관리
- 성과비교, 포트/종목 비중 도넛, 기간별 히트맵

## 설치와 데이터

설치 후 실행 파일은 기본적으로 아래 위치에 설치됩니다.

```text
%LOCALAPPDATA%\Programs\Market Overlay\MarketOverlay.exe
```

개인 포트폴리오와 설정 데이터는 설치 폴더가 아니라 아래 위치에 저장됩니다.

```text
%APPDATA%\MarketOverlay
```

업데이트 설치는 이 개인 데이터를 보존합니다.

## 문서

- 사용자 가이드: `USER_GUIDE_V1_9.txt`
- 패치노트: `PATCH_NOTES_V1_9.txt`
- 릴리즈 노트: `RELEASE_NOTES_V1_9.md`

## 소스코드 접근

소스코드는 공개 배포 저장소에 포함하지 않습니다. 협업이 필요한 경우 저장소 관리자에게 별도 private repository 접근 권한을 요청하세요.

## 주의

- 이 앱은 투자 판단을 대신하지 않는 보조 도구입니다.
- Yahoo Finance 기반 조회값은 증권사 HTS/MTS와 지연, 환율, 세금, 수수료 기준이 다를 수 있습니다.
- 코드 서명이 없는 빌드라 Windows SmartScreen 또는 보안 프로그램 경고가 표시될 수 있습니다.
