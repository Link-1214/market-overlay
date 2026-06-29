# Market Overlay

주요 시장 지표와 개인 포트폴리오 상태를 데스크톱 오버레이로 확인하는 Windows용 투자 보조 도구입니다.

## 다운로드

- 최신 릴리즈: [Market Overlay Releases](https://github.com/Link-1214/market-overlay/releases)
- 현재 정식 버전: `v2.2`
- 설치 파일: [MarketOverlaySetup_v2.2.exe](https://github.com/Link-1214/market-overlay/releases/download/v2.2.0/MarketOverlaySetup_v2.2.exe)

설치 파일을 실행하면 기존 버전이 같은 경로에 업데이트 설치됩니다. 포트폴리오, 매매기록, 배당기록, 사용자 표시명, 설정은 `%APPDATA%\MarketOverlay`에 보관되어 업데이트 후에도 유지됩니다.

## 주요 기능

- 시장 오버레이: CNN F&G, VIX, USD/KRW, S&P 500, Nasdaq Composite, KOSPI 등 주요 지표 확인
- 종합 오버레이: 시장 요약과 포트폴리오 핵심 수치를 한 화면에 압축 표시
- 내 포트폴리오 오버레이: 총평가액, 원금, 수익, 전일대비, 현금비중 확인
- 포트폴리오 관리: 포트별 보유종목, 예수금, 매수/매도, 직접 수정
- 매매기록/배당 관리: 자동 기록과 수동 입력, 필터, 정렬
- 성과비교: 현재 보유구성을 주요 지수와 단순 비교
- 비중/트리맵: 현재 자산 비중과 선택 기간 수익률을 시각화

## v2.2 핵심 변경

- 포트폴리오 탭의 `비중/트리맵` 시각화 영역과 보유 목록 영역을 드래그로 조절할 수 있게 했습니다.
- `기본값` 버튼으로 시각화/목록 폭을 되돌릴 수 있고, 조절한 폭은 다음 실행 때 복원됩니다.
- 시장 데이터 조회 경계를 정리하고, v2.1에서 추가한 Yahoo 전일가 보정 경로를 회귀 테스트와 진단 로그 대상에 포함했습니다.
- `%APPDATA%\MarketOverlay\logs` 진단 로그와 설정 탭의 `로그 폴더 열기`를 추가했습니다.
- 내장 종목명 데이터를 최신화했습니다. 미국 12,881개, KRX 4,231개, JPX 4,446개, 총 21,558개입니다.

## 문서

- [사용자 가이드](USER_GUIDE_V2_2.txt)
- [이미지로 보는 사용자 가이드](docs/USER_GUIDE_SCREENSHOT_V2_2.md)
- [v2.2 패치노트](PATCH_NOTES_V2_2.txt)
- [v2.2 릴리즈 노트](RELEASE_NOTES_V2_2.md)
- [변경 이력](CHANGELOG.md)

이미지 가이드는 현재 v2.0 계열 예시 캡처를 사용합니다. v2.2의 splitter, 로그, state schema 변경은 문구로 보강했으며 실제 v2.2 최신 화면 캡처 교체는 후속 문서 보강 작업으로 남아 있습니다.

## 데이터와 주의

- 이 앱은 투자 판단을 대신하지 않는 보조 도구입니다.
- Yahoo Finance 기반 조회값은 증권사 HTS/MTS와 지연, 환율, 세금, 수수료 기준이 다를 수 있습니다.
- CNN Fear & Greed 조회 실패 시 Local F&G 대체 계산값을 표시할 수 있습니다.
- 코드 서명이 없는 개인 빌드라 Windows SmartScreen 또는 보안 프로그램 경고가 표시될 수 있습니다.
- 앱은 업데이트를 자동 다운로드하거나 자동 설치하지 않습니다. 새 버전이 있으면 GitHub Release 페이지로 이동합니다.

## 소스 코드

이 public repo는 일반 사용자 배포용입니다. 설치 파일, 사용자 가이드, 패치노트, 릴리즈 노트만 공개합니다.

개발 소스는 private repo에서 별도로 관리합니다. 코드 검토나 수정 협업이 필요하면 별도 권한을 받아 private repo를 사용하면 됩니다.
